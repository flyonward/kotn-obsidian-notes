```button
name New NPC
type note(NewNPC, split) template
action template_NPC
templater true
```
^button-NewNPCButtonID

// Templater:
// To move file to specified folder, then show pop-up prompt for file name
// \*However, this does not prevent Templater from running upon file creation where the default filename is "Untitled". Thus, using `<% tp.file.title %>` with the below code will result in "Untitled" wherever used.

```
<% await tp.file.move("/Places/" + tp.file.title) %>

<%*
const hasTitle = !tp.file.title.startsWith("Untitled");
let title;
if (!hasTitle) {
    title = await tp.system.prompt("Enter Dungeon Name");
    await tp.file.rename(title);
} else {
    title = tp.file.title;
}
_%>
```

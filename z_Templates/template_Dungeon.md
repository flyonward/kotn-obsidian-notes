---
type: place
subtype: dungeon
location: <% tp.file.title %>
dg-publish: true
---
## Summary
<% tp.file.cursor() %>

## People / Characters
```dataview
table description as "Description" from "Characters"
where type = "npc" and contains(location, "<% tp.file.title %>")
sort file.name ASC
```

## Other Tidbits & Misc Info

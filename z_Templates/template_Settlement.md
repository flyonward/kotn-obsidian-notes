---
type: place
subtype: settlement
location: <% tp.file.title %>
description: <% tp.file.cursor() %>
dg-publish: true
---
## Summary

## Landmarks / POIs

```dataview
table description as "Description" from "Places/POIs"
where type = "poi" and contains(location, "<% tp.file.title %>")
sort file.name ASC
```

## Shops
```dataview
table proprietor as "Proprietor", shop_type as "Description" from "Places/Shops"
where type = "shop" and contains(location, "<% tp.file.title %>")
sort file.name ASC
```

## People / Characters
```dataview
table description as "Description" from "Characters"
where type = "npc" and contains(location, "<% tp.file.title %>")
sort file.name ASC
```

## Other Tidbits & Misc Info

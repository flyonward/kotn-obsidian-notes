---
type: place
subtype: settlement
location: Calling Horns
description: A small town that started as a roadside inn until purchased and expanded upon by Tamalin Zoar.
dg-publish: true
---
## Summary
A small settlement that first began as a roadside inn. A town was built around the inn after it was purchased by [[Tamalin Zoar]].
## Landmarks / POIs

```dataview
table description as "Description" from "Places/POIs"
where type = "poi" and contains(location, "Calling Horn")
sort file.name ASC
```

## Shops
```dataview
table proprietor as "Proprietor", shop_type as "Description" from "Places/Shops"
where type = "shop" and contains(location, "Calling Horn")
sort file.name ASC
```

## People / Characters
```dataview
table description as "Description" from "Characters"
where type = "npc" and contains(location, "Calling Horn")
sort file.name ASC
```

## Other Tidbits & Misc Info

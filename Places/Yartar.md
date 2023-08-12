---
type: place
subtype: settlement
location: Yartar
description: An industrial river port
dg-publish: true
---
## Summary
An industrial river port, led by an elected leader called the [[Water Baron]].
## Landmarks / POIs

```dataview
table description as "Description" from "Places/POIs"
where type = "poi" and contains(location, "Yartar")
sort file.name ASC
```

## Shops
```dataview
table proprietor as "Proprietor", shop_type as "Description" from "Places/Shops"
where type = "shop" and contains(location, "Yartar")
sort file.name ASC
```

## People / Characters
```dataview
table description as "Description" from "Characters"
where type = "npc" and contains(location, "Yartar")
sort file.name ASC
```

## Other Tidbits & Misc Info

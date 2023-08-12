---
type: place
subtype: settlement
location: Phandalin
description: A town built in ruins
dg-publish: true
---
## Summary
Noted as a "town built in ruins".

## Landmarks / POIs

```dataview
table description as "Description" from "Places/POIs"
where type = "poi" and contains(location, "Phandalin")
sort file.name ASC
```

## Shops
```dataview
table proprietor as "Proprietor", shop_type as "Description" from "Places/Shops"
where type = "shop" and contains(location, "Phandalin")
sort file.name ASC
```

## People / Characters
```dataview
table description as "Description" from "Characters"
where type = "npc" and contains(location, "Phandalin")
sort file.name ASC
```

## Other Tidbits & Misc Info

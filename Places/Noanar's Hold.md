---
type: place
subtype: settlement
location: Noanar's Hold
description: A small, spooky village with a shuttered keep standing on a hill, looming over the village.
dg-publish: true
---
## Summary
Noanar's Hold is a spooky little village with rattled folk and a creepy shuttered keep located on a hill, overlooking the village.
## Landmarks / POIs

```dataview
table description as "Description" from "Places/POIs"
where type = "poi" and contains(location, "Noanar's Hold")
sort file.name ASC
```

## Shops
```dataview
table proprietor as "Proprietor", shop_type as "Description" from "Places/Shops"
where type = "shop" and contains(location, "Noanar's Hold")
sort file.name ASC
```

## People / Characters
```dataview
table description as "Description" from "Characters"
where type = "npc" and contains(location, "Noanar's Hold")
sort file.name ASC
```

## Other Tidbits & Misc Info

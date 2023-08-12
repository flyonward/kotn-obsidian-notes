---
type: place
subtype: settlement
location: Triboar
description: A bustling mercantile town.
dg-publish: true
---
## Summary
A bustling mercantile town.
## Landmarks / POIs

```dataview
table description as "Description" from "Places/POIs"
where type = "poi" and contains(location, "Triboar")
sort file.name ASC
```

## Shops
```dataview
table proprietor as "Proprietor", shop_type as "Description" from "Places/Shops"
where type = "shop" and contains(location, "Triboar")
sort file.name ASC
```

## People / Characters
```dataview
table description as "Description" from "Characters"
where type = "npc" and contains(location, "Triboar")
sort file.name ASC
```

## Other Tidbits & Misc Info

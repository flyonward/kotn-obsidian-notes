---
type: place
subtype: settlement
location: Neverwinter
description: A large, bustling, cosmopolitan city.
dg-publish: true
---
## Summary
![[NeverwinterHarbor.webp]]
A large, bustling, cosmopolitan city.

## Landmarks / POIs

```dataview
table description as "Description" from "Places/POIs"
where type = "poi" and contains(location, "Neverwinter")
sort file.name ASC
```

## Shops
```dataview
table proprietor as "Proprietor", shop_type as "Description" from "Places/Shops"
where type = "shop" and contains(location, "Neverwinter")
sort file.name ASC
```

## People / Characters
```dataview
table description as "Description" from "Characters"
where type = "npc" and contains(location, "Neverwinter")
sort file.name ASC
```

## Other Tidbits & Misc Info

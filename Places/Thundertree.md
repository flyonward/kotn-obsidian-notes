---
type: place
subtype: settlement
location: Thundertree
description: A town in ruins, plagued by zombies
dg-publish: true
---
## Summary
A town in ruins, plagued by zombies brought on by the eruption of Mt. Hotenow 30 years ago.

## Landmarks / POIs

```dataview
table description as "Description" from "Places/POIs"
where type = "poi" and contains(location, "Thundertree")
sort file.name ASC
```

## Shops
```dataview
table proprietor as "Proprietor", shop_type as "Description" from "Places/Shops"
where type = "shop" and contains(location, "Thundertree")
sort file.name ASC
```

## People / Characters
```dataview
table description as "Description" from "Characters"
where type = "npc" and contains(location, "Thundertree")
sort file.name ASC
```

## Other Tidbits & Misc Info

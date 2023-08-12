---
type: place
subtype: settlement
location: Giant Castle On A Cloud
description: A castle for giants, floating atop a cloud.
dg-publish: true
---
## Summary
A castle for giants, floating atop a cloud.

## Landmarks / POIs

```dataview
table description as "Description" from "Places/POIs"
where type = "poi" and contains(location, "Giant Castle On A Cloud")
sort file.name ASC
```

## Shops
```dataview
table proprietor as "Proprietor", shop_type as "Description" from "Places/Shops"
where type = "shop" and contains(location, "Giant Castle On A Cloud")
sort file.name ASC
```

## People / Characters
```dataview
table description as "Description" from "Characters"
where type = "npc" and contains(location, "Giant Castle On A Cloud")
sort file.name ASC
```

## Other Tidbits & Misc Info

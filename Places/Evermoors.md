---
type: place
subtype: area
location: Evermoors
description: A region located southwest of Silverymoon, comprised of hills and troughs and partially filled with swamps, chilly bogs, and rolling landscapes.
aliases: [Trollmoors]
dg-publish: true
---
## Summary
A region located southwest of [[Silverymoon]], comprised of hills and troughs and partially filled with swamps, chilly bogs, and rolling landscapes. There is a dense fog that permeates throughout the area and frequent gusts of wind. It is said that the swamps in this area are heavily infested with trolls.
## Landmarks / POIs

```dataview
table description as "Description" from "Places/POIs"
where type = "poi" and contains(location, "Evermoors")
sort file.name ASC
```

## Shops
```dataview
table proprietor as "Proprietor", shop_type as "Description" from "Places/Shops"
where type = "shop" and contains(location, "Evermoors")
sort file.name ASC
```

## People / Characters
```dataview
table description as "Description" from "Characters"
where type = "npc" and contains(location, "Evermoors")
sort file.name ASC
```

## Other Tidbits & Misc Info

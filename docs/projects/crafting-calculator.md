---
permalink: /projects/crafting-calculator
title: crafting-calculator
---

# [{{ page.title }}]({{ site.github.owner_url }}/{{ page.title }})

I created this project to improve my experience playing Minecraft modpacks where crafting recipes
can be many layers deep.
At present, support for non-consumed catalysts is missing, so an item that is required for a recipe
but not consumed will not be accounted for in the "Raw materials" and "In storage" lists.

![An example craft]({{ site.github.owner_url }}/{{ page.title }}/raw/release/images/partially_crafted.png "An example craft")

The calculator produces its output by the following procedure:
1. Step down through the crafting tree to determine the minimum amount of each item necessary to
   craft the target.
1. Build the list of items which cannot be crafted and the list of items which are already in
   storage and thus do not *need* to be crafted.
1. Step back up the crafting tree from the raw materials and items in storage to build up the
   sequence of crafting steps which can be performed using only the raw materials, items from
   storage, and the results of previous crafting steps.

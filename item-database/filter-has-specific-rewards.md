---
title: Has Specific Rewards Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 32
---

# Has Specific Rewards Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>32</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>No</td></tr>
<tr><td>Affects Result Columns?</td><td>Yes. The item's rewards are shown under the item name.</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>uint</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>See Below</td></tr>
</table>

Filters items based on whether or not they reward any of the provided list of items.

For example, if you wanted to find all items that were capable of rewarding Baryon Boughs, this filter allows you to do that: 

[https://www.light.gg/db/all?f=32(592227263)](https://www.light.gg/db/all?f=32(592227263))

This filter essentially allows you to search for items that have any of the items you provide in their "Reward From" tab on their item detail pages. 

The Bungie API assigns a unique number to every item called a "hash". You may notice this number in item page URLs such as 

https://www.light.gg/db/items/**2429822977**/austringer/

Item Detail pages show the item hash as "API ID" in the Details section on the right.

This filter is not visible in the UI.


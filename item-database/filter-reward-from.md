---
title: Reward From Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 34
---

# Reward From Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>34</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>No</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>uint</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>See Below</td></tr>
</table>

Filters items based on whether or not they drop as a reward from any of the items you provide.

For example, if you wanted to find all items that a specific Purification Ritual bounty rewards, this filter allows you to do that.

This filter essentially allows you to search for items that appear in the "Reward From" tab of any of the items you provide's item detail pages. 

The Bungie API assigns a unique number to every item called a "hash". You may notice this number in item page URLs such as 

https://www.light.gg/db/items/**2429822977**/austringer/

Item Detail pages show the item hash as "API ID" in the Details section on the right.

This filter is not visible in the UI.


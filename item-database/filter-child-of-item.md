---
title: Is Child Of Item Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 27
---

# Is Child Of Item Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>27</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>No</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>uint</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>See Below</td></tr>
</table>

Filters items based on whether or not they are a child of the provided list of items.

For example, if you wanted to find all items that were capable of dropping from the Exotic Engram with the hash 3875551374, this filter would allow you to do that.

This filter essentially allows you to search for items that can be found in the "Contained In" tab of any of the items you provide's item detail pages. 

The Bungie API assigns a unique number to every item called a "hash". You may notice this number in item page URLs such as 

https://www.light.gg/db/items/**2429822977**/austringer/

If this filter is present, only items whose item hash are one of those provided will be returned.

Item Detail pages show the item hash as "API ID" in the Details section on the right.

If this filter is present, only items which are children of one of the item hashes provided will be returned.

This filter is not visible in the UI.


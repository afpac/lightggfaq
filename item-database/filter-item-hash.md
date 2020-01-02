---
title: Item Hash Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 11
---

# Item Hash Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>11</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>Yes, see below</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>uint</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
</table>

Filters items based on their item hash.

The Bungie API assigns a unique number to every item called a "hash". You may notice this number in item page URLs such as 

https://www.light.gg/db/items/**2429822977**/austringer/

If this filter is present, only items whose item hash are one of those provided will be returned.

Item Detail pages show the item hash as "API ID" in the Details section on the right.

This filter is visible in the UI as the "Item API IDs" box under Advanced.


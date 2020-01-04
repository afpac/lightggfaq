---
title: Stack Unique Label Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 40
---

# Stack Unique Label Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>40</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>No</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>string</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>Any string (50 chars)</td></tr>
</table>

Filters items based on their associated item's stack unique label. This is a field found on some items in their raw manifest data. You can most commonly find this on bounties. Check for the inventory.stackUniqueLabel property under the item's Manifest tab. 

Not all items have this property, and it doesn't appear to be used consistently even where it does exist. This filter was made to see if building stuff around this property was wise, and I decided not to. But, might as well leave the filter in case someone finds a use for it later.

This filter is not visible in the UI.
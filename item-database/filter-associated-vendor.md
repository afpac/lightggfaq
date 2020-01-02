---
title: Associated With Vendor Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 19
---

# Associated With Vendor Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>19</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>Yes, see below</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>uint</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>See Below</td></tr>
</table>

Filters items based on whether or not they are associated with a given vendor.

The Bungie API assigns a unique number to every vendor called a "hash". You may notice this number in vendor page URLs such as 

https://www.light.gg/db/vendors/**1616085565**/eris-morn/

If this filter is present, only items which are associated with one of the vendor hashes provided will be returned.

This filter is visible in the UI as the "Associated Vendor" box under Advanced.


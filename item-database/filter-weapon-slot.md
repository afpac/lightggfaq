---
title: Weapon Slot Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 8
---

# Weapon Slot Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>8</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>Yes, see below</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>int</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>0-2</td></tr>
</table>

Filters items based on the weapon slot they occupy.

If this filter is present, only items that are weapons and can be equipped in one of the given slots will be returned.

|Parameter Value|Slot|
|---|---|
|0|Kinetic|
|1|Energy|
|2|Power|

This filter is present in the UI as the weapon slot options under the Slot listbox.

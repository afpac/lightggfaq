---
title: Armor Slot Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 7
---

# Armor Slot Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>7</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>Yes, see below</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>int</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>0-4</td></tr>
</table>

Filters items based on the armor slot they occupy.

If this filter is present, only items that are armor and can be equipped in one of the given slots will be returned.

|Parameter Value|Slot|
|---|---|
|0|Helmet|
|1|Gloves|
|2|Chest|
|3|Legs|
|4|Class Item|

This filter is visible in the UI as the armor slot options in the Slot listbox.
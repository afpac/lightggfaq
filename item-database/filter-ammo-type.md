---
title: Ammo Type Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 30
---

# Ammo Type Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>30</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>Yes, see below</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>enum</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
</table>

Filters items based on their ammo type.

With the advent of Forsaken, we can't assume what type of ammo a weapon uses based purely on the slot it occupies, hence the need for this filter!

If this filter is present, only items that have one of the ammo types provided will be returned.

See [Destiny.DestinyAmmunitionType](https://bungie-net.github.io/multi/schema_Destiny-DestinyAmmunitionType.html#schema_Destiny-DestinyAmmunitionType) for allowed parameter values.

This filter is visible in the UI as the Ammo Type listbox under Advanced.


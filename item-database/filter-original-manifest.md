---
title: Original ManifestID Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 13
---

# Original ManifestID Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>13</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>Yes, see below</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>int</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>See Below</td></tr>
</table>

Filters items based on when they were first detected in the API.

Each API update is assigned a light.gg Manifest ID. You can see these IDs by going to the [API Update Tracker](https://light.gg/db/changes/).

This filter returns items who were first detected in any of the provided manifest IDs. 

This filter is visible in the UI under Advanced as "Added to API On".


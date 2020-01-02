---
title: Collectible Source Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 17
---

# Collectible Source Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>17</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>Yes, see below</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>string</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>Any string (50 chars)</td></tr>
</table>

Filters items based on their associated collectible's source description.

With the addition of Collections with Forsaken, each item has a related collectible which tracks whether you have ever collected the item. These collectibles have a "hint" as to what you need to do to collect that item. Sometimes they're useful, sometimes they're not.

This filter searches that source description to see if it contains any of the provided terms (case insensitive).

This filter is visible in the UI as "Collectible Source Hint Contains" under Advanced.
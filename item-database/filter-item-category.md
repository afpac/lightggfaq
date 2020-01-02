---
title: Item Category Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 9
---

# Item Category Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>9</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>No</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>int</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>See below</td></tr>
</table>

Filters items based on their item category.

In the API, items are associated with multiple item categories. Some are useful, some are not. 

Regardless, if this filter is present, only items that fall into one of the given item categories will be returned.

Visit [data.destinysets.com](https://data.destinysets.com) and search for `ItemCategory` to view valid parameter values (send the `hash` property).

This filter manifests in the UI in various lists/direct URLs, but it does not have a UI component to directly manipulate it.

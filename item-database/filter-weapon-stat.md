---
title: Weapon Stat Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 29
---

# Weapon Stat Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>29</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>Yes</td></tr>
<tr><td>Affects Result Columns?</td><td>Yes. Rating replaced w/ stat values</td></tr>
</table>

**Parameters**

Operation
<table>
<tr><td>Data Type</td><td>enum</td></tr>
<tr><td>Allow List?</td><td>No</td></tr>
<tr><td>Allowed Values</td><td>0 = Equal<br/>1 = Less Than<br/>2 = Greater Than<br/>3 = Less Than or Equal<br/>4 = Greater Than or Equal<br/>5 = Not Equal</td></tr>
</table>

Stat Value
<table>
<tr><td>Data Type</td><td>int</td></tr>
<tr><td>Allow List?</td><td>No</td></tr>
</table>

Selected Stat
<table>
<tr><td>Data Type</td><td>uint</td></tr>
<tr><td>Allow List?</td><td>No</td></tr>
<tr><td>Allowed Values</td><td>See Below</td></tr>
</table>

This is filter is another complicated one and has some syntax of its own beyond what's described in the [Raw Filter Syntax](./search-filters.html#raw-filter-syntax) documentation.

As you'll note above, there are multiple parameters for this filter, where most others just have one parameter (that can occasionally accept a list of values).

For this filter, it wants to know three things

1. What stat do you want to filter by?
2. What comparision do you want to do (such as impact **greater than** 60)?
3. What stat threshold do you want to set, such as 60?

Given the example question of "what weapons have more than 60 impact?", the query for that search looks like this:

`29:4:60(4043523819)`

Let's break down the components of the query:

* 29 indicates to use this filter
* 4 indicates that I want to do a `>=` greater than or equal comparison (answering question 2 above)
* 60 indicates that 60 is the threshold I want to set (answering question 3 above)
* 4043523819 indicates that Impact is the stat that I want to search for.

As far as the logic of the filter itself goes, it will return any item whose default API stats have a value for the given stat that matches the operation/value conditions you provide.

As with the God Roll Finder filter, it's probably wiser to just use the UI (Equipment stats under Advanced) to start your search for this and then customize from there.



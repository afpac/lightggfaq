---
title: Require All Perks At Once Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 28
---

# Require All Perks At Once Filter

**Attributes**

<table>
<tr><td>Filter Number</td><td>28</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>Yes</td></tr>
</table>

**Parameters**

Roll Exclusion Mode
<table>
<tr><td>Data Type</td><td>enum</td></tr>
<tr><td>Allow List?</td><td>No</td></tr>
<tr><td>Allowed Values</td><td>0 = All Rolls<br/>1 = Curated Only<br/>2 = Random Only</td></tr>
</table>

Selected Perks
<table>
<tr><td>Data Type</td><td>array of uints</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>See Below</td></tr>
</table>

This is the filter that powers the God Roll Finder. It's a complicated beast and has some syntax of its own beyond what's described in the [Raw Filter Syntax](./search-filters.html#raw-filter-syntax) documentation.

As you'll note above, there are multiple parameters for this filter, where most others just have one parameter (that can occasionally accept a list of values).

For this filter, it wants to know two things

1. What types of rolls are you interested in?
2. What perks do you want to look for, and in what grouping?

Let's take a sample God Roll Finder search to illustrate how the syntax works. Suppose I want to find all weapons that can roll with Arrowhead Break or Chambered Compensator as well as Combat Grip or Heavy Grip. The query for that search looks like this:

`28:0(839105230!3661387068;3438534621!1012699414)`

Let's break down the components of the query:

* 28 indicates to use this filter
* 0 indicates that I don't care whether the roll is curated or random. 
	* This answers the "What types of rolls are you interested in?" question above
	* If you do care what type of roll, see the allowed values for "Roll Exclusion Mode" above.
* Within the parentheses there are two lists of perks (separated by a `;` semicolon). 
	* These lists specify the different "groups" of perks I'm willing to accept
* Within each of those lists are the list of perks I've assigned to each group, separated by an `!` 
exclamation point.	
* The list of lists within the parenthese answers the "What perks do you want to look for, and in what grouping?" question above.


As far as the logic of the filter itself goes, it essentially finds all items with a roll of the given type that have at least one perk from each of the groups provided. So if you just want to find all items that can roll with Outlaw or Kill Clip or Rampage, you can send just one group (separated by `;` semicolons). However, if you want to force certain perks to be present with other perks (as in the example above), you will need to create multiple groups of perks separated by an `!` exclamation point.

All of this being said, it's probably a better idea to just craft your search using the God Roll Finder UI, click 'Filter this List', and then customize it from there. 


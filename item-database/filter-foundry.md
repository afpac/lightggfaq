---
title: Foundry Filter
parent: Search Filters
grand_parent: Item Database
has_children: false
nav_order: 15
---

# Foundry Filter

***Deprecated***

**Attributes**

<table>
<tr><td>Filter Number</td><td>15</td></tr>
<tr><td>Allow Negation?</td><td>Yes</td></tr>
<tr><td>Visible in UI?</td><td>Yes, see below</td></tr>
</table>

**Parameters**

<table>
<tr><td>Data Type</td><td>enum</td></tr>
<tr><td>Allow List?</td><td>Yes</td></tr>
<tr><td>Allowed Values</td><td>See Below</td></tr>
</table>

Filters items based on their "foundry". 

This is visible in the in-game UI by the background image in the upper left. 

There are more foundries in the game than those that are supported by this filter (such as Tex Mechanica), so don't treat -15(0) as "all weapons associated w/ a foundry" when it's really "all non-Suros/Omolon/Hakke/Veist weapons". 

The filter was originally created to help support a collection manager leaderboard in which you "championed" a given foundry and killed a bunch of stuff with their weapons. Since that leaderboard has been retired, this filter hasn't gotten much love and likely won't for the foreseeable future.

This filter is visible in the UI under Advanced as "Weapon Foundry".

|Parameter Value|Foundry|
|---|---|
|0|None|
|1|SUROS|
|2|Omolon|
|3|Hakke|
|4|VEIST|
---
title: Armor Inspector
parent: Inspectors
grand_parent: Loadout Calculator
has_children: false
nav_order: 4
---

# Loadout Calculator

## Armor Inspector

The armor inspector allows you to specify which mods and perks you want to use for a given weapon. 

Summon the Armor Inspector by clicking any of the armor slots on the right column of the loadout summary. From there:

### Energy

* When added, all armor defaults to Arc at energy level 9
* You can change the element/energy level of your armor at any time
	* Should you have any mods that no longer match the new element, they will be removed
	* Similarly, if you lower the energy level, mods will be removed until they fall within your new level.
* Raising the energy level to 10 masterworks the armor piece, granting +2 to all stats (see below on how this is reflected in the UI).


### Modifications

* Clicking an Empty Mod Socket icon will summon a list of mods that are compatible with your current armor element and energy level.
	* The energy cost for each mod is shown in the lower right corner of its icon.
	* Mods from the current season's artifact will only display in the list if you have them selected in the [artifact inspector](./artifact-inspector.html).
		* If an artifact mod is removed from your artifact, it will also be removed from any armor currently using it.
	* Should your chosen mod grant stats to your armor (such as Powerful Friends increasing mobility by 20), the Stats list below will update to reflect the mod's effects.

### Stats

The Stats list shows the current values of the armor's stats given your Mod/Masterwork. 

With the advent of Armor 2.0, armor stat values are (generally) randomly generated. The manner in which the game generates them, however, does not appear to just be random(2,42). The UI attempts to reflect the current theory of how the system generates these stats. The short version of how it works goes like this:

When a piece of armor drops, to generate its stats:

* Stats are grouped into Mobility/Resilience/Recovery and Discipline/Intellect/Strength
* Each stat has a base value of 2
* Masterworking the armor grants 2 to each stat
* Each of stat group receives 4 stat "blocks"
	* These blocks are assigned randomly to the 3 stats in the group
	* Each block has a base value of 4
	* Each block is granted 1-3 bonus points, giving them a maximum value of 7.
* Each stat has a hard maximum value of 42

The UI attempts to take stat values (either Imported from your current characters or randomly generated using the Randomize button) and apply this logic to it. 

To the right of each stat is the breakdown of each of the sources that lead to the final value for that stat. Hovering over any of the squares will tell you what the value for that source is and a description of where it comes from.

Possible sources:

1. Base Value - All stats have a base value of 2
2. Masterwork - If the energy level of the armor is 10, all stats get +2
3. Random Stat Blocks - As described above, these are how stats are randomly generated
4. Mods - Should your selected mods affect the stats of the armor, that value will be shown also (orange if positive, red if negative)

To the right of the source breakdown are plus/minus (+/-) icons. Clicking them will manually change the stat's value beyond what it was when the armor was generated.

### Roll Quality

Using the algorithm above, we are able to determine whether or not a roll is "good" by calculating how many of the opportunities for the stats to roll higher were met. Each piece will have between 0 and 24 missed bonuses. Roll Quality is determined by the number of missed bonuses:

| Grade | + |   | - |
|:-:|:-:|:-:|:-:|
| S | 0 | 1/2 | 3 |
| A | 4  | 5/6  | 7  |
| B | 8  | 9/10  |  11 |
| C | 12 | 13/14 | 15 |
| D | 16 | 17/18 | 19 |
| F | 20 | 21/22 | 23/24 |

In the stat source breakdown, missed squares show on the end of each stat row to indicate when the piece was capable of rolling higher and didn't. High quality rolls will have very few of these; low quality rolls will have many. You can use the manual change +/- icons to play with the values.

### FAQs

**Q: Why do you start armor pieces at 9 energy?**

This was done so that you can clearly see the benefit granted by masterworking when you raise the energy level to 10 (the 12 additional stats).

**Q: Why did you make it so stats can be manually adjusted? Won't everyone just always max them out?**

The ability to adjust manually exists so that we are able to theorycraft builds at the far ends of the RNG spectrum without having to mash Randomize or wait for the items to actually drop in game. The whole point of this tool is to be able to play around with scenarios without having to wait for them/pay for them in game, and being able to adjust the stats to accommodate for that is key. Being able to look at Super/Grenade/Melee cooldown breakpoints and build your mods/perks/class abilities around that is one of the big goals here.
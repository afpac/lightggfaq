---
title: Weapon Inspector
parent: Inspectors
grand_parent: Loadout Calculator
has_children: true
nav_order: 2
---

# Loadout Calculator

## Weapon Inspector

The subclass inspector allows you to specify which mods and perks you want to use for a given weapon. 

Summon the Weapon Inspector by clicking any of the weapon slots on the left column of the loadout summary. From there:

**Modifications**

* Clicking the Empty Mod Socket icon will summon a list of mods that are compatible with the weapon
	* Mods from the current season's artifact will only display in the list if you have them selected in the [artifact inspector](./artifact-inspector.html).
		* If an artifact mod is removed from your artifact, it will also be removed from any weapons currently using it.
	* Should your chosen mod grant stats to your weapon (such as Backup Mag increasing the magazine size), the Stats list below will update to reflect the mod's effects.
* The masterworks the weapon is capable of rolling are listed. 
	* Selecting a masterwork will grant +10 (see the FAQs section below on how stats are calculated) to that stat. The Stats list below will update to reflect this.
* You can deselect any node to indicate your loadout is flexible for that component of the build.

**Stats**

The Stats list shows the current values of the weapon's stats given your Mod/Masterwork/Perk selections. If a stat value is higher than its base value, the value and the bar indicating this change will be green. Similarly, if the value is lower than its base value, they will be red instead.

**Perks**

The Perks list allows you to select which perks you want on the weapon for your loadout.

* You can modify which perk list you want to see by selecting a different option from the Roll Type dropdown list:
	* *Random*: The list of available perks for the random roll of the weapon
	* *Curated*: The available perks that always drop on the Bungie "curated" roll of the weapon
	* *My Roll*: If the weapon was Imported from one of your current characters, this option will show you just the perks that are on your specific roll.
* Changing the roll type will clear any existing selections
* Select perks by clicking on them. Selected perks will have a gold border
* Community recommendations are shown as a glow behind perks. 
	* Blue = PVE 
	* Red = PVP
	* Gold = Either
* Should a perk affect the weapon's stats (such as Extended Mag), the Stats list will be updated appropriately 


### FAQs

**Q: Why do perks/mods say they give +10 to a stat but the actual number on the stat is different?**

The way that the Bungie API communicates stats is convoluted. Essentially it gives a value for a stat along with a formula to translate that value into what should be displayed. 

Mods/perks show the value that should be fed through the formula to get a new display value when they are selected. Once you select them, the inspector does the math and updates the Stats list with the correct display value. 


**Q: What are recommended perks?**

These are perks compiled by top community theorycrafters to be the perks to look for on each given weapon.

**Q: Why are some perks recommended on some weapons but not on others?**

Each weapon has its own recommendations independent of whether the perk is preferred on any other weapon.

**Q: What do the different colors mean?**

The colors denote which type of activity the perk is recommended for: 

* Blue = PVE
* Red = PVP
* Gold = Either

**Q: Who are these "top theorycrafters"?**

Perk suggestions come from [u/Mercules904](https://reddit.com/u/Mercules904), [u/pandapaxxy](https://reddit.com/u/pandapaxxy), and [u/HavocsCall](https://reddit.com/u/HavocsCall), with contributions from [@chrisfried](https://twitter.com/chrisfried), and [@sundevour](https://twitter.com/sundevour).

Thanks to [@48klocs](https://twitter.com/48klocs) for compiling all of the different recommendations into a single, easy to parse place. Check out his github project <a href="https://github.com/48klocs/dim-wish-list-sources/" target="_blank">here</a> for all the source files that power these recommendations.

**Q: I don't agree with some of these suggestions, and I'm really mad about it!**

Coming up with a complete consensus on what perks are best is a losing battle. However, these community members are widely respected for their work and contributions on trying to guide people as to what rolls are worth chasing. If you strongly disagree with anything they're suggesting, we recommend reaching out to them on the avenues linked above to better understand their logic or potentially change their mind. 

Overall, the suggestions here are just that, suggestions, and they are meant to give a little guidance to players who may be overwhelmed trying to determine whether the items they have are worth using/keeping. If you're a veteran player, these likely aren't for you, so try not to get too up in arms should you find suggestions you disagree with.
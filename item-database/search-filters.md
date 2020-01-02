---
title: Search Filters
parent: Item Database
has_children: true
nav_order: 2
---

# Search Filters

## Overview

The light.gg Item Database provides upwards of 40 different filters to help dig into Destiny 2 item data. 

The database allows combining these filters as well as selecting multiple options within them (in most cases). 

If you're interested in the raw filter syntax and how to compose queries directly, keep reading. Otherwise, [jump to the list below](#filter-list) to see all available filters and what they do.

## Raw Filter Syntax

If you pay attention to the URL as you're using the item database, you'll notice most URLs look something like:

`https://light.gg/db/all/?f=[something]`

Where [something] is a bunch of numbers separated by commas, semicolons, etc. This parameter is responsible for explaining to the database exactly what you're looking for. 

Let's build a query to explore the syntax.

Generally speaking, each filter has a number assigned to it. For example, filter #2 is the "[Is Weapon](./filter-is-weapon.html)" filter -- it returns only items that are weapons. So, the URL to return all weapons would be:

`https://light.gg/db/all?f=2` [Link](https://light.gg/db/all?f=2)

Simple enough, right? Let's say, however, you're really interested in rare quality weapons. Let's add another filter - #4, the [Rarity](./filter-rarity.html) filter:

`https://light.gg/db/all?f=2,4(4)` [Link](https://light.gg/db/all?f=2,4(4))

Here you can see that we're stringing the filters together by putting a comma between them. This functions as an AND operator - all filters separated by commas must be true in order for an item to appear in the result.

From there, let's assume that you realize rares are mostly just useful for the glimmer they provide, so you decide you want to see legendaries as well:

`https://light.gg/db/all?f=2,4(4;5)` [Link](https://light.gg/db/all?f=2,4(4;5))

This illustrates how some filters are able to accept a list of parameters. Those that are able to do so by sending a semicolon separated list (the 4;5 part in the query above). This component functions as an OR operator - the filter will return true if ANY of the options sent match. So in this example, we are essentially saying "show me all items that are weapons AND the rarity is Rare OR Legendary.

Now, let's say you decide you want to get some armor in the mix:

`https://light.gg/db/all?f=2|3,4(4;5)` [Link](https://light.gg/db/all?f=2%7C3,4(4;5))

Here you can see that we have added another chunk of syntax, the pipe `|` between the 2 and 3. This is the OR operator for filters. We're now saying "show me all items that are weapons OR are armor AND are Rare or Legendary. When using the OR operator, it's important to know that the AND `,` operator takes precedence, meaning that it happens first. If, for example, we were to do this instead:

`https://light.gg/db/all?f=2,4(4;5)|3` [Link](https://light.gg/db/all?f=2,4(4;5)|3)

We would get a much different result than we expect. This is because the AND operator happens before the OR operator, changing our question to "show me all items that are weapons AND are Rare or Legendary OR are armor". This query wouldn't return any armor since an item cannot be both armor and a weapon.

Finally, the other operator available to us is the `-` negation operator.  Going back to our weapons only example, let's say we now want to see all weapons that are not legendary or rare. To accomplish that, we would instead do:

`https://light.gg/db/all?f=2,-4(4;5)` [Link](https://light.gg/db/all?f=2,-4(4;5))

Hopefully these examples shed some light on how the raw filter syntax works. Each of the filters below will describe what its filter number is, whether it supports lists/negation, and what parameters it expects. With this knowledge of the syntax, you should be able to look at each filter and compose whatever query you're interested in running. 

As always, reach out to us on Discord if you get stuck.

## Filter List

Check the table of contents below for the most up to date details on all of the available search filters.
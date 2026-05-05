+++
title = "Arcanum Data"
date = "2024-07-31"
id = "bmz6XSd7xGM"
status = "transcript"
tags = ["Arcanum", "Production"]
summary = "I talk about the sheer amount of data in Arcanum. TLDW: it's a lot."
references = ["z-onK2K2_k0", "ETVsAHbTh2c", "GYWEgQAh6So", "5l7YcGCQ5Ck"]
+++

Hi everyone. It's me, Tim. Today I want to talk about Arcanum data.

So the last few weeks — well, since I've I I posted this almost a year ago, I think — since I converted Arcanum to be a Windows, a modern Windows app, it's way easier to debug it I can put break points anywhere. I can run the game in a window, you know, hit the break points wherever I want, look at what is going on, because you know it's been 25 years more since code started on that game. I don't remember how everything works and I didn't write everything. There were three other programmers, so I've been going through it for various reasons, and one of them I was doing recently was I was trying to see how the data flow was handled, basically what was loaded when in the game. And first of all, let me just say there is a lot of data in this game. I look at it and I have to remind myself that the entire game was made by essentially 14 people. Yes, there's a lot more people in the credits, but you know I'm not counting people who did localization and production and you know, uh made the boxes and handled advertisements and things like that. I'm just talking about the actual development team. It was 14 people.

There's a lot of data, so I thought I'd go over it. This is going to be kind of technical, not as much. I basically I'm not sure who'd be interested in this. I'm tempted not to say it's technical, because I'm not going to go into the details.

What I would did is I: I found a lot of data being loaded. So what I did is I got a count of it by what type of data it was, and then I arranged that data into four categories: art, General, game data, sound and text. And I'm doing the text last for a. Reason which I'll get to. Um, I also want to tell you that the totals I'm giving you here for how much data was each one of those types in each one of those categories? Some of that's going to include some unused data.

Frequently, like element zero was used for a placeholder, or if something didn't like, if something didn't use a sound, then zero was the sound we use. It didn't correspond to any data file. It meant it doesn't make it sound in this category.

Um, however, it's all loaded by the base game and that's what's important is this: is all the data being loaded, so let's start. I'll start with art. This is roughly in order. It got loaded, but I moved some around because some just at the end I want to like whoa.

There are 846 unique pieces of interface art because — that's like Corners to make. Window and edges to make Windows background thing, anything, that appears in an interface as part of the window and not the data being displayed.

There are 846 of those, there are 40 unique NPC art like body. That means for race, gender and what they're supposed to be wearing, not players. There were far more for players, um, but just like how many. How many unique NPCs could you see in the game?

40. How many unique monsters were there? 32 in my head there were a lot more than that, but 32. How many different containers? Containers or anything that can have an inventory — that's not a living thing — chests, bookcases, anything like that? 73.

How many different light shapes are there? We handled our light by projecting a shape onto the tiles and then changing their color to reflect the light hitting it. There were 32 different light shapes. How many? Different tiles did we have?

88. How many different roofs did we have 16? How many different walls did we have? We had 43 different wall segments, but that includes corners and wall pieces that had, like the left side of a window, the middle of a window and the right side of a window, or the same thing in the left and right side of a door. If you actually break it down into different types of walls, there were only seven, but those were made up of 43 different art pieces. How many different portals do we have? Portals were doors, Port Colores, anything.

You would click on it and it would. It would block pathing until you clicked on it and it changed its state 373. That surprised me. I don't remember that many, but then I remember we did make like a door and then color it different ways and we saved them all off separately.

Scenery — scenery is anything that you just see in the world that may or may not block you, may or may not block site, may or may not block cover, but wasn't a wall or a container or a creature. We had 1,434 pieces of scenery, then items were broken up into how they looked on the ground, how they looked in your inventory and how they looked on the paper doll. There were 709 unique item ground art pieces, 712 unique it item inventory pieces and 415 paper doll art pieces. The reason the paper doll one is lower is not everything that could be in your inventory could show up in your paper doll.

Then there were 339 items that appeared as in the item schematic, either as what got made or the components that you put in There were 373 pieces of facade. Arts, now, we didn't have 373 facades, but they were made up of sub pieces. Facades were any large thing that it was too big for us to make a structure or wall or piece of scenery and you weren't allowed to walk on it. Like the crashed blimp was a facade. Um, one of the castle entrances in the game was a facade. It was basically a bunch of tiles that were marked. You're not allowed to walk on them and they were made up of lots of little tiles.

There were 373 of those, there were 78 unique portraits. There were 625 effects that could occur because of items. You know particle effects related to items usually hits swipes. You know explosions, there were Nine Movies in the game, nine cinematics. There were 56 end slides and each one connected to a piece of art and a sound effect. And then there, were 456 what were called I candy pieces of art. I candy was anything that didn't fit in the previous category, that was just put into the world as something to see, something to dress it up, but wasn't scenery, wasn't AN particle, an item effect, wasn't a facade. That was called eye candle, eye candy, and there was 456 of those.

Now, keep in mind that whole game was made with what? Five or six artists — pretty impressive. Now look at game data, there were 25 unique story States. I think that was too many. Um Fallout had three. Arcan met 25? I think the answer is somewhere in between.

There were 81 unique Maps, there were 163 quests. Now, since we had one, I think, sto main story quest for each story state, that means that the vast majority of those 163 quests were side quests. There were 54 blessings and 52 curses, which I was surprised was almost balanced. Blessing and curses were anything you that happened in the game where you did something that it was almost like divinely or supernaturally imposed on you. In effect, there were 502 spells, there were 58 level schemes, which is different ways that your character could be automatically leveled up if you didn't want to handle leveling up yourself.

There were 56 different factions that we had to keep track of. There were 36 skills, there were 123 inventory sources, and that was shops would have an inventory Source, meaning it was a, list of items that this is what this shop sold. And if you bought things from them, after a few days, when they wanted to refresh their inventory, what did they refresh it? From an inventory Source list, and there were 123 of those. Like the example, the first one was called rural, General Store and there were 69 unique keys in the game. So yay, that included, I think, a skeleton key that could open any lock.

Sound sounds are much smaller, there were 460 Critter sounds, a sound an NPC, PC or Monster could make. There were 29 interface sounds, mostly buttons and slider controls. There were 106 item sounds. Those were sounds associated with an it, a particular item, like shooting a gun. There were 75 melee sounds and you're thinking: well, wait a minute, isn't that like sword?

Well, melee was separated out because first of all punch — you could punch people and there's no item associated with that. But also we had sounds for things like if a sword hit a particular kind of armor, so sword hitting metal armor versus sword hitting leather versus sword hitting just flesh. Those all had sounds that was put under melee sounds. There were 842 sounds associated with spells and there were 126 other sounds — miscellaneous.

That's things like. The first example on that list was a chest opening. So that's a lot of sounds and each one of those was hand connected to Something in the game. Now we get to the big list text. There was a lot of text in the game. There were 1,152 unique description strings and a lot of those got reused like it could be like sword or dagger, and then a bigger string might be a rusty dagger or a glowing sword. There were 25 combat Tech strings. These were strings that were used during combat, things like poison level or critical hit. There were 77 backgrounds in the game and the associated text with them that, like you know, whether you raised by elves or raised in a circus, there were 408 strings just used by the main menu and interfaces hanging off the main menu. Things like options and loading games and stuff like that. There were 330 strings used by in-game books and 24 used by in-game notes. The difference there was books had pages that you could turn where I think notes always got displayed on one page. There were 223 newspaper story strings, 34 telegrams — I forgot there were telegrams in this game. There were 35 plaes.

Plaques were mostly used for some puzzles that were in the game um. I think one of them was the, puzzle, the that happened up in um, the vendor grth Wast, the lost city up there spoiler. And then the last set of strings I saw loaded were the 204 quote lines in the quote file. Now something I'm not including lines of dialogue there were. If I remember correctly, there were about a half a million. I don't remember it I think I'm in the right ballpark there.

The reason I didn't list those? That would require opening every single dialogue file and hand counting the lines in them, because you have to count NPC lines, player lines. Um, some of those lines vary depending on the player's gender. Um, then you'd have to include generated dialogue, which is combinatoric. I mean, here's an example: you may have a node that says good morning, nice to meet you, and then the player could respond: can I see your stock or I have to go? That same one dialogue node could also be replaced with good evening, nice to see you again, and the player respond: what's for sale or good buy? That's one node, but it generated two very different looking combat or dialogue conversation notes. Even if there were 10 combinations for each of those three lines, that would be 10 by 10 by 10 or a thousand combinations, and a lot were more than that, so I didn't count that. What's the point of this?

Arcanum was a really big game. It was a big game and, keep in mind, they made by 14 people — big, game.

But it also explains why I can't answer a lot of their questions. Sometimes people ask me questions, very specific questions about: hey, what about this specific Quest or this piece of art or this map, and I can't answer your question because there was so much stuff in this game that there was stuff that went in that I never saw or that I did see but I don't remember or never took a note on. So I just kind of wanted to talk about this so you guys can just understand.

This is a 25-year old game, there's a lot of stuff in it and new games can have even more stuff in it, and are made by way bigger teams than 14 people. Anyway, that's a long video where I'm just talking about Arcanum data.

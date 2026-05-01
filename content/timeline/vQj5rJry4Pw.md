+++
title = "Developing South Park: The Stick Of Truth"
date = "2023-09-10"
id = "vQj5rJry4Pw"
status = "transcript"
tags = ["South Park: The Stick of Truth", "Storytime"]
summary = "Hi everyone. It's me, Tim. Today I want to talk about South Park, the Stick of Truth, also lavalier mic, so hopefully this sounds better."
references = []
+++

Hi everyone. It's me, Tim. Today I want to talk about South Park, the Stick of Truth, also lavalier mic, so hopefully this sounds better.

I haven't talked much about South Park or pillars of Eternity or tyranny, because I wasn't involved in any of those projects in a lead role, so my viewpoint is mainly as a programmer. I did some design, but mostly I was a programmer, so take these stories as from someone with that somewhat limited Viewpoint. When I talk about a lot of my other games, I was a lead, or even the Project Lead, so I had access to a lot of information of stuff that was going on — not true in South Park.

In fact, I came onto that project late in October of 2011.. The game was supposed to have shipped in six months and I was only coming on as a temporary employee. I was planning to move to Seattle when I was done.

For various reasons, that never happened and South Park itself wouldn't ship for. Almost three years later it shipped in — uh end of first quarter, I think, 2014.. So two and a half years later, I was replacing a programmer who's moving on to another project they had called stormlands, which ended up getting canceled. But I'll explain some things that happened along the timeline of South Park. So I started in October of 2011.. I was going to be a programmer.

The game itself, South Park, used code from obsidian's in-house engine, Onyx, that they used in Dungeon Siege 3.. This explained why many of the C plus methods began with Ds underscore. So I was quickly trying to come up to speed with that engine, which was in C plus, and South Park was going to be my first console game. I'd never made a console game before this, so I was kind of excited. Just for that reason turns out the Xbox pretty.

Easy to code for if you know, the PC, especially DirectX, calls PlayStation 3 not so much easy to code, for it had its own special cell architecture. It had multiple processors. My biggest issue with the PS3 was if you put a break point on your code it didn't always stop where you put the break point, because multiple processors will be running.

You'd see them go, stop, and maybe they stopped at the line you wanted. Maybe they stopped one line under one line later because the your the way your break point was. There was already an instruction that was given out to a CPU before it realized, oh, I've got to stop here. So it meant debugging was a little interesting. I learned how to do. It wasn't a huge fan, in fact.

Whenever a bug came in from QA, I checked and if it wasn't PS3 only, I always debugged. It on the PC or the Xbox. Sometimes one came in and said this is only happening on the PS3 and I'd be like, okay, let's, crank up that debugger and figure it out.

I was a huge South Park Fan — huge. I remember watching their Christmas special back during a Thursday night thing, which was one of those weekly things we did at interplay. I remember when that special came out we thought it was a one-off. It was Jesus fighting Santa Claus.

George Clooney was involved. I think he was the voice of the dog. It was funny. We thought it was a one-off, next thing we knew they had a show, so it was really fun to be working on it. You have to remember, though, there's a particular kind of humor in South Park. Not everybody likes it I think it's hilarious. I love how they make fun of everybody. No one escapes being ridiculed on that show.

Same thing with Simpsons. I like that style of humor. They, you know, they have a gay character, big gay owl. I think he's funny. Yeah, he's a stereotype, he's hilarious, so I believe a few people had issues and either they didn't work on the project or some of them just worked on the project but didn't do the more disturbing work. You have to remember, there were some things — and I'll talk about something I had to do, but there were some things where you had to, especially as an artist, frame by frame, like, draw people's private parts and their underwear and just gross things happening. You know, someone had to animate.

Uh, Mr Hanky, the, piece of poop. Um, I mean you just it's not like it happens like that. So this is. The person who spent every day staring into their monitor, you know, making a model or animating it, or putting a skeleton in and doing the animations and setting animation frames, and all that on a dancing piece of poop. That was the job.

Um, one thing I noticed was Matt and Trey seem to change their minds. A lot jokes would go in, system mechanics would go in, levels would go in, and then later they wouldn't like them. Um, they said: well, we, initially we liked it and now we don't think it's funny.

Well, that's the problem with video games is you're gonna play it multiple times. It's not like a show where, you do the storyboards, you animate it's up in a week and you're done. This thing takes years to make and you're gonna be seeing those jokes over and over again. So I think we lost.

A lot of funny stuff. Um, there were a ton of levels that we did completely finished, done, coded art, debugged, optimized. I mean I remember optimizing a level that got cut. It was sad because some of these were super fun and would have added a lot to the game. They added new factions, new areas of the town.

Um, one of the ones I remember the most, there was a cemetery with a bunch of goth kids and you went in it and you had a big fight with. I remember there I think there was a werewolf. I know Michael Jackson was involved, it was just. It was such a cool level and it all got cut. We had a whole thing called Christmas Town, which was North Pole or north of Canada — um, Canada itself, you know, done in the 8-Bit style. Was hilarious. Um, the one I worked on a lot.

There was a faction of all girls who loved Paris Hilton and their gang was called the stupid spoiled and at one point their leader, Paris Hilton, comes to school and you have to fight her and she's a boss and she had a special attack called the vag blast and — and I mean, I'm not an artist, I didn't animate this thing, but at one point there was a bug with it and I remember sitting with the artist going through it on my computer in debug mode, frame by frame, trying to figure out what happened, and things were spewing across the screen: there was a baby shark, there was a pineapple, and I was just like, hmm, yeah, let's. Oh, we finally found the bug. You know it got to be done with that. Um, there was an. Entire alternative advancement system that was made. That was eventually not approved but I thought it was great.

Um. Jesse Farrell had made it was called the ass system because all of the advancements were called like things like smart ass, kick ass, dumbass, I think one was called jackass, just a bunch of funny names like that, and they were all represented like: this is the you know, um, I think the uh spellcaster was smart ass and the fighter was like kick ass. So it made sense. It was fun. It was very South Park didn't get approved.

Another interesting thing is when I started, there was a producer on it and I'm not sure what happened. I didn't interact with him much and then he got replaced, um, and Chris Parker stepped in. Chris Parker was one of there were five owners at the time there. Only Chris Parker and Chris Avalon seemed actively involved in game development — um Fergus could do it anyway. I told you he did it on Fallout, but running a business is a lot of work. Chris Jones was handling all the tech director stuff and Darren Monahan was handling IT and basically operations. So they were busy.

Chris Parker was really good because — and I've told many people this — he's the kind of person who can step in and he will get that game across the finish line. There's a joke in game development that the first 80 of game development takes 80 of the time and then the last 20 of a game's development takes another eighty percent of your time. That's because it doesn't seem this way, but you always seem to get most of the game done, and that from that's when the unexpected problems happen. That's when it becomes obvious. That you misestimated how long things would take, that there are more bugs or optimizations that needs to be done, that couldn't be predicted, that lighting isn't working well or lighting caused levels to slow down, and now you need more optimization. There are always things like that. Parker seems really good at organizing this stuff, cutting through a bunch of bureaucratic tape and just getting stuff done, so that was really cool. Um. The other thing that happened was during the development of South Park.

Uh, Josh Sawyer and Adam bretnecke did the kickstarter for pillars and I thought it was cool. I was like this is really cool. Well, I started getting involved in that. They asked me to do some design stuff. I did some classes, I did the stronghold — um. These.

All these eventually got Modified by Josh, but it was fun to be involved. I, also um, at some point we were — I did some videos for it — we were doing stretch goals. Um, Josh wanted me to do my recipes from a lot of my previous games or just brand new recipes, and that eventually became a, stretch goal and something that kind of that you could get. I thought that was pretty cool, because it was nice having those recipes printed.

What that meant was: the kickstarter started in September of 2012 and ended a month later and, wow, you know, we got a lot of money and we had to start this thing. So I was still in South Park, so I tried to finish up my stuff there and then in 2013, I got moved over to pillars and I started doing a lot of code for that. The problem was South Park really couldn't stand, I mean, at the end of a game. Development artists can tend to move somewhere else, but programmers are needed, there are features that need to be done, optimization — so I got moved back onto South Park. It was funny because I — it was I'm — with pillars. And then when I was on South Park and pillars and I went back to South Park, finished it and I think literally the next day I came in and just instead of spinning up, uh, Microsoft Visual Studio to do work on South Park, I spun up Unity to do work on pillars. So pillars or a South Park, shipped in March of 2014..

I think it did really well. It was a fun game. It was super fun.

Um one. I actually designed something for the game that got cut. It was called. It was a different form of turn-based where you, when you, after you, moved, you didn't. Go back to your position, so you moved and you stayed wherever you ended your move at. So if you ran up to attack something and hit them and then you were out of action points, that's where you ended up. Some people you know, if you could take a step forward, hit them and then move away a little bit, it was fun because it meant the screen, the combat screen, got all jumbled up. We ended up not going with that, but it was super fun to work on it.

Like I said, there was so much system mechanics and actual content and art that got thrown away. That game just blew my mind, there could probably be an entirely second game shift with what got thrown away, but it was super fun to work on. I'm glad it did Super well. It was my first console game. Super happy, wasn't my? Last, but it was fun to work on consoles and it was fun to work on South Park and after carbine it was fun just to be a programmer again. So anyway, those are most of my stories about Stick of Truth and I'll try to put together eventually something on pillars and tyranny as well.

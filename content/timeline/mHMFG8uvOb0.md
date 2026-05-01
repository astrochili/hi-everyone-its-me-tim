+++
title = "Coding Toys (Insomnia Edition)"
date = "2023-05-19"
id = "mHMFG8uvOb0"
status = "transcript"
tags = ["Programming"]
summary = "Hi everyone. It's me, Tim."
references = []
+++

Hi everyone. It's me, Tim.

It's three in the morning and I can't sleep. This happens occasionally, so I try to do something productive. Tonight I think I'll show you some of the little toys that I make when I get bored now. I already showed you the space Raiders game that I made. It's a riff on atari's Star Raiders from the 70s.

I had a lot of fun making that. Put in models that I got off the unity store and had fun making ships, flying patterns and putting shields on ships and figuring out the best way of making a photon torpedo in unity. I know I got a lot of good feedback about the gurps character editor that I showed yesterday. That was really fun. That's also a toy. I made that on my own time.

Yes, it led into Fallout, so you never know where one of these toys is gonna lead. Let me show you some things I've been making, recently. I put together something in unity the other day. I wanted to put together a physics-based dice roller. So I just made a six-sided dice model, made them different colors, rolled them, played with, putting them together in groupings and displaying what dice rolled. So I knew that I was getting the dice rolling correctly and that was fun and I thought: what can I do with this? It's fun to do, it's fun to make. So I made a game called Dungeons and dices, where you pick a character class, give you one little special ability you can use. You roll the dice and you use them to attack monsters. These monsters do damage to you every round that you haven't killed them off.

The dice have to be arranged in a pattern similar to what you'd see in Yahtzee. You know, in this case I'm trying to kill a rat, full house. So I need. Three of one die and two of another color doesn't matter on this card.

Boom, I killed the rat. When you kill a rat you get some XP. You can see your level bar over there, you get a little Health back, but every round that you have to re-roll you take damage. It's not always a full house.

Let's see if I — oh I — used my Thief ability, which is, if I have all the slots filled but one, I can just go ahead and kill them. Ah. These defense cards are special in the sense that if you have more cards than one, you have to fill the defense one first. So this card has a plain bow on it, and what that means is that all of the dice have to be the same color. Now, I'm colorblind, but I can tell that these are different colors because I picked the colors. So I think these are tan. You just have to have all 10 dice you can see I'm taking a lot of damage. I think three points. Every time I don't kill this guy, perfect kill. I just went ahead and did my Thief kill. The other thing I made was a little different. I was trying to figure out if I could make a dungeon generator, and I did, and the way this works.

Oh, look, you can also go in. Once I find a dungeon, I, like you, can dive into it and run around. It's a fun little game. You might turn it into something. Not sure what I'm gonna do with this, but I'm gonna have to make creatures, character abilities and props in the dungeon.

I've already figured out how to put doors in, I just haven't bothered to do it yet. Like I said, these are just little toys real quick. If people want to know how I did that. I made random dungeons. My idea was just to take a flat surface like a sheet of paper. Think of it as graph paper. I dropped random rooms down, pick the location, made a random width and height of the room, just a random rectangle, plopped it down. If it intersected an existing room, I threw it away and just kept going, loot that 100 times until I had somewhere between 10 and 20 rooms. Then I treated that as nodes on a graph, added in all the edges and then I used a, an algorithm — I think it's called dijkstra's algorithm — to generate the minimum spanning tree between all those nodes that represented the minimum set of hallways that I would need to connect all those rooms. But that's kind of boring, so I added back some edges to make sure that.

Every room was still connected, but sometimes there were multiple ways to go through. Then I took that flat surface and then just generated a 3D map. Wherever there was a room, I put in floors. Where the room stopped, I put in walls, — walls that even worked well for the hallways, because they just represented flat floor surface connecting rooms, and the walls went up between them. It was fun to do. I think everybody should make toys like this, especially if you want to be a game developer.

It's great to get an idea out of your head and realized. You'd be surprised at what it makes you learn. The curbs editor, made me learn super VGA modes back in the 90s, which really informed what I did on the game. After that, these games I'm doing in unity just forced me to learn Unity UI and physics modeling — not friction, gravity, lighting — things I didn't normally know or didn't know before, because either in the games I made like pillars of Eternity or tyranny, I didn't have to do those things. So kind of kicks you out of your comfort zone.

It also makes you test your ideas and figure out if they're good or not. Sometimes I just have an idea. I just need to get it out of my head. This is something that I like to do. I find it very useful. Don't always do what I have insomnia, but I I find that if you constantly try to go beyond just having ideas and you try to realize them, not only will this increase your skill set, but it'll help you learn how to edit your own ideas, something that took me a long time to learn how to do. So if these are things that you like, um, I think you should grab something.

Unity game salad. There's a Unreal, of course, there are so many game engines out there that you owe it to yourself to pick up one, learn it and just try to hone your skills on it or, the very minimum, realize the ideas you want to do. In fact, at some point, I should probably do a video about how to get a job in the game industry, but don't know if that's today, but anyway, that's what I do around here at three in the morning. Hope you all have a good day.

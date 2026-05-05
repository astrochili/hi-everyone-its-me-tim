+++
title = "Toy Update, Part 5"
date = "2024-10-04"
id = "niZtYIiIxOw"
status = "transcript"
tags = ["Toy Update"]
summary = "OK, one last toy update, showing everything I have done with my space game to date."
references = ["YYSDWFfXzlg", "oCKPphehFGk", "wpbUuoyGPBM", "CA7gIg5b6_8", "mHMFG8uvOb0"]
+++

Hi everyone. It's me, Tim. Today I'm going to give you toy update part five.

Now, I know I said last week that was probably going to be the last update for a while. This one really is, because I'm going to explain everything I did and then show you several minutes of game footage so you can see how it all turned out. But I've already archived the code and the assets into a compressed file. I threw it up on the cloud and I'm not going to be working this for a while. I just I want to do other things and you know, like I've said many times, I'm not on a schedule, I'm not beholding anybody, so I work on this. When it's fun, it is fun.

I've really gotten into shaders and render Trail. Uh, yeah, Rend trails and, um, particle effects, which I've never really done much before. It was super fun.

It's giving me ideas for other things. So this is the last toy update for a while for my space game. Anyway, let me walk you through what I did. Um, the first thing I did was I took a lot of the ideas about shaders and I made a new Shader — Shield, uh uh, Shield Shader.

Here it is. You can see it's a lot more complex than the old one. What I've done is I've added a texture to them, uh, using a combination of a noise filter and UV time based scrolling, and that way it just is a much cooler looking effect.

It's. I still use color and the Fresno effect and all of that. That was just a cool thing to put on top of it. And then, when I was doing the photons, I decided the plain yellow ball wasn't good enough. I gave them a new Shader too, which had a very similar effect, but with no Fresno over it. But I also, in addition to wanting to give them a new Shader — so they looked like a cool ball of plasma going out — I decided that I would also give them a trail, and there's something in unity called a trail renderer. So I put in a trail which started the color of the photons, which I think is yellow — I'm trying to remember the RGB value I picked — and then it Trails off into white. The alpha reduces as well, well, the width gets smaller, so it looks like it has this thinner, fading whitening trail behind it when you shoot it I thought that was really cool and again, I'll show you all this when I do it.

Um, finally, I was playing around with the ships and I gave them a trail too, but I thought it looked wrong. It made them look — remember, this is an old retro game — and it looked a little too high-tech to have a. What looked? Like a little plasma trail behind it. So what I did was I went through the particle effect system and I ended up putting in a particle effect that looks like little puffs of smoke coming out behind them that puff out and fade over about I think it was 10 seconds. Um, and what's funny about it was it does make them look very archaic. It looks like a um, like they're.

The ships are running an internal combustion engine and it just it made laugh. It also made the ships easier to track, uh, visually, because when they flew by you, they leave this Trail and you could follow the trail to see where they were worked out — really great. I didn't increase the alpha because if you, if I, didn't do that, shooting them through the smoke was a little harder. So I made the smoke, uh, very translucent, but it was still.

Pretty fun, now I want to talk about all the features I put in on the players ship, because then it the on the players ship, because then it will make understanding how upgrading them worked. So I will show a screenshot of the game. So here's a screenshot. I will direct your attention to the bottom right corner. So those are the six major player systems.

The first one is the shields, which, for the player, doesn't show as a bubble around them, it shows as a tint to the view screen. The next one is the scanner, uh, which I was calling the long-range scanner, which is why it's an L, but you know now I have a separate UI for a long range scanner. That is the element that's over there on the bottom left. That basically is a radar screen that shows what's in front of you and behind you in 2D. Then there is a Tracker, well, that's the third one. That is the ability for you, to uh, do a middle click and track the, uh, the enemy ships, with a, with a bracket. It also later on, when you get tracking photons, which is an upgrade you can get — and I'll talk about upgrades — um, they work you through the tracking system. How good they work is based on the tracker.

There's the engines, which get more and more speed as you improve them, um, and lose speed as they get hurt. The B is for tractor beam, when you blow up another ship, it turns into cargo. The cargo floats out in space, if you go, if you fly over it, you pick it up, fills up the cargo meter that's there in the bottom, when it's full, you can upgrade. The tractor beam pulls them in faster and from a bigger radius when you improve it. And then, finally, the last one, H is Hull. That is, how much strength is remaining in your Hull. Now, all of these systems can take damage and have damaged state, so they visually appear a little different when they're damaged, or they sound different or the ship moves differently. And then they have a final broken, non-working State.

All of them can be upgraded with cargo and, as I said, when the car, when you pick up cargo, it fills up the bar. When the bar hits the top, it presents you with three systems that you have that still are upgradeable. So it picks a random three and says: you want to upgrade these. Once you hit the maximum upgrade, it stops offering that one.

Um, when you get hit with a photon torpedo by an enemy, the shields attempt to stop it. When the shields aren't full, they're guaranteed to stop it. When the shields are damaged, there's a chance it makes it through, and when the shields are completely broken, it always goes through. When the damage goes through, it's applied at random to one of the underlying systems that still is undamaged, uh, and it's just random. Now all of those systems can go to zero and you can still function. You can function without a shield, you can function without a tractor beam, you can even keep playing. If the engine's broken, you can't move, but you can keep playing.

However, when the hole hits zero, you die. Now there's a score up in the upper left, but when you die, it also tells you the highest wave of ships you reached and how many the total ships you killed were. Let me talk a bit about waves. The waves, um, it starts with one. Or two ships with no Shields and then there's more ships with every wave. Finally, at wave five, there's a lot of ships and also a Corvette. The Corvette is a big ship, it is shielded, it shoots multiple photons and it launches ships. So you really want to take care of the Corvette.

And then, after wave five, um, the ships, the small ships themselves, start getting upgraded. So it reverts back to just sending you small ships, but they have shields, they might be able to shoot multiple photons at once, and that those shield and everything get stronger in as the waves get higher. And then every fifth wave, there's a Corvette again.

So and again, and then — I mentioned this before — there's different Arenas that can be picked. There's a planet Arena, a star base Arena and an asteroid field Arena. Okay, so now that I've described all that, let me walk. You through a playthrough and I'm going to talk over it. So we're going to try to do this. So, okay, so this is star Traders. It picked the space station Arena. You can see the photons. You see my photons have the little trail behind them.

There's one of the ship. The ship has its little smoke trail behind it. I'm tracking it, now there are two enemy ships. I can shoot them no Shield, so what if you hit them, they get destroyed in one hit.

And there's a cargo container so you can zoom up on it. You can fly over to it, if I don't fly to it, if I just hit here, they'll eventually get pulled in Slowly by the tractor beam. It's much better to fly over them.

You can see the cargo meter at the bottom is filling up. Okay, wait two, there are three ships. You can see the bottom three down by this. So, again, they don't have shields, but there's more ships in this way, so I'm taking them out. With one hit each I can pick up cargo. So now I get three more cargo. So I'm going to probably get up to about half of my cargo bar filled just by the end of wave two, just because there were two and three ships in those last waves.

But it can. They can vary a little on waves. Wave Three is coming in. Uhoh, six ships. I think that's the most I'll see.

Um, again, they don't have shields, but there's a lot of ships and they're all coming in at me. They're all shooting and, like I said, it's easy to find them with the trail. I think the trail looks pretty cool, makes the game a little more retro. Um, some, very easy to.

Spot, especially when they're far off, so I'm going to get these. I think, if I can pick up all of these uh caros, that this will let me fill up my cargo bar and I can upgrade and demonstrate what the how the upgrade works. Oh, I just need one more, oh, and the other wave's coming in. Hopefully I can just pick up another one while I'm being shot at.

Um, I like that, there, photons also have Trails which make it easy to see the photons Direction, uh-oh. Oh, oh, my Shields are gone. Okay, as soon as I get an upgrade, everything's healed to full and I get to pick of these one of these three things. Uh, I picked the shields, so the shields are now can take more hits until they're fully destroyed. So keep playing. Oh, this one has seven. I guess I forgot what.

How many could be? In each wave, so this one has seven ships in the wave. This is wave four, so this is the last wave I'll get till Corvette shows up again. I think it's really cool to have Trails on the ship, the particle effect, smoke Trails — so I can see where they are when I'm looking around. I don't think I'm going to get enough cargo to upgrade before the Corvette shows up.

That's okay, although I really wish my shield could get repaired, because they've taken a lot of damage. One more ship. Sometimes I leave the other ship one. When there's one ship left, I leave it out there, so I have time to pick up all the cargo. Maybe, if I'm lucky, I can pick up enough cargo before the Corvette takes me out. We will see. Oh, my hole's taking damage too.

Let's find out what's going on there, that's all. I'm going pick up. Let me blow up The Last Ship, okay, so this is wave five. So there will be a Corvette. You will see It's big, it shows up big on the radar, it's big in the view and it will start the in the view and it will start launching ships. So you may see the ship number at the bottom.

Go up, there it is. There's the Corvette, lot of other ship. Oh my God, there's a total of nine, total of 10 ships out there.

I don't think I'm going to survive this. Oh, if my takes one more and it's got a big shield around it, yeah, I don't think I'm going to survive this. And the oh and oh, I don't know.

Oh, I overheated my photons. Oh, I'm so close. Come on, come on. Oh, oh, I got destroyed. Okay, I reached gr five and I encountered 30 ships.

Okay, so that's the toy as it stands. Now some of you may go: hey, that's a game. For my, standards, that is not a game. However, it's way closer to being a game than it was in the first toy update I did so. I hope that gives you a good idea of the arc that you can take when you're trying to turn just an set of ideas you have into a toy and then you're starting to turn it into a game. Anyway, probably not going to make another one of those for a while. My Arch all backed up, but I hope you enjoyed that and I'll go back to doing other fun Friday topics after this.

+++
title = "Toy Update, Part 2"
date = "2024-09-13"
id = "wpbUuoyGPBM"
status = "transcript"
tags = ["Toy Update"]
summary = "Hi everyone. It's me, Tim. Today I want to do part two of my toy update."
references = ["CA7gIg5b6_8"]
+++

Hi everyone. It's me, Tim. Today I want to do part two of my toy update.

I did a video a few weeks ago where I did an update on some of the toys I code, which are the little games that I'm just having fun with, and this was my space combat game and I talked about how I wanted to do a few things to make it better. Namely, I wanted to make new Photon torpedo types and I wanted to change how the shields looked on enemy ships. So I did that and I kind of want to give you an update because I want to show you that even with toys, you know, you can play with them and they get progression and you can make them better over time.

So let's talk about the photons first. The first Photon type I wanted to add was a viral Photon torpedo, and what that would do is when you'd strike an enemy ship, it would be taken over and start fighting for you. And I thought: well, this is going to be really easy to do. So what I did is I found there weren't that many places, but I found the few places in the enemy ship AI where it referenced the player ship, you know, usually to get its position so it could turn to fly towards it and it could shoot at it. And then I made that a parameter, and the parameter was something that was stored on the ship itself. When the ship is created it, that parameter is set to the players ship, but when it's hit with a viral torpedo, I have it select at random one of the other enemy ships.

Did it work? Yes, let's look warning. Okay, so that looked pretty cool, huh? Well, it turns out my code, AS Flawless and diamondlike as my code, is, led to two bugs with very distinct conditions under which the bug occurred, but a very similar fix. So let me tell you what the two bugs were.

The first one happened if you would shoot an enemy ship and it got took taken over, and then it started flying and it targeted another enemy ship and then it destroyed it. After it destroyed it, would just fly away into the Distance by ship, and that was because it had destroyed its Target and the target was marked as inactive and that's not a valid Target, so it didn't know what to do, so it did nothing. A similar bug happened if there was only one ship left and you hit it with a viral torpedo, although what happened there was you'd hit it and then Unity would start throwing reference exception there, errers. Both of these, turned out, had the same fix. The first one was you're targeting a ship that is no longer valid, and the second one was caused when it got hit.

There were no other ships to reference. There were no other ships to attack. So the AL, the, function I wrote to return an enemy ship to attack, returned null. So the first bug: when an enemy ship killed its ship, it had an invalid Target. And on the second one, when you Target alone enemy, it had no target, its Target was null. Both of these, basically, can be considered two different types of invalid targets. I fixed it by making sure that when the enemy's Target was invalid, either it was null or the ship had been destroyed. I then retarget the player.

This adds a nice side effect of the viral torpedo: wears off. So if you take over an enemy ship, as soon as it kills another enemy it throws off the virus and comes back and fights you, and also it doesn't, it makes it so it doesn't do anything. If you viralize a solo enemy ship, there's no other ship for it to attack.

The second type of torpedo I wanted to make was an implosion torpedo. My original idea was that it would shoot out for a bit and then explode, and that explosion would draw on all the enemy ships. The problem was I couldn't really figure out a good distance, and it was also weird that if it hit an enemy before it made it to that distance, it just did nothing. So what I did was I made it so that when, it hit an enemy ship, that ship would be temporarily disabled and would Spin and then it would pull in all the other enemy ships, and that looked really cool, except when it ended. You there had this little ball of enemy ships.

It would just end and they'd all kind of just. Fly off slowly. They'd regain control. I didn't like that, so I tweaked it so that when you hit an enemy ship, an implosion would occur and pull in all these ships and they'd sit there in a bundle and then they'd explode outwards, Ling outwards really fast, and then the explosion would turn off and they'd regain control and come at you.

Let's look warning. [Applause] ] [music].

Okay, there was one other change I mentioned I want to do, and this time was not to photons, it was to make new shields. If you remember, I had a shield which could take a few hits before it would drop, and this just made it so that it was part of my enemy progression, so that it made enemies a little tougher. Well, I redid the shields so that their color would change based on how many remaining hits they had. So I did that. Here's the code.

You can see that at distinct points in the damage to the ship it would change from. The Shield would first show up red, then change blue, then go white and then be gone. Now here's the problem.

I'm color blind, so you can see I I took advantage of unity. You don't even have to do RGB values. You can actually say color red, color blue, color white took advantage of that, but I don't really see that much difference between them. So I made the size adjust too.

Let's look. Warning: okay, two things about the shields that, um. I want to mention one.

Adjusting the size isn't that noticeable. I I thought about increasing how big they get, but it gets kind of ridiculous. So I'm thinking about how to fix that. If you have any ideas, leave it in the comments. Comments — comments also currently the shields only resist anywhere from one to five hits, so I just hardcoded the changes at distinct points.

You know they it They show up red. After another hit or two they go Blue. After another hit or two they turn white and then they're gone.

Notice, I could have coated it with a gradient. I could have put in a fancy gradient that goes, red, through purple, into red, into blue, brighter blue, brighter blue, and then into white, and then they're gone. And then I could have, as you take, damage. I could have moved along that gradient. I didn't do this because it only takes one to five hits, so I did it the easy way.

True, if I change Shields to go 10 to 20 hits, that's going to make them be red for a long time and then suddenly click the blue. That's when I will change it to. Be a gradient. This is an example of code you don't do early. You do it when you need to, very similar to that talk I did about. I wish I could have just put in a simp, had a programmer put in some simple AI code until we needed something more complicated. Don't put in complex code early. You never know what you're going to change things later and that's when you can make the code more complex. It also keeps it easy to bug.

So what am I going to do next? Well, the progression, the enemy progression in this game is currently goes: I throw more ships at you, then I throw ships with shields, then I throw a capital ship with the other ship which does a lot more. It can has multiple photons and Shields, and then finally, that capital ship starts to launch Fighters. So you really have to take it out. What I'm going to do is formation flying. I'm going to have the enemies form up into formations and shoot simultaneously.

This really makes them damage your ship faster, and it's something I did way back in Star Trek 25th anniversary and we didn't use it because it's really hard. But here it will form a natural progression. Maybe I'll have the enemy ships that launch from the capital ship form, create formations, because they're launched as formations. So I'll do that. I'll see if it makes the game harder, too, much harder. If it, if it's really hard, I'll push it off for a much later enemy progression.

But anyway, those are the things I'm thinking of. This is what I'm doing with my toys. I thought you'd like to see it. So if you're making toys at home, you can kind of see how things progress as you play with toys that you never intend to ship but you're just having fun with. Maybe you're learning how to Cod, maybe you're learning Unity. It's just for fun, so I hope you like that.

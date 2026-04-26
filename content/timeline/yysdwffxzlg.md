+++
title = "Toy Update, Part 4"
date = "2024-09-27"
id = "YYSDWFfXzlg"
status = "transcript"
tags = ["Toy Update"]
summary = "Hi everyone. It's me, Tim. Today I want to do a toy update, part four, which is also an insomnia update, part two, because"
references = ["oCKPphehFGk", "wpbUuoyGPBM", "CA7gIg5b6_8", "mHMFG8uvOb0"]
+++

Hi everyone. It's me, Tim. Today I want to do a toy update, part four, which is also an insomnia update, part two, because

I've been up since 2: am and my lack of sleep translated into new code in my toy. I did a bunch of changes to the shields that you guys asked for. I did a bunch of extra code that was floating around in my nogin and for some reason I can do math at 3:00 am. But once I hit the UI — some of the UI stuff — I was going to do the quote Marie condo. UI coding does not spark joy in me and that's where I kind of stopped. But anyway, I want to show you what I did because it's I think it's pretty cool.

The first thing I did was to Shield. I read through all of your guys' comments and there were conflicting comments on what to do with the shield gradient. So what I ended up doing was I pulled out blue. A lot of people said blue doesn't.

Belong in there — and I switch the gradient so that when it first starts taking damage, it's a dim red, then it becomes an orange, and then it becomes a yellow, and then it becomes a white, and that's when the shields will fail. I had flipped it around because a lot of people were saying: well, red to me means damage, but many people were pointing out that red means low energy. So when I changed the direction, I noticed that I wanted to make them fade too. So you hit it and it goes to whatever color it should — B based on its Shield State, and then it slowly Fades out over time. The problem with that is it was not paying any attention to my Alpha changes. Well, I looked at the Shader I wrote and I was like duh.

If you look here, you'll see that Shield color is a. Four Vector — red, green, blue, Alpha — and it pipes into the color on the fragment of the, on the sh, the fragment node of the Shader. But that's only a three Vector. It's only red, green, blue.

Why? Because, if you look down, Alpha's got its own channel, because of course it does. That's where the Fresno output. The Fresno effect output pipes in there, because that's how Fresno work. They compute the alpha and it's um higher near the edges and lower in the middle. So you get transparency at in the middle. So what I did was I piped the Fresno effect into a multiply node and made a new exposed property called Shield Alpha. Those two multiply together and go into the fragments Alpha. Now I have a way of controlling the shield Alpha. So let's take a look at some combat where the ships now go from dim red to bright. White as they take more damage and then they fade over time.

Here we all righty. I thought that was pretty cool, especially for getting all that code done in the middle of the night. I wanted to show some other things. A few of these are things I already had done, the upgrade stuff I'd already had done and, um, I think rear view was done. But let me show you some other things I did.

Um, it's hard to see the ships when they're flying around, especially when there's a lot of detrus and planets and other things in the in the scene. So I made a Target lock, so whenever you uh right click your mouse, it locks on to the nearest ship to your cursor and it brackets it so you can see it happening here. I think it's pretty cool. It was fun to do the math for the projection of. The location of the ship in three space, projected onto the HUD in two space, and draw the brackets there.

That was super fun and then, of course, turn them off if the ship goes behind you. So that was fun. Uh, for funsies.

I thought of another torpedo type which I called a camera, Photon. And what it is when you shoot a photon it puts a camera on it and pops up a little UI element and you can see what that camera seeing. So let's take a quick look at. And that was fun. I can tell you there were some really weird bugs because I forgot to check that it was the player's camera. So every time an NPC shot at me, the camera would switch to a photon. It would, I'd see my ship and it would get really big and then take damage and I'm like, okay, I need to switch that to be player photons only.

So that was fun. Um, while I was playing with cameras I decided I wanted to do a long range scan interface, so I made it so that there was a really distant trailing camera behind the players's ship. I also put a giant green — and I Ed The Shield effect — a gr giant green sphere around the player ship that can only be seen by this longrange camera. And then I made warning, so there I thought that was pretty cool to see a long range camera in place. I don't think I ever showed you guys that I can do a rear view.

Look, so here's a quick running version of the game where I can flick to rear view. Just, you know, switches to a camera that's facing out the back of the ship and I also turn off all the HUD elements. When that happens I don't tend to use it, but a lot of space games have it. So I'm like, okay, rearview we go, or aft view, I think they call it.

Um, and then the other coolest thing I did was I put in a bunch of upgrades for all the different elements that the ship can have, and I've working on this for a while, but I don't think I showed it to anybody. What happens is, as you pick up those little cargo pieces and your cargo meter fills up when it reaches full, the game will pick at random a few things to upgrade. You don't always get to upgrade everything you want. It's very much inspired by vampire survivors where you didn't get everything thing you could buy. It randomly picked from the ones you were eligible for. So I did that here. It kind of represents that.

The cargo. You don't control what parts you're picking up. So you've picked up a lot of parts. Here's what you're allowed to upgrade, so let's take a quick look at that and you can see how upgrades work. I think I upgraded the engines at the end and then showed you how fast I can.

Oh, oh [Applause]. All right, so that's most of the up uh changes I've made in the last uh few weeks: the um because. Some of them predated the last one, but I forgot to show it to you. I know there's a lot of UI improvements people ask for, especially making the um UI have thinner line elements and transparency. Like I said, I'll have to admit I start working on this stuff and I quickly get bored. It starts to feel like work and I have a rule when my — when working on my toy game feels like work, I just stopped working on it. So I stopped and I decided: hey, it's the middle of the night, I'll make a quick video show you guys upgrades and I may stop working on my toy for a while. I don't know, so I probably won't be doing a toy update every week like I've been doing, but I thought you'd like to see where it was as of right now. Anyway, hope you like that.

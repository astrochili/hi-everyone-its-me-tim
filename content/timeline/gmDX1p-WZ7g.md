+++
title = "Writing Design Specifications"
date = "2023-12-12"
id = "gmDX1p-WZ7g"
status = "transcript"
tags = ["Game Development", "Game Design", "Writing"]
summary = "Hi everyone. It's me, Tim. And today I want to talk about how to write design specifications."
references = []
+++

Hi everyone. It's me, Tim. And today I want to talk about how to write design specifications.

Specifically, I'm going to answer a question from Thor RoR TV who asks: I was trying to write a design document for a solo project I'm working on and was wondering if you had any examples of how to properly write a specification that might be given to a programmer or an artist. Also, are there any pitfalls to avoid when writing speci ifications? That is a very good question, thoro TV, and it's also a little hard to answer because there's a wild, wildly huge range of design specifications. You might be writing a might be writing, you might be writing a system mechanic. You might be writing a user interface, you might be writing a — um, some narrative guidelines.

So these are all wild, different, but they all pretty much share in common one thing, which is details. You have to get very, very detailed when you get to the specification level, and that is especially true if you're working with anybody who's not in house, because if you plan to use any external groups, whether it's a art group, code Group, whatever — you are going to want to have as many details in that specification as possible. So rather than try to cover the entire gamut, let me do an example of what I would put in specifications. Let's say you're trying to do a particular weapon that is going to be in your game.

The art and programming specifications look totally different, so let me break those into both. Let's walk through what the artist would need. The first thing you want to let the artist know is what all the different types of weapons are in the game, and this can be a separate document that then you include as a link um at the top of any document — document you do for particular weapon and the reason you need the artist. Needs to know this — is you may have a weapon that just says this is a rifle, a two-handed rifle. We're going to specifications later, but under the weapon types you say: well, we're a Sci-Fi game and we're going to have lasers, and we're going to have plasma weapons and we're going to have ballistic weapons, and even the ballistic weapons look a little sci-fi, like they may have a digital readout of ammo remaining or may have a laser uh aiming scope. This is important because the artist is going to make this thing look like it belongs in your world.

So, even though they may be doing one particular weapon, they kind of need to know how it falls in to the family of weapons that are going to be in the game and that document about weapon types. You may also want to talk about weapon looks, so you may say yes. We have all the different types, but our look is like super slick far future sci-fi or clunky mechanical sci-fi or old timey Victorian brass and steampunk. You want to have a standard look across all your weapons, and these artists are going to do it, and then for that particular weapon specification, you need to include a lot of details. That's my buzzword for this is details.

The artist has going to know whether it's a one-handed or two-handed weapon, because that will determine what animation to use for firing it. Again, they want to refer to that weapon types document to know how many different animations they're going to need. They may get able to get away with one one-handed animation, but two-handed animations there may be one like this, so they'll put their hands in different places. They're going to want to know how is this one held? They're going to need to know things like reload information. How is it reloaded?

Is it something that pops out the bottom? Do they put it? Do they have to break open the weapon to reload it? What ammo goes into it, because ammo will be a separate item that artists will be making and you want it to look, at least visually, sort of like what they're putting into this weapon. They want to know information on how it gets wielded and unwelded. Does it just appear in their hand? Do they do the hands go down and then come back up with it? Do they reach behind them and pull out something?

This is both for what it looks like when you see someone do this, but also when it's first person and you in a first person game, when you see yourself do it, there will be all kinds of information on how aiming is done. With this weapon. Is it just fired from the hip? Does it have iron sights that you look down? Does it have Scopes that bring up a whole new screen that magnifies and has crosshairs — all of these. They're going to want some basic timing info like: here's how long it takes to wield the weapon, here's how long it takes to aim it, here's how long it takes to fire it and recover. Here's how long it takes to reload it.

Well, there're also probably want to know if there's ever going to be any um perks or skills or anything else the player can get. That will change that timing, because if it's too fast, some animations would be hard to do and if it's too long, some animations would look really weird if they're really long. So knowing what that range is will help them decide an animation to use. They also need to know, speaking of animations, they probably want to know things like what non-combat animations still retain showing the weapon and what don't. For example, when you're walking with a weapon, it may show the weapon. When you're running with the weapon, it may show it, although I've worked on some games where when you run, the weapon disappears and then there are animations that certainly never show the weapon, like when you go to pick a lock. The weapon just disappears, and they may want to know: do you want it to disappear or do you want them to unwieldy do? Then you have to add all those timings together to figure out how long will it take to pick a lock. It's unwelded pick reweld, knowing that if someone doesn't have any weapon in their hand, it will use the faster timing.

So you have to take all these into account. And talk to your, artist, about it. This is just for one weapon, by the way. Now let's contrast that to what the programmers will want to know for that exact same weapon. Now they're going to need weapon animation data.

Some of this will come from designers, some will come from artists. For example, you may — you may — be in charge of what animation states there are and what the timings are, but the artists will be the ones who say: well, these states can blend to and from these other states and these can't. Things like, when you're holding a weapon, you can blend into aim or you can immediately blend into fire. Um, some states are animated, so when you're holding it, may have an idol. Where it's, there's an animation for the holding, so some of them won't.

It'll just be here we go. The programmers will have to know.

What happens on interrupt, if I'm reloading a weapon and I get attacked, what's supposed to happen? Does the reload keep happening and I'm taking damage? Does It Blend the taking damage animation with the reload animation? Is the reload halted and does that mean it just immediately goes into the hit and the reload is gone? Do I still show the weapon on a hit?

Do does the? Does ammo get reloaded if I'm in a rupted in the middle of a Reload? Is it partially loaded? Is it fully loaded if it reaches some point in the animation and zero loaded if it didn't reach that point? So if you're showing someone shoving in a, bunch of uh a clip and after it gets shoved in they get hit, is it fully reloaded? If they're bringing it up and they get hit, is it not loaded at all?

These are things the programmers are going to want to know. They also need to know what happens on failure. What happens if the player says they want to reload and they have no ammo?

Does it show something? Does it show the animation start and stop? Does it just go?

No ammo. They need to know that there also has to be a lot of weapon data, um, and the programmers want to know which one of what of this weapon data needs to be exposed to designers — and by exposed I mean they. It's available for them, either through a tool or through, like Unity. Let you expose variables in the and the, structure itself, so it's visible in the unity inspector. They're going to know what do designers want to expose so they can tweak them, and what do they not want to expose.

Like. This is a value we will decide. On and then it's fixed and I don't want it available for people to tweak.

And these are things like: what type of ammo does this weapon take? What's the max ammo it can hold? Um, what? What does this weapon weigh? Um, there's a lot of dat data that programers want to know about weapon use, like: what different attacks are available? Are there special attacks available? Like with a gun, can I pistol whip someone?

Is there a aim it? Can you shoot from the hip and then also do an aim down sight for a special attack? Are there power attacks for this melee weapon?

All of these they want to know. Do these have cooldown timers? Um, the cooldown timers, of course, gets us into interface, like: what are the mouse and keyboard inputs to do all these actions with the weapon? What is going to be displayed on the HUD for each weapon?

Do you want the current ammo amount? Do you want the maximum ammo amount?

Do you want the cooldowns for any of the things you can do with this weapon, and how are these going to be displayed? How do these vary by weapon? Again, it may have to go to a link to an interface document which says: in general, we do this and then the specific weapon uses these parts of the HUD.

These are just things that that are the basics of what have to be done and it sounds like. If this sounds like a lot of work, it is. And also, this is where you have to give actual values.

You can't say, yeah, this reloads slowly, this one reloads fast. You're going to have to Define what slow and fast is like. Slow maybe takes 3 to 5 Seconds to reload and fast is less than. Two seconds to reload.

You're going to have to Define this here so that the animators and the programmers have some idea of what these ranges are going to be. The animators for doing the animations and the programmers for I don't know what, like how fast the cool Downs are going to move and if they display a timer, how big those numbers are. Is it one digit, two digit, three digigit? Um, now, there's some pitfalls you can run into when you're writing these docs and they basically fall into, I think, two types. One, you can give not enough info. If you don't give enough details, one of two bad things is going to happen. Either you won't get something that you desperately needed — oh, you forgot to mention that you needed a Reload animation. You don't have one now, so reload just Boop.

It's kind of magically happen — or if you don't, give DET tails, the other bad thing that will happen is the artist or programmer will fill it in for you. So you're going to get something. You're get it, but it may not be what you want. So you may end up with a Reload animation that can't be interrupted. Sorry, you didn't say you wanted it to be interrupted. This is not an interruptible animation.

The other Pitfall you can run to is you give too much wrong information and you may wonder how this can be. But like when I mentioned having a link to the different weapon types at the top of each weapon, that's to make it off to one side with the person can refer to it. But if you put that at the top of everyone, it's like those recipes you go to on the internet, like I'm going to learn how to make fried chicken and you go. To some recipe and it's someone talking about making fried chicken with their grandmother in West Virginia and you're like I just need to know how to make fried chicken.

Programmers: if they have to Wade through a bunch of lore about a weapon just to get to the cool down timing information, they're going to hate that specification. In other, you should break down your specifications into clear sections and some of those sections, like types of weapons you have, could be done once and just linked to, rather than repeat that at the beginning of every single weapon specification. So if you give too much wrong information, your programmers and artists are either going to not find what they want and miss it, do something wrong. Then you get mad at them because the information was there and they're mad at you because they felt like they had to dig it out. Of a section on narrative, design, or you will just end up having to use the wrong. Whatever they end up doing, it'll be treated like a not enough information problem and they either you won't get something you need or you get something you didn't want. So that's about that's, I think, everything I can tell you about how to write a specification, um, without going into all the different specifications that a game would need.

So theori, theor TV. I hope that answered your question.

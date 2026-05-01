+++
title = "The Cost Of Moddability"
date = "2024-12-26"
id = "dzJCtA-ANvs"
status = "transcript"
tags = ["Modding", "Production"]
summary = "Hi everyone. It's me, Tim. Today I want to talk about the cost of modability, specifically the cost of making your video game modable by end users."
references = ["LH4llMQmJ1E", "coPkWyJIl-M", "T7ToTnHj-CI"]
+++

Hi everyone. It's me, Tim. Today I want to talk about the cost of modability, specifically the cost of making your video game modable by end users.

And this is a really good topic and it came from a really good question by pelicano 1987 who asked: how much in time money does it cost to make a game modable? Usually, players just think that releasing the dev tools is enough, but it isn't. When is it viable to think of allowing easy to mod even something like custom maps or Sprites, 3D models, rules and mechanics? How much does a game lose when it changes Focus to allow for player generated content? I'm going to talk about this. I can't go into specific cost because it varies.

Are you making a, an RPG? Are you making a platformer? Is it just one Indie solo Dev? Is it an entire team?

So I will talk about what goes into making modability. But the reason this is such a good question is there a so many game players. Out there that think along this line.

Why didn't they just make it modable? All they had to do is: and then it's something like duh. Let me just tell you that the answer to this is the same as so many questions that come up in this channel: time and there money, you don't. It is not as easy to make it as modable as you say.

Whenever anyone says just do this, my immediate gut reaction is they have absolutely no idea what they're talking about. Frequently, this is, you know, from manager: hey Tim, why don't you just do this? Because that would just take this long, which would just cost you this much money. Do you still want me to just do that, that kind of thing? And they're like: no, I can't, you just do this right now. And I'm like nope, um, and then we talk about why. It would take that long, which I usually have a good reason for saying why something would take two weeks. It's not just me going and it takes two weeks because I don't feel like doing it, which I've run into.

So first I'm going to talk about what it takes to make a game modable, and let me caveat this, because I have caveats on everything now. It helps to do this from the very beginning, when you first start designing the game, preferably. But before you lay down a single line of code, you really want to have decided how the game is modable and how you're going to make it modable, because retroactive, retroactively converting a game to be modable is really hard, and by hard I mean time, and by time I mean money. You will be rewriting things that already work. You'll be rewriting code that already Works flawlessly, just so.

They all go through a choke point so that you can check for modifications, and I will talk about that at the very highest level. There are three stages to making a game modable, and they are making the systems exposable and then exposing them, and then making the resulting exposed part changeable, and preferably easy to change by a modder. Although that latter part is completely optional, as long as it's exposed and they can get at it at some point, your job is done. Anything you do to make it easy for them to modify it, is you being nice and pleasant and hoping that you have a big modding Community, which may not be the goal of your game? Keep in mind, every time you ride a game, you have goals for it, and is one of your goals easy modability? If it's not, if mod ability is even a goal, why? Are you doing this?

So let's talk about those three stages. Uh, one at a time, so let's start with the first one: making systems exposable. You can do this in two ways. You can either have a method that uses data and you expose that data, or the method itself can be exposable, and I'll talk about that. The former, where your the method uses data, it means you have some kind of way of calculating something that uses parameters, the values, and those values are read in somewhere and you could. That therefore, ultimately, down the line, could be modable by the players.

An example of this would be weight of items. You can make the weight of any item exposed. It's somewhere in a data file, so when you're, when, items are being read in, part of their data is how much they weigh. This means if you, the player, are. Playing this game and go, ah, I wish ammo was weightless, you could. You could solve that by finding where that data is and just setting all the weights of ammo to zero. Contrast this with that second method, which is the entire method itself: is exposed. This is um, it could be function or method, I'll just pick one and I'm just going to call it a method. You expose that, so in this case, there's an encumbrance calculation somewhere and the player in a mod can override the calculation, the entire calculation, not just parameters, which means, instead of making ammo items have a weight of zero, you just skip them when calculating encumbrance. The encumbrance method no longer looks at ammo. They both, uh, do the same thing in that case. But the latter method of exposing the, all the methods in the game — is way more powerful, because you can actually change on the Fly.

Let's say you wanted ammo to — you know certain kinds of ammo — to weigh double, or you wanted it to only, uh, make ammo count if you're playing on hard mode. Really hard to do that with the data method. Uh, very easy to do that with the method Okay, so that's stage one. You've decided to make your systems exposable, so stage two is exposing them. How do you actually expose them?

If it's parameter data, it's pretty easy. They're in files that get read in. So now those files exist somewhere, and we're talking about stage three.

How does the player actually get a hold of those? The method one is harder, depending on your engine, and this is another reason I can't go into too much detail on this because, depending on what engine you're using, putting in overrides are very different. So let me talk.

About what I did in Arcanum and I will link that below if you want more details. In Arcanum there were, for any system, there were two places where I checked to see if there was a script override.

When you're asking, can I do this thing and then do this thing? So, for example, for items, can I pick it up? Can I wield it? Wield it, can I take it off? Can I drop it, drop it off? Take it off, can I drop it, drop it?

There are a ton of other ones too. There are, you know, can the player be seen by this creature? They see them.

Can they go into combat with the player, start combat with the player? The reason you have these that way is a couple things: the override on the cans. Let you override the game and say they can't pick this item up, like can't, they can't pick this item up, like you. Let's say you make an item and you're like Orcs can't pick it up. Boom, that sword cannot be picked up at all by an orc. Let's say you want to say if an orc picks it up, they take damage. Then on the pickup you override and say so, you let them pick it up. But when they pick it up you're like: are you an orc? Take some damage. On the can.

See, in combat you may say something like I want to make a ring of invisibility and no one can see through It's the most, it's an artifact. It's artifact level invisibility, so even C invisible spells won't see it. You just put on the can C function.

Are they wearing this player wearing this ring can't be seen. And that will override everything in the game. You.

May also want an NPC to do something special when combat starts like: y, you know, everyone come to me, we're attacking. You can do that easily by on the combat start on that creature. You just have them say that thing. This made it very easy for people to do all kinds of things in the Arcanum method, but it was something we had to do when we made the engine. We had to make sure if you want all the, all of those, can they do this? It means every way of picking up an item had to go through a single choke point in the code so we could check the script there. And then every way of picking it up had to go through another choke point so that if it overrode the pickup function, everybody used the override.

Not super hard if you haven't written a line of code, potentially very difficult if you've written a lot of code. And that brings me to this third step, which is now that you've exposed all that stuff. How do you make that exposed part changeable? If it's data and files, you have to make sure those files can be edited by the player, and then the edited files take priority over whatever is in your database file. Somehow this has to, because that data has to get connected back in and has to take precedence over what was there.

Preferably, you also let the player bundle all these files. If they make a bunch of different files and they want to put it into a mod, you give them a way to bundle it into that mod. So so the when they want to deliver their mod, they're like: here is a file that you drop into your mod folder and that will override all this other stuff. Now, hopefully these use all the same tools that your developers use.

Maybe they can, maybe they can't. I've used a number of tools at different companies that assume they're on the network of the company, the internal Network, so they can do things like check files into per force, uh, check status of things, uh, put bugs into jira. So they're, interconnected with a lot of other things.

Maybe they can be made Standalone or maybe you make a different set of tools for home users, but again, that would take you time and that costs money. One thing to bear in mind is: once a player mods the game, they have to be able to test it, and that's a whole other thing. That depends on the engine. A modable game May crash and you may not be able to do anything about that. It may be the whatever off the shelf engine.

You're using doesn't handle bad data well. It also may depend on tools like, if they want to mod something that you're letting them override a c script with another C script. It may need to be compiled, so the end user may need to have a c compiler. May Maybe not, maybe you can come up with a different way of doing it, or that may be a restriction to the engine you're using. You also want to think about the kind of error messages you want or even can produce for mods. Like I said, if there's an error, some of the games we've had in inserted into jir and said, hey, this game just crashed and here's the stack. You can't do that for a mo, a modder, because they won't have all those internal networking um features available to them. So you may need to make different error messages for mods.

Again. More time, more money, and just as a side note, I've worked on several games where an error message said something like this illegal script code, see Dave. And we just knew what it meant, because there you shouldn't ever be able to have a bad script op code in there. So if you ever saw one, that's catastrophic. It does not know what to do with that, and so you should go see Dave, because probably something was wrong with the tools or somebody made a change to an enumeration in code and didn't keep it aligned with something else that they were supposed to.

There were also a lot of cases where I've worked on a game where an artist could and did crash the game by checking in a, bad model or bad texture, bulletproofing. All of that takes a lot of time, which means a lot, of money. It also slows the game down to always check as you load in every piece of data check that it's in certain parameters. So many of my games — after we went from our debug game to our release prototype — we turned all those checks off to G to gain speed, usually loading speed, but sometimes running speed.

Guess what? Are you going to leave those mod checks in or are you going to make a special parameter like you can run the game in mod, test mode, and those checks are re-enabled again. Time, money and you now have to explain this to modders. I assume you have someone who's writing some documentation so modders will know what to do. In addition, just adding something like a model occurred to me that models may need. Like a certain model, like a creature model may require certain animation States, certain labels that can be searched for. By the game engine, certain data that has to be there.

It just can't work how, if you put a creature in, there has to be a. You know a way for it to walk around, or is it? Is it flying only? And is that labl flying? And does your game know what flying is and what kind of combat attacks does it have?

And where is that data kept? Is it kept on the creature? Is it kept somewhere else?

All this stuff has to be done. Textures usually have to be a certain size. That used to be. They had to be a power of two or boom. Now they don't have to be, but potentially it's way less efficient if they're not. So all that is documentation that you might have internal that may not be appropriate to externalize.

Some will be, some won't. The ones that aren't have to be Rewritten. Time and money, also — I've already mentioned modability — depends on your engine — Unity, unreal and all the others. They handle modding differently. Some allow you to handle it differently yourself, even on the same engine, so you have decisions to make. Decisions means time. Decision time means money for a f for a game with a fixed time and budget. Adding modability, then, means you won't be adding other features. I talk about this in my video for design fallbacks.

If you want to put in something, you may have to not put in something else, just because you don't have the time to do both and your time is fixed and your budget is fixed. So you have to think about that. In fact, for all of this, I just want to say: think about it carefully. Adding modability is not a no-brainer and anybody who claims otherwise is either inexperienced or trying. To talk you into doing something that they want.

Um, I don't want to say they're lying, but they're basically trying to convince you of something that isn't true. So just remember, if you want to add modability, you need those three stages. You need to make systems exposable, expose them and then make the resulting exposed data something that moders can change. So I hope this answered your question. Pelicano 1987.

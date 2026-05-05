+++
title = "Spaghetti Code"
date = "2026-01-19"
id = "YG4i-F67YOk"
status = "transcript"
tags = ["Programming"]
summary = "I talk about spaghetti code: what it is, where it comes from, and why."
references = []
+++

Hi everyone. It's me, Tim. Today I want to talk about spaghetti code, what it is, why it exists, what people say about it?

Many of you talk about spaghetti code, maybe without using that word: spaghetti code. What spaghetti code is when you look at a piece of code from a game and it's just all over the place. It's poorly structured, maybe there's a lot of methods that have tons of different parameters in them. There's methods that look very similar to each other. Maybe there's duplicate methods. There's methods in different modules that seem to be doing the same thing. Spaghetti code, Basically poorly structured code. Most people go "H, stupid lazy programmer".

I've been on both sides of I've been a programmer and I've been a designer giving programmers specs. So let me explain spaghetti code. Probably a tiny percentage of it is caused by stupid lazy programmer. Most of it is caused by something else. And for those of you who like to do timestamps, because they don't like hearing the context of my question, They don't like hearing the long explanation, Most spaghetti code comes from design specs being changed. There you go, You can tap out now. But let me explain why this happens.

So a game's design specification, its design spec, is written. Then the code is written to that spec. Then the spec changes, maybe something's added, maybe something's — uh, changed, maybe a definition of something is changed, The code has to be changed as well. But usually time isn't allocated to this, because it may have been a feature that's now done. So usually time isn't allocated or isn't estimated well for this, or maybe nothing was estimated for it.

So the code is rewritten, if the code has to be written so fast that you literally can't refactor it, in other words, restructure it from the bottom up to support, the new change. You often end up with that, with spaghetti code. And let me walk you through an example. I'd love to tell you this was hypothetical, It's not. Let's say you're working on a game, Let's say it's a role playing game H. And let's say it mentions DR.

Damage resistance is a very resistance. Damage resistance is a very simple concept. You get hit, if you have 10% damage resistance, whatever damage that hit is get gets reduced by 10%. So if something hits you for 20,- 10% of that is two — You only take 18..

That's damage resist resistance, which I'm going to call DR from now on. The design doc says DR is part of armor. You have one armor you wear. You're wearing plate, you're wearing chain, you're wearing scale players and humanoid NPCs, which is defined to be, you know, bipeds. So your elves, your orcs, your hobbits, they can wear armor and they get DR from the armor.

So the programmer reads this: That's all the only place DR occurs anywhere in the game's design specification. So he writes a function called item armor, getd dr. I'm using he because this was me — That function, when you call it item armor, get dr, looks at what armor they're wearing, that one piece of armor they're wearing, gets the DR off it and returns it. And then it's probably going to be used by the combat programmer — which is often me as well — to get the DR and change damage when it comes in.

Okay, so all that's written, It's really great, It's beautiful, It's flawless code, It's a diamond. Oh, a change comes in. Lead designer, combat designer somebody. Hey, uh, we've decided for artistic reasons and also for, uh, basically make variety, that people can now wear ar, multiple pieces of armor There's. A chest piece, there's arm, hand, leg, feet, foot and helmet.

Oo, a lot of, there's a lot of them. Oh, and, by the way, the DR is summed across those. So basically, you go and add up all the DR from all the different armor pieces and that's what you get. Okay, got it, so programmer goes in changes that item armor get dr function to just loop over all the armor pieces and sum up the DR, Return it. Change is made again: Oh, we don't want it to be the sum of DR, We want it to be the maximum DR.

So it goes through all the armor pieces. The one with the most DR wins. So you don't add them up. Okay, Programmer goes back into that item armor get dr function Still does a loop, but instead of adding it up, they keep track of the biggest. One they ever saw And then, when it gets to the end, it returns it.

Not a big deal, Not. What item get is now looking wildly different than what it looked like before, but it's still working. Wait, another change comes in. We have a spell that one of the spell designers made and it gives temporary DR to whatever casts it. And, by the way, you already have status effects being handled by a completely different system, the status effect system. So it should track that DR as well. So you have a status effect DR.

Well, [sighs]. Item armor get dr now rewritten to loop over all the armor pieces but then call status effect and say: give me the total DR from status effect and it adds it into that. Great, You probably have something in the status effect system too, called status effect total bonus, because you're calling it for other.

Things. Give me all your fire resistance. Give me all your — you know, uh, paralyzation resistance. Give me your poison resistance. Give me, you know, the total number of arrows that have been reflected by the shield missile reflector spell. This, turn, whatever, you have, there's probably a total by status effect type.

But wait, suddenly the inventory UI designer comes to you and says: "Why is the UI wrong in the inventory? It's supposed to give you the total UI or the total DR from all your armor pieces, but now it's occasionally shows an additional value". And you're like: "Oh, that's the additional value from status effects". And the inventory UI designer is like: "I don't want that. I never told you do that, you stupid lazy programmer. I don't want that", so now what do you do?

Do you put a parameter on item armor? Get dr on whether it should. Include status effect DR or not, or do you make a separate function that does it? Or do you call the item armor get dr and then call the status effect total DR and subtract it just for the inventory system. But wait, satisf um already has that gather total bonus for DR for has a. Give me the total bonus for this status effect type And DR is now a status effect type. Wait a minute, when I call that function with DR, how come it's not giving me the item DR, It's only giving me the stuff from the status from spells. And you, the programmer, can try to explain to whatever designer asks this question or QA person: well, we have DR from items and we have DR from status effects. That person may go, I don't care when I want to know total DR. So should that status effect total? Bonus, include items or not? Should the item get armor include items? Should neither of them include items? And if you care about it, you call both and add them together. Or maybe you put a parameter on each one saying: should it include the other type?

Um, [sighs], basically, this is where spaghettification begins, because usually the programmer is not given time to do this, all this refactoring. So it has to be whatever is fastest, whatever you can get done right now. Also, the designers don't know how the code is set up and they don't often care. They're like: why can't you just do what I'm asking you to do? Not even understanding or caring sometimes that different designers have told them different things, which often leads programmers to go to their lead programmer and the lead programmer go to lead designer and go: look, you got to figure this stuff.

Out. I have multiple designers telling my and then telling people different things and you guys keep changing stuff and uh, QA then starts sending in all these bugs. You know, this inventory UI is wrong and this, uh, this, particular display here is wrong. Where the person got hit and the right, the, wrong DR was taken off, or the right DR was taken off, but the, printed display in the combat log was wrong, because you can have a disparity between what the combat system is doing and what the display of the actual effects are saying.

So now we're well along the specification. Wait, at some point they're like: you know what? We're going to add health to armor. So armor can take damage and get degraded. And when it does we want that to degrade the DR as well. And we need to do this because we need an economy sync. We need a repair, You know you can. You have to go to merchants to get repaired. We really need to add a money sync. This game doesn't really have one, or doesn't have enough of one, which, by the way, there's a whole. I did a whole video on how hard it is to come up with money syncs.

Well, guess what? Now, anywhere in the game where you're calculating DR, you need to know the item's health. If it's DR coming from an item, you can't get a total amount. You have to do it bit by bit. And if it's coming from a status effect, that's one thing. And if it's coming from a piece of armor, it's another.

And depending on how you wrote your code, did you just do a total bonus coming from the status effect system, which included all the item DR? Maybe you rewrote it? So when you put on a P, when you put on an item, it just adds the DR into the status effect system. It adds a status effect when you put it on, takes it when takes it off, when you removes it, when you take it off. Oh shoot, You can't do that, now the status effect system needs to know the origin of that DR so it can call item and reduce the DR. Or maybe you didn't do that, maybe the status effect system calls in the item system and sums it up And now the item system has to go off and call the health system and find out what the item's health is.

This is starting to get really complicated. I guarantee by this point there's a lot of bugs that have been introduced. It's a lot of angry designers and angry programmers and they all think each other's stupid.

Maybe. The problem with this is the programmer might not even know the best way to do this because he doesn't know how the stuff is being used. Keep in mind, when he did the loop over the item to get the total DR, he didn't know that the inventory UI designer wouldn't want status effects added to that. So what does the designer want? What does the combat designer want? What does a UI designer want?

There's a lot of questions, so the programmer starts asking these questions. This, can be done in emails. It can be done in strike teams.

Maybe it's up on Slack or Confluence. This slows down the whole process. Time passes. These features aren't getting implemented as quickly. Now there's no time for some additional features to be done, or maybe some bug, some bugs to be fixed.

Producers are getting angry at this. The game slips, or maybe it. Ships with other features missing. Does this sound familiar to you? Do you know of any games that have shipped with things like this?

You, right now, you're thinking, well, I've got, I've got a solution to this. Let me walk you through some of the solutions that have been said to me to fix this.

The first one is: you're not allowed to make changes to design. So designers are supposed to make one big monolithic game design dock and never change it that has never worked in the history of games. No one has ever thought everything perfectly through the first time. They always want to add something or change something, especially if it, if it's exactly what they wrote — and it's, if it's exactly what they wrote — and it gets coded flawlessly and created artistically perfectly, including the UI, and then you start playing and it's not fun. So at that point people usually go. Well, after a certain point, where, draw a line on the schedule. After that point, there will be no changes, Good luck. Never seen that work, Never heard what that good point is.

Is it the alpha, Is it the beta? You, is it shipping?

Then the other thing is: well, why don't you just give the programmers time to do a refactor after every major change? First of all, what's the definition of major change? Also, how many major changes will there be? Also, how long will those major changes take to refactor?

Unless you can answer all of these, we're going to have a problem. And remember this all stems from the fact that usually a game has a fixed budget, which translates into a fixed amount of time you have to do this game. This is why, by the way, um, if you're wondering this, is why games ship late or crunch or ship missing a feature.

Maybe the time it took to refactor was a time you were going to go add uh, NPCs taking cover in combat. I didn't have time to put that in the AI because I was busy changing this DR stuff. Or maybe it shipped with bugs because all these changes went in. There wasn't time to fix all of this stuff before you shipped, because you ran out of time. And then, after all this happened, you probably end up still with some spaghetti code.

There's probably code in the shipping product that never got refactored. The programmer isn't happy about it. Everybody else washes their hands up and goes: "That's not me, That programmer did that", forgetting all the changes they asked for, all the specific exclusions they wanted, the extra parameters, the extra calls, the extra, the, changes in how things work underlying foundationally. You know there's been a lot of foundational changes made. They forget about all that. They like: look, that's not my code, Somebody wrote some bad code there. And then of course, you guys get it and you're like God, that programmer is stupid. Or you just go: wow, developers are stupid and lazy.

What I'm trying to point out here, this is the thing that I've always had to explain to everybody, since the beginning in the 80s to now. Games are not products. They are as much art as they are. Product. Changes happen, Design changes, Art changes, Code changes.

They're not all predictable. The problem with code is you can look at a piece of code and judge it independently and go: this is a really bad, badly written piece of code. Occasionally — rarely, it's because the programmer actually wrote a really bad piece of code. But usually the lead programmers are there to hey, you need to rewrite that. More often it's because that piece of code has been rewritten multiple times to account for changes in the design specs until finally the game just had to ship. And that's where Spaghetti Goat code comes from. And I've seen it in just about every game codebase I've ever looked at, including my own by me. Anyway, that explains Spaghetti Code.

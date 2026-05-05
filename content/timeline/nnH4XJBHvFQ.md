+++
title = "Balancing Game Features"
date = "2024-09-24"
id = "nnH4XJBHvFQ"
status = "transcript"
tags = ["Game Design", "Balance"]
summary = "I talk about how I balance game features with a method I call \"stick a pin in it\"."
references = []
+++

Hi everyone. It's me, Tim. Today I want to talk about balancing game features.

Now this is a question from Josh and Parker who asked: could you go over the process of balancing new game features as they're added to the game? How do you make sure new weapons or spells aren't overpowered but the player is still able to get enough new content to stay entertained? How do you know how many hits an enemy should take to kill Etc?

This is a good question. It's also a tough question. I'm G to preface it with. I think other people have kind of asked indirectly for this in the past and I've been thinking about it because I was never taught how to do this. I've never actually sat down and talked with another game developer about how to do this.

It's just something I learned as I went along and it kind of reminds me of the mathematical proof, where you make an assumption and then you make a bunch of deductions and if you f make deduction, that's false, you know your assumption was wrong, so you go back and change it. So I don't know what to call this, but I call I — I - I referred to it when I'm mentioning it to designers who are on my team — as stick a pin in it. So this is my method of balancing game features: um, that I call as stick a pin in it. So what I do is I pick one thing to start from and I pin it. I'm like this is I'm going to fix this in place and then I adjust other things based on that and when I'm happy with them, I pin them. And then I go on to a bigger circle of things and I figure out how they work and I pin them. And if ever I have a problem, I go back, take one of the pins out and put in new values.

For That's as simple as it is. I know you were expecting something more complicated, but that's it in a nutshell. So let's walk through an example of how I would do this. Let's say you're making a role playing game, because that's what I make, so you let's start with the player and let's start at the player at level one. So think about what changes when the player levels up hit points, skill points, perks.

So let's pin one of those. Let's pin hit points so decide how many hit points the player is going to start with and then how many hit points they get every level. Now bear in mind the amount they get. Every level is going to change, there may be items that give you temporary points and maybe perks that permanently change how many hit points you get when you go up a level. Their attributes, when they start off, can adjust that as well.

Try to factor all that in but come up with, like here's a range. Like maybe the player starts with 50 hit points and every time they go up a level they gain 10, and that can be adjusted a little bit by things. So maybe it's really the range is 5 to 20. So now what you do is you have an idea: as the player goes up a level of the range, their hit points will be at every level. Write that down, use an Excel spreadsheet. Whatever you need to do.

That's your first pin, now decide how that player is going to mitigate incoming damage, how, basically how they reduce it. This could be anything from the armor they're wearing, which may have Dr or DT, damage resistance or damage threshold. This is the time where you're going to pick that. You're going to decide whether your armor has one or the other or both.

I've done all those combinations in my games. Damage resistance is usually: here's a percentage of the incoming damage you throw away. It may be all incoming damage. It may be damage of just a particular type.

We'll get to that. Damage threshold is usually you. Unless the damage does at least this much, it does nothing, you throw it away. Sometimes it means you throw it away and then damage over the threshold — all of it gets through. Sometimes it means you subtract the DT from any incoming damage and if it's positive, then you subtract it. You can do it either way, but you also have to remember there are skills like block and Dodge which will reduce incoming damage, and it doesn't do that the same way. Basically, there's a per set chance they succeed and then, if they, succeed, usually the player takes no damage. So what you have to do there is you have to say, okay, if something has a 50% chance of succeeding, then that's like having a Dr of 50%.

Half the time it does nothing and the other half of the time it all gets get through. So you can treat that as a the same way you did Dr. Remember that there are perks too and other things that are going to factor in and reduce incoming damage. Don't forget healing, if the player has the ability to heal, then they're going to be able to mitigate damage by healing some of it mid combat, whether it's a heal potion, a heal spell, a heal skill pin, that then decide on what damage output you want by level, and you want to break that down probably into the players and the creatures, what, you want to do is you want the idea of how many attacks. You're trying to figure out how many attacks it's going to take to bring down an enemy or the player. So for creatures, you have to consider natural attacks or weapons. For players, it's weapons, abilities like spells and anything they get perks, skills that increase.

That. This should let you calculate what type, what's the damage output of creatures and players by level. So now you have these charts of here's how much damage, or here's how many hit points you have per level. Here's how you mitigate incoming damage per level. Here's how you perform damage by level, and again, those are going to be ranges, because weapons tend to have ranges. The there's some things where there's a chance you're going to avoid damage. So that means it's going to be a range then. So we pin that now.

Let's go to creatures: hit points, which we haven't talked about. Try to decide, now that you know how much damage a player may be outputting. Try to decide how many hit points you want a creature to have, based on how many combat rounds you want it to be before the player can take them down.

Okay, and put a pin in that. Let's stop right here and think about what we have. We now have hit point on both players and creatures. We have damage reduction from different sources. We have damage output for both players and monsters. Take a look at all that. You want to take a look at all that and see what it means.

How many rounds would a typical combat last? How big are the numbers? Is the does? When things reduce those numbers, does the reduction look impressive? Remember going from 100 hit points?

Oh, I would have. Taken 100 to, I would have taken 99.

Isn't that impressive. How many rounds is combat tending to last? As you go up levels, how do those numbers change? This is where you look at those and then you go: oh, I don't really like that. So you unpin one thing back up and recalculate. If you try to do it any other way, I find it getting. It's too complicated. You lose track of things, you're pulling out too many pins at once and everything just kind of falls apart.

So here's an example. Let's say you're trying to think of a new weapon or a new spell or some new ability. Think about: when does it enter the game? What player level do you expect it to enter the game? You now have a good idea of how much damage it should do. You can compare it to other things you've already thought of, like the, weapons in that you already put in the game.

Now there are complexities that I've just touched on here. For example, damage comes in different types. You may have normal damage. You may have fire damage. You may have acid damage. Your normal damage may be broken down into crushing damage and impaling damage and um cutting damage. So all of that factors into the type of damage that comes in and the type of damage that gets mitigated. So that shows up in your attack and defense parts of your calculations. You may have monsters that have multiple attacks. Either they can do multiple attacks around of different types, or they may do different types of damage. They may appear in groups. They can summon other things, so halfway through a combat they may summon three more of themselves or three other. Types of monsters.

You have to take all that to account as damage output. Speaking of damage output, that itself can come in multiple different ways. There's constant damage output, when you're Swinging The Sword you tend to hit, like, especially in The Outer Worlds, we didn't roll to hit, so you could really calculate a constant amount of damage every round. Compare that to spiky damage, where you may be miss, and then you, hit and you do a lot of damage. Or spells that that, um, magic users can cast, but it takes them longer than you know.

A fighter may get in three hits and then the Mages. One spell goes off and does as much of damage. If you calculate the damage per second, those that that spell or the mism hit type of melee is spiky, it does nothing and then a lot.

So you have to. Calculate that and that's why I tend to do damage per second. I calculate and here's how much damage I expect to do per second. Similarly, for charge up abilities, if you have to build up an attack, you either have to hit SE things several times and then you can do your power attack, or you can only charge up and do this attack once every 10 seconds. That's a form of spiky, and again you reduce it to damage per second.

Now, does all this sound hard? Welcome to game Design. This involves a lot of math. Um, I find it's really useful to use something like Excel or some other spreadsheet to do these calculations. I find it's very easy to when you think of it, as I'm going to put my pins in things like hit points and damage output per se per second and damage resistance. Uh, per second this gives you some very good base points to calculate everything else from now.

I'm sure there are other designers with other methods. Oddly, I don't remember ever talking about this with other designers. I don't know what they did. I was never taught this. I've never even heard of a class that teaches it or a book that talks about it.

If any of you know about that, mention it in the comments. This is just one method. You can do it and also, if you choose this method, you don't have to do it in the order. I just present it. You know, I talked about doing hit points and then damage mitigation, and then damage output and then creature hit points.

You don't have to do it that way. You could start with damage output first and then figure out: okay, here's how many hit points I want things to have. So and the what you're really just trying to do is reduce everything to.

Here are abilities that ultimately will do damage. Here's how much damage a thing can take before it goes down, which is a combination of its total hit points and any way it has to mitigate damage. This will give you an idea of how long it would take to bring down a creature and how long it would take a player to be brought down. Those numbers alone can let you do things like figure out how many creatures you should put in an encounter at a particular level, because if you put in too many, it's going to take the player down in a fewer number of rounds than they could take down the attackers. Now, with Randomness in there, it can still happen that the player can die, but if you always make sure that — all the other things being equal and with random roles — if you expect the player to be able to kill three wolves at level one before the player would run out of hit points, that's usually going to happen.

Remember, in these charts you hit maker by level. You may want to vary it by level. If you want your game to feel like it's getting a lot harder, you'll reduce how many rounds it takes a creature to take a player out. Um, usually games get a lot easier because people do the same curve, but the abilities they get introduce a lot of spiky damage or charge damage, which is harder to calculate, and then the player ends up taking out creatures a lot faster than you would expect. This is just a something you're going to have to figure out how to handle mathematically when you pin things. Anyway, I hope this helped.

Uh, Josh and Parker. I hope this answered your question.

That's as straightforward as I can explain it and, like I said, I've never been taught this. I don't know what other designers do, but this is how I've always my games.

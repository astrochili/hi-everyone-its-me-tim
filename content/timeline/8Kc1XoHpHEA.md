+++
title = "Bugs In RPGs"
date = "2024-03-05"
id = "8Kc1XoHpHEA"
status = "transcript"
tags = ["Bugs", "RPG Design"]
summary = "I talk about why there are bugs in RPGs, forever and always."
references = ["jWEuSV_nbfA", "xM6Cr04wWSc"]
+++

Hi everyone. It's me, Tim. And today I want to talk about bugs and particularly bugs and RPGs.

My experience is all in RPGs so I'm sure a lot of what I'm saying will generalize, but I just want to talk about why RPGs tend to be buggy, and this actually comes from a question a lot of people had questions. This is when I picked rrams 1989 asked: will all RPG games always be very buggy on release?

What's the main reason for this? I will break that into two sections.

Will they always be buggy? Yes, they always have been buggy. Um, despite what a lot of people may say or remember, RPGs have always been buggy. Games have always been buggy, yes, especially console games, especially when they were done on um cartridges and media that could not be updated. They were heavily QA and, in many cases, heavily simplified to make sure that there weren't as many bugs. But there were always bugs and there always will be bugs and going forward. I think the situation will probably be worse or at least about the same, and there's a bunch of reasons for that. And remember, I'm talking from experience as someone who has shipped games with a lot of bugs. However, The Outer Worlds didn't have many, very many bugs at all relative to other obsidian games and my own games, so it is possible to ship a game with less bugs. I don't believe you can ship a game with no bugs.

So let's talk about that and remember I'm talking about RPGs. Um, RPGs are really complicated pieces of software. They are extraordinarily complex and made of many interlocking pieces. So, unlike a — and I'm not belittling these games, I'm just doing comparison — unlike a game like Street Fighter, where you may have what a dozen characters that can fight and they each have a few moves and a few animations, they have no inventory. They have no Quest history, they have no leveling.

That game is inherently simpler to make now. It has stuff that's way more complicated. Because of that, people expect more from the animation, people expect more fluidity of combat than you might get at an RPG, but there are fewer pieces to it. So those developers Deep dive on those fewer pieces that they have now in a lot of RPGs, especially nonlinear ones, that nonlinearity, or just the fact that the player can choose to do different things at different times, leads to blocking conditions. Um, this is very much a programming way of looking at it.

Once you have multiple solutions to things, to quests, to problems, to puzzles, this necessarily means you will now have multiple bugs. You will have multiple items being used for those Solutions, multiple skills, multiple character builds. So you have a lot more opportunity for bugs. Also, emergent gameplay leads to something, now, I love emergent gameplay. I have a whole video about emergent gameplay — but emergent gameplay leads to something called emergent bugs.

You have ways of using skills and items and environmental things like hazards or doors or chests. You have ways of — if you have ways of interacting with them that the designers didn't intend that emerg from the rules that were created. This will lead to bugs. This will lead to interactions with those items that weren't planned and do the wrong thing under the rules that were made. Those are really hard to track down. Those are really hard to anticipate.

I would argue. As games become more complex, they're almost impossible to anticipate. You simply have to try to catch them after you make the game. Now, like I said, simpler games don't have all of these, but they do have some of these. There are things that are just really hard to make sure that you catch.

Every possible way something could be used every possible way. Somebody did key presses or moved the controller or interacted with something while using something else or under a condition, having a status effect on them, how multiple status effects interact. These are all things that can happen in the simplest of games that make them really complicated to try to test.

Now somebody else asked on a different question. Well, how do you even rate bugs when you're, when you're making a game and you know there are bugs in there, how do you rate them? Because you have to rate them somehow. You have to acknowledge at some point, beyond the most simplest game, you are going to have probably more bugs on your bug queue than you'll ever be able to reach, and some of you going well. Some of them are minor, well, how do you rate them?

What's the difference between a major bug and a minor bug? And I will tell you how I rated them on my RPGs. So the highest rated bugs, the ones you did not want to ship with and when you saw them arise in testing, were ranked the highest in the cue of things that need to be fixed. Crash bugs number one. You do not want people crashing because not only is that horrible for the player, because they lose all their progress, but it's. It shows an underlying instability that will make people unwilling to keep playing, because if it happens multiple times, or if it happened after they Lo, they hadn't saved for a while, or if it tends to happen when certain things occur and suddenly they realize, oh my goodness, my build is causing crash bugs. They just stop playing, so crash, crashing is probably the number one reason people rage quit a game.

My other highest rated ones for my games are things like: you've made a build that you discovered cannot complete the game. Either you don't have the skills that are needed, or this build tends to get a set of quests that can't be done, or this build can't acquire all the things that are needed to complete the game, for whatever reasons. That's horrible too, because the player isn't responsible for this and there was no to anticipate it.

Suddenly they find after 5, 10, 50 hours, yeah, the character they're playing can't finish this game. That is so draining to have that happen, and then that's so. That's the second um kind of bug that I rate the highest. The third one that I give the highest rating are things that would prevent the game from being certified. Windows and all the consoles have certain things that you need to do to make sure they get certified and if you don't pass any of those, they won't let your game ship. This can be anything from you're not connecting to their Achievement System or, um, you can't quit out of the game at any point. Or you have put in content that don't meet the rating that you said your game was for. So you put in some mature content but you ask for a teen rating.

These are all things will prevent your game from being certified and if you're not certified, you're not shipping on that platform. So those, three things crashes, um, not being able to be completed and not being able to be certified. Those are the three highest kind of bugs that you look for and go. These have to be. Fixed, now you may have a lot of those, which is part of the reason these lower tiers may not all be cleared out before the game ships. So the next tier down would be finding things that were incorrectly implemented. So you're playing the game and you're like: o, this skill isn't working the way the design doc says it should or um, I thought this item was supposed to be able to do this and it's not doing that, and that will prevent something from working. Or now this item isn't seen as very good, when actually it should have been one of the best ones in the game.

So then you have to go back and say, hey, implementor, you need to fix this. But there's a flip side of what can happen, and that is something was correctly implemented but it's causing an issue that wasn't anticipated. Maybe it's interacting. Badly with an environmental item, maybe it's interacting with other items, so maybe two items were put in individually. Those items are fine, but together they cause a problem. Maybe things don't stack correctly, or maybe they stack and cause a bug or whatever.

And then you have to decide what to do. Do you, because the implementation is what was on paper? Do you delete that item or that feature? If it's a feature, it make it may. Deleting it itself may cause ramifications.

Oh no, we can't take out all of crafting because crafting was considered when we made our item economy. So not having a crafting channel to get items into the game means that there are Level ranges in the game where you can't get good items, or you can't get the best item because it's no longer available because you took out crafting. So sometimes deleting things from a game causes a lot more work than leaving it in and fixing the thing that's broken. So those two things — either incorrectly implemented things or things that are correctly implemented and now causing issues — are probably the next tier and then the lower tier ones are things like: this isn't fun. We did this, we put this thing in.

People are playing it and they say it's not fun. Maybe you have a class that isn't fun. Maybe you have a dungeon that isn't fun. Maybe you have a skill that no one ever takes because it's not fun. Not that it doesn't work, not that it doesn't have some utility, it's just not fun. So people aren't playing it. We also look for areas of the game that aren't clear. Maybe when we looked at our Telemetry of play testers, we found that people tended to stop playing at a certain point.

Maybe it's not clear how. You're supposed to advance the main quest line. Maybe it's not clear how you're supposed to get that important item. Maybe it's not clear who you're supposed to talk to next. Those are things that we look for and go: okay, we need to clarify things which may require writing, new dialogue, um, changing the way Quest markers work. It can be a wide range of solutions to that problem and that's why you end up having to talk about it and try to figure out what solution can we Implement with the time and resources we have left?

And then the final one I was. I didn't know how to talk, how to classify it, but I call it sanding off friction. You look for things in the game that are just causing people to be frustrated. Maybe drop rates aren't high enough, maybe they're NPCs that are just super annoying to interact with. They were written to have character.

I've talked about this, if, this main NPC — his personality — is entirely being sarcastic, maybe a lot of players are just like, uh, I hate talking to that guy, so I call this sanding off friction. These are bugs that are put in where people just don't like It's, it's just something you got to fix. So those are low priority because, like I said, I'd rather fix a crash bug or an incorrectly implemented feature before I start sanding off friction. But if you've ever shipped a game with a lot of friction — which I have — people don't like that either. Um, now, I know a lot of people are thinking, but it's gotten worse lately because people ship games that aren't even look like they're even trying to be done. And yes, everything I just said is true for games from day one in the industry and games being shipped now.

One thing that makes all this worse is when Publishers or anybody who has the money basically goes: we'll just patch it later. Let's ship it and we'll patch it later. That wasn't an option back in the day, where you burned it onto a cartridge that couldn't be fixed. Or you shipped a game for console where you played it by popping in a CD. There was no hard drive so those couldn't be fixed, so you had to ship it as close to possible.

Now people are like: I don't want to keep spending money, let's ship it, make some money and then use that money to try to fix these bugs. Also, if you're kickstarted or self-funded, you may just run out of fund. There may be no money to go in and say, o, we need to fix this.

You're literally done. You can't pay people, so unless they want to work for free, you're shipping what you got or you're just throwing it all away. If you just literally think that this will be so awful that it will ruin your reputation, you just throw it away.

There's a lot of games out there that you've never heard of, that you'll never play, because they were canceled before they even hit a part where the company would mention that the game existed. So, yes, patching — patching things post — relase - has made this problem worse, but it didn't create this problem. So probably everyone now is going: well, how do we stop this? How do we prevent this from happening?

It's complicated, but I have a few things. I thought of a few ways of doing it. Basically three ways of doing it.

One: start: QA, start Play testing early, as soon as the game is playable, maybe as soon as you made that. First playable, but certainly by the time you've made a vertical slice — try to have a QA, a play test group, playing it. Now you have to make sure these play testers are aware of the state, because there's nothing more Soul draining for a developer to say, hey, I'm giving you a gray box level. Can you tell me if you feel the mechanics are good and all your feedback is it's ugly?

I hate it I don't like this. It looks stupid. You, why are you making this?

It's frustrating to have play testers who don't understand the stage of play test testing. Not everything is in its final form when you get it and you have to understand that before you start Play testing it. The second way of getting better bugs, I think, is having in-house QA.

I've always had far more luck with people I can go and talk to. Than people who are not only not at the company but maybe not even in this time zone. So I've got to come in at 6:00 am if I want to talk to them, or I've got to stay till 11:00 pm because they're literally on the other side of the planet.

Having in-house QA means they can access design docs and since we do, are design docs now up, say on Confluence or something, that are living design docs, changing design docs. They can have access to the most recent design doc. So when they're playing the game they're like that's a weird skill. They can go look and see exactly what is intended for that skill to behave, so they can write a bug confident that hey, this isn't working the way it's supposed to.

The other thing I love about Nas QA: I started doing this back in Fallout and I loved doing. It I couldn't do it in everything for at troa, but I wanted to — is a weekly meeting with the QA lead. I like to do this as early as I can, probably past the first test playables, but at some point I started having weekly meetings and part of that weekly meeting was just having him tell me what are the worst bugs you've seen. Why do you think these are so bad? If I can't tell like this bug doesn't seem important, why is it on your top 10 list this week?

What do you feel about the game? How does it feel that no one will play your game more than QA? They sink so many hours into your game.

Ask them how it feels, get opinions, and a good QA lead will not just tell you how he feels, but he will have talked to the people on the team and go: well, the action — people are loving it, but the story people not so much. This is really valuable advice to be getting from your in-house QA Department. If you're not getting that, I feel sorry for you. We got that for The Outer Worlds and I think it's showed in the final product, because it was very, very stable and not bug free, but didn't have a lot of bugs. So that's a second way in-house QA helps. And then the final one is having test plans. So you as a designer should be able to describe how your features should be tested.

Here's a skill for lockpicking. Hey, I want you to lockpick a door, but also, do chests also use it on? You know, maybe there's unusual things that can be locked, like occasionally, um, you know, a dead body will have a, something that you have to pick, or maybe it also works. On computers, who knows? Just write down those test plans and then make sure they're followed.

I've already told stories in other videos about: on my D and D game, QA didn't really test bards — they didn't like them. And on my vampire game they didn't test naratu because they were ugly. I'm not saying they didn't test them at all, but they barely tested them.

There were some really really obvious bugs that we shipped with those characters. Um, that they just didn't follow the test plan. So you have to have a test plan and you have to know it's being followed. One thing that helped being followed: that weekly meeting with your QA lead.

Now, what is all? How can I wrap all this up? Everything I just described takes money. You want to test early money. You want to have QA in house money. You want to have test plans, and make sure they're being followed. Money, because that's a time your, designers, will be spending not designing but instead writing test plans for their design.

That's times where QA people won't be playing. They'll be looking at the test plans and planning how they're going to play. Then you're going to have be meetings about whether you met those test plans.

That's all time. Time is money, so ultimately, I could have gotten rid of this entire video and just said: why do games have bugs? Money — will we always see games with bugs? Yes, because of money. As long as money is not infinite, you will probably see bugs Because unless the game is made so narrow in scope that they could test every possibility in it I hope this gives you some insight into why you should expect bugs in games and I hope our crams 1989. This answered your question.

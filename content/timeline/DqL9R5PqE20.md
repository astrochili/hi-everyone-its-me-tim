+++
title = "Implementing Randomness"
date = "2023-08-03"
id = "DqL9R5PqE20"
status = "transcript"
tags = ["Programming"]
summary = "Hi everyone. It's me, Tim. Today, I want to talk about randomness."
references = []
+++

Hi everyone. It's me, Tim. Today, I want to talk about randomness.

The reason I want to talk about this is Randomness is probably the one most logical, mathematically defined objective — no room for feelings — topic that I can imagine that I've had more conversations about with other developers, with fans, with reviewers, with everyone in my entire 42-year career. It is a strange thing: I talked about this in a conference I did in Dubrovnik: reboot 2017.. So, if you've seen that's what I'm going to talk about, but I wanted to kind of go over here because someone asked me to, talk about it and I think it's funny, so I I brought this up a lot in the past, so I will talk about it here. Um, the first story I like to tell was from Fallout. We Fallout used a linear congruential generator that I took out of a — uh, a book called numerical recipes in C.

It's a very simple, long period, random, pseudo-random. Generator, which means it doesn't repeat for a period of time longer than the universe. So, and it's got a very good chi-squared value, meaning it produces really good random numbers.

Still. One day — uh - I believe it was ahead of QA, but it might have been one of the QA — seniors for Fallout — came into my office and said the random number generator is terrible, you've got to fix it. And I said: tell me what you saw happen. And they said I was standing right next to someone. I had a 95 chance to hit them and I missed. I'm like, well, and he goes, I missed three times in a row.

I'm like, well, let's do math. I love math.

A 95 chance to hit means there's a five percent chance to miss meaning. There's a one in 20 chance you will miss meaning on average every time you. Shoot someone. You should expect, out of every 20 times, to miss once. However, this is a truly randomly generated number every time it is not. Here's all the numbers from 1 to 20, in a random order, and we will re. You know we won't reshuffle that until we're in.

Every time you roll that die, you might get a one. So the chance of missing twice in a row is one in 20 squared, which is 1 in 400. The chance of missing three times in a row is one in 20 cubed, which is one in eight thousand. Now you may go wait a minute. One in eight thousand, that's almost never gonna happen.

Well, let's look at it this way: if you shoot 20 times in an encounter — and let's say some of them are less than that, some of them are way more — if you have 10 encounters an hour because you're in QA and you're constantly playing the game, then that means you're going to shoot about 200 shots an hour. So you work 40 hours a week. Wait a minute, that's 8 000 shots a week. So you should expect to see your character Miss three times in a row, about once a week. I remember he sat and looked at Matthew — something's wrong with that — and I'm like: no, you've been playing this game for months. I expected you to miss three times in a row, many, many times. And it doesn't matter if I change the random number generator, that's gonna happen. So, so the next couple examples I gave were from WildStar, because I used to be the programming director on WildStar and I tried to handle the programming cases that were just small and self-contained so I could get them done in a reasonable amount of time and not pull one of my programmers off a bigger, um feature of the game. So one of the things that came up in WildStar was music was repeating. But here's really the story of what happened.

So the audio director gave me five songs and said: play them randomly. Okay, perfect, so what I would do is when it was time to play a song, I would pick a number from one to five and I would play it, and when it was done I'd pick a number from one to five again, then Play It Again. He came into my office the next day.

Hey, uh, I saw what you did and the problem is I heard song one and then I heard song one again. I was like, yep, you sure did. That can happen. You know there's a 20 chance you're gonna see a song back to back.

And he goes, well, that's not what I wanted. I never want to hear song back to back and I'm like okay. So what I'm gonna do is I want to pick a number from one to five, but if it's the same number as the song I just played, I'll just pick again until I get a different number. Now you're never gonna hear the same song.

Twice, he was in my office the next day. Well, I heard song one, and then I heard song two and then I heard song one again. I'm like perfect, and he was like no, I never heard songs three, four and five. And I'm like you're right, I'm doing it randomly. He goes, well, I want to hear all the songs played before you replay one.

And I'm like that's not random. He goes: yes, it is, that's everybody think. That's totally random. That's the.

Most complete random you can be, and I'm like: no, that means that if you, know, after the fourth song, you know what song is coming up next, because there's only one song that has been played. That's completely not random, and he goes: well, that's what I want. I'm like: okay, so here's what I did. I would randomize the sequence one through five, play it and then re-randomize it next day. He was in my office. He goes: I can't believe you did it again.

I heard two songs in a row. What he heard was songs two, five, four, one, three and then three, five, one, four, two. Notice that three ended the first randomized sequence and began the second.

So what did I do? I went into the code that randomly shuffled the numbers one through five and when I started to, when I made the new Shuffle, I remembered what. The last song played was and if it showed up in position one I would swap one with a random the, song in the first location with a song in locations two through five. So I just randomly swapped them.

Boom, he was happy. Note: what I wrote is not random. I did a shuffle which then is played in order. So it's not random, because the more you go along, the more you hear songs, the more likely you are to know what's coming up, because it's any of the ones that haven't played yet and you're guaranteed you will never hear a song back to back, which can happen in Randomness. But he was happy, he didn't want random, he wanted Shuffle without replacement. But we moved on the design team on WildStar — this is what I've said on the programming team — a designer came to me and he said: hey, I need you to redesign the loot system so it has Randomness. And I'm like, what do you want? He goes: I want a monster, that can drop loot twenty percent of the time. And I'm like, okay, so about one in every five kills, you're gonna see Loot drop.

He goes: yes, coded it in super simple. I know what you're thinking. You should have learned by now. He didn't want random, but I, I mean I asked him: that's what you want? He said, yes, so he comes in the next day.

Hey, I killed 10 monsters in a row and I never saw Loot drop. And I'm like, yeah, that can happen. There's a one in five chance it'll drop. You might kill tan. He goes: well, that's not I want he goes.

What I want you to do now is, every time you kill something if it doesn't drop loot. I want you to up the drop chance. And I was like, okay, well, I can do that. He came the next day: I'm still killing lots of monsters and he wouldn't give me a number, but he goes. I'm still seeing lots of monsters without saying drops. Okay, what do you want me to do? He goes. Okay, in addition to the loot chance that I'm going to specify and the fact that every time you kill a monster and it doesn't drop loot, I want you to up that loot chance. I want to put in a maximum kill count before it ignores the loot chance and just automatically drops the loot.

I said, okay, I put that in. He was happy. What I did was totally not random. I mean, it's completely not random. You know you will see a Loot drop every end kills 100 of the time. It is not random.

I thought we were done. I'm like I got this Randomness stuff behind me. He came to my office two weeks later and said: hey, I said Critical Hits to 20, but I just shot someone 10 times and didn't get a critical foreign and did the same thing for criticals. Note that what I was doing took a very simple call to a random number generator with a predefined percent chance did I make this role and instead I had to keep arrays of data around in the music. In the music it was all the pre-rolled music that was going to play in the Loot drop case. I had to keep how many times this player had killed this type of creature without getting a drop so I could up the loot percent chance by a certain amount or check against a Max kill count.

Keep in mind they may leave, and come back. It's all the players doing this. It's definitely a lot of data.

Keep around, it turns out, I would say, most of the time, when a designer or almost anyone but a programmer, says to you: I went Randomness, no, they don't. Randomness to a programmer means you're rolling some dice, taking what the dice show. Almost all the time what they want are shuffled permutations. Meaning they want the POS, the list of all possibilities that can happen to be enumerated, stored, shuffled, and then, when you get into that shuffle, reshuffled with some modifications so you don't see the end of the first permutation occur at the beginning of the next permutation. Permutations are not 100 random, they are a random shuffle. It's like when you randomize a deck of cards and you start giving out the cards.

Yeah, you can't. See somebody get the Queen of Spades twice, because it's not a random shuffle, it is a permutation of the of the deck and until you get to the end of the deck you won't see the same cards again. That's why in Vegas, they often reshuffle decks, uh, before they get to the end, or they use multiple decks so people can't do card counting. Randomness is something that has affected every game I've made. It is a funny thing that it's basically an example of smart people using a word that doesn't mean what they think it means and even though you try to get them to use other words, you know a few weeks later they're back to hey, this isn't random. So what I learned as a programmer is to listen to what people wanted and not what they were asking for, which, by the way, is a very good skill. When you are also reading reviews and game forms about games you made, people will tell you they want something, but it's not what they want. They want something else. Either they don't have the vocabulary or the self-reflection or they just can't even put into words what it is they want. But frequently people ask for things and it's not what they want — something else, and it takes a while to extract that from them.

So I hope this helps. Uh, everybody understand not only the general difficulties of game development, but if you're actually a designer or programmer, I hope you approach your features a little more openly and a little more non-vaguely, you basically need to learn what the terminology means and how to ask for things which are exactly what you want and not. Well, this is what I'm going to ask for and you should. Figure out what it is I'm asking for, but I wouldn't hold your breath that this will change anytime soon. This has been happening for decades, but I think with a little more forethought, I think development can go a little smoothly. If people just think about what it is they want, how they're expressing what they want.

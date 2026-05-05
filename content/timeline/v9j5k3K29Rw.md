+++
title = "Making of Bard's Tale Construction Set (1991)"
date = "2023-06-06"
id = "v9j5k3K29Rw"
status = "transcript"
tags = ["Programming", "Retrospective"]
summary = "I talk about how the Bard's Tale Construction Set video game was made in 1991 at Interplay. I forgot to show the box for the game, but you can see a giant poster board reproduction of it on top of the display cabinet behind me."
references = []
+++

Hi. It's me, Tim. Today I want to talk about the making of Bard's tail construction set.

That was the first game. I made it interplay and I was a contractor. I didn't get hired until after the game came out the way it all came about.

In late 90 my father passed away. We weren't terribly close. My parents had divorced when I was young. But the impact of having a parent die, especially he was only 57, he's my age, I was only. I thought I was 24, I was 25.. And I was still in grad school and it just made me rethink what I wanted to do. I was on course to become a college professor. I rethought that. I had so much fun making grandstand bridge and I'd never stopped making games.

In fact I'll do a video about. I got really involved in the mud scene, multi-user dungeon. I'll do a whole video about that because ironically it ties a little bit into Fallout. But what I did was in.

Early 91 I went to the bookstore and bought several computer gaming magazines, like computer gaming, World, PC Gamer — I forget which ones they were — and I went through the ads and every video game company that had an address. I sent a resume to. I don't remember how many I sent, but I got two responses. One was 360 Pacific, which I think was an organ. The other one was just a few miles from where I lived. I was on campus at UC Irvine, and over in Santa Ana was a company called interplay which I'd heard of and I played Bard's Tale Two. I hadn't finished it because I was. I was in the gold box games and I'm like, okay, I'm gonna play this.

So I responded. They responded to my letter. I called them up. I talked to someone named Tom Decker who later on I would work for, and I got a an interview. I was so nervous about the interview that I went to a friend of mine, John Roy, and asked if I could borrow one of his suits. And he gave me this really fancy, expensive Italian suit. And if, oh man, it fit so well, I was like this is a nice suit. I went in for the interview. The receptionist thought I was their insurance salesman. So as soon as I walked in, says, oh yeah, your appointment's very soon.

I'm like great. I sat down and then she said, okay, you'll be meeting with so and so from HR. And I'm like shouldn't I be meeting Tom? She goes, what's your name? Again, and I told her and she said: Oh, I thought you were our insurance salesman.

No programmer shows up here in a suit. By the way, Jesse Reynolds showed up for his interview a few years later — an interplay — in a suit, and, yes, I made fun of him for it anyway. So I had my interview with Tom and he told me there was someone else who had applied for the job and she and I were neck and neck. Um, we had about the same amount of experience. I think she might have even made a game before and I had one game under my belt already. I had Grand Slam Bridge published by electronic cards. By the way, that was the interview where Tom actually looked. He owned a copy of grandstand bridge and he looked at it and my name — my name is not the credits — and that's where I found out.

I was really upset. He said later that he believed that I worked on him because I look so honestly upset that my name wasn't there. But what sealed the deal for this job was he said it was a Bard's Tale and that was, you know, like d, and I said, oh, I play D? D all the time, and he said: can you tell me what thako is? I was very excited. I proceeded to tell him that Falco stood for to hit Armor class zero, that for the classes in d?

D there were four thako tables based on the base classes of fighter, cleric, thief and Magic user. Then I told him what the factos were for level one against AC's, what the number was for the thacko, and said: and the trick is, you can take whatever your armor class is and um, subtract it from thako to get your to hit value. So if the fact goes 18, then AC 10, you only need an eight. And I said: but it doesn't work for a magic. User because stackers repeated six times and that isn't the first 20.. On the magic user column Tom had been quiet during this entire exuberant explanation, and he said: yes, thako is to hit armor class zero.

That's all he wanted. I found out later that the other programmers — she didn't know what that go was and he was impressed and a little taken aback at how detailed my answer was. But he said: yes, you certainly played d, so I got the contract. It was a 14-week contract, 14 weeks to make Bard's Tale Construction Set using the code from the original bardstale, which I was told was a black box, meaning I should be able to lift that code up, set it down and just shove new data into it. So what they really were hiring me to do is to write editors for data so that a, the player of our construction set, could create an item or a monster or a new spell and just fill in data.

Problem I was supposed to come in every two weeks at the a few days later I called Tom and said, this code is not a black box. I actually drove over — it wasn't too far away and I showed him like deep buried deep into combat code there was a line that said if monster equals 59, then do dragon breath. This is all C code it was, so not a black box. I mean, there's no way I could use that. There's no way that combat code could be considered a black box. Who knows what monster 59 was going to be?

And obviously it was a dragon, but there was no enumerations for types. There were monsters, didn't have a drop down for a type. Didn't have an enumeration set in them, so I could go: oh this, type is Dragon, so let's see if it's time to do dragon breath.

All the rules for, like, how often something could happen, like you could, how often. Think Dragon was hard-coded so there's no way to change it. And these were all things they wanted.

Done, there was another problem too is they couldn't find the source code for the version they wanted me to build it off of. I think they wanted me to build it off of bar scale two, I don't remember — with two or three, but they couldn't find the English version. So they gave me the German version — and I don't read German — and, yes, the strings were embedded in the code. So I was like I, I can't do this, can't be done in 14 weeks. So first I got to spielvo.

You agreed to do it in 14 weeks and I said I also you agreed it was black box, so I will do what you asked for, but it won't work. I will write editors for data and put it into the code that you said was Black Box. It won't work, but if you're going to stick to the letter of this contract, so will I. That kind of worked. They assigned another programmer to do the. When you're playing Bart's tale, there's some data up here, there's rolling text here and then there's a uh picture here and the picture is animated. So if it might be a person pretending to talk — it wasn't lip synced — it might be a monster, you know doing this. They got another programmer, Phil Britt, to do all of that and that was actually a lot of work because, again, that wasn't something that was easy to extract.

In the code, but also I wasn't really that up to speed on PC graphics if this was an Atari boom. It also meant that he interfaced with some of the artists a little more than I did. I like talked to Todd kamaster who was their 2D art Master. Todd was an amazing artist and I did things like the menus and um editors and things like that, but Phil worked with them on all the animations.

So that was great. That let um. That freed me up to basically spend weeks, and I was doing this all in my dorm at UCI and there wasn't room anywhere else. So I pretty much threw everything off my desk in my bedroom and plopped a computer down which they supplied because my PC couldn't handle this. It was in VGA, not super VGA, but my computer was EGA. That's how old things were. Oh and our construction had to run in VGA, EGA and CGA.

CGA was four colors and you didn't get to pick them. It was black, white, they were called cyan and magenta. Even back then my color vision was so bad it kind of looked like an off-white. And then this puckiest purpley color that I've ever seen. I don't know who picked those, some insane person, but it had to run in all three of those modes.

Luckily the resolution was the same, so it was 320 by 200, either in Four Color, 16 color or 256 color. Honestly, I really think it only looked good and played well in VGA, but they just wanted to support it to make it backwards compatible. So I went back to doing all this work.

Funny story: the very first check they sent me bounced, I got paid when I went in every two weeks. To say, Tom, they paid me a check at some point, and I forget how many weeks in — I took it to my bank. The next day the bank called me and said that check balanced and I was like, oh, and they said there's a fee for bouncing. I was like, ah, caught up in her play, talked to HR. Uh, the one there apologized, said that they had such a constant payroll amount that she forgot to increase it. When they brought me on as a contractor, she issued me a new check plus the amount of the bounce fee.

Everything was good. She was mortified. I was like, look, it's fine. I didn't tell her that as a grad student I pretty much lived, you know, paycheck to paycheck. And now that I was doing this job I didn't sign up to be a ta uh teaching assistant, which I normally did every quarter, which that was interesting because, even though it was an AI grad student, I ended up taing programming, languages, operating systems, because that one was at eight in the morning and I was the only one would get up that early — a whole bunch of things that were not AI related, but I didn't do that anymore, so I could do this anyway, we finished it.

There was quite a big bug push at the end, but we had really good QA. Um, that was where I met Chris Taylor. When I'd go in every two weeks to talk to Tom, Chris Taylor would often come in and just stand there and listen and I didn't know who he was.

He would just stand there at the wall going and it turns out he was just really excited about this being made. Um kind of wanted to be part of it, just. Loved coming in and having me say, every few weeks this feature's in, like you could do this, you can do this. You can make maps, you can make spells, you can make traps, you can make monsters, um. We finished it up, got it debugged, it shipped in the fall, I want to say October of 1991..

The first game I'd had out since grandstand bridge in 86. It got reviewed in the dragon magazine a few months later and it got five stars. I was stoked. I mean, I had a subscription to Dragon magazine. Have my a game with my name on it in Dragon Maxine.

That was cool, so of course that was so much fun. Went home for Christmas break back to Virginia, visited my family, came back and basically told Tom I won a full-time job in the game industry and I hope it can be an interplay. Because that's where I want to do it I want to make more RPGs with you guys, but I'll send my resume out if that's not possible. And Tom went to bat for me and I got the job. So that is the story of the very first game that I ever made for interplay.

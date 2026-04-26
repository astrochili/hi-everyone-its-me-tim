+++
title = "Developing Tyranny"
date = "2023-09-24"
id = "KZTkg50ihsU"
status = "transcript"
tags = ["Obsidian", "Programming", "Game Engines"]
summary = "Hi everyone. It's me, Tim. Today I want to talk about the development of Tyranny."
references = []
+++

Hi everyone. It's me, Tim. Today I want to talk about the development of Tyranny.

Now, like my Pillars of Eternity talk, I was not a lead on. This project only lasted about a year and a half — half and I don't have a lot of notes, but I will try to tell you the major points. For me, this is all, again from my point of view here, the actual development of Tyranny. You need someone like Josh Sawyer or, um, not uh, Brian Hines, who was the game director, uh, Chris Avellone, who started as the game director. So I'm just telling you the point of view of someone who did programming. I started working on Tyranny right after pillars of fraternity shift in March of 2015. It was not a sequel, but it did use the engine that pillars used. So I was already familiar with the code and I was up to speed on Unity. So it just made sense to move me right onto Tyranny and I started working on it. Now, when I started, Chris Avellone was the game director for it and he had given a very interesting mandate.

There were things that didn't exist in the world and one of them was religion, and I remember talking to him about it because I said I took a — I don't think it was my religion class, I think it was a philosophy class I took in college and there was a professor who said — and I don't know if this is true, but there are three things that every human civilization has always created, with no exceptions, no matter how remote, no matter whether it's in a cold or temperate or tropical zone, no matter what. Humans have always invented: religion, dragons and soup. You can find them in every, culture, every civilization all around the world. So I thought it was interesting that there was no religion. He just that was. Something he wanted to explore and I'm fine with that. There was a lot of things in my games where I would lay down something we're not, this is something we're not going to have, or this is something we're going to explore. So I got it.

What was interesting was one of the programmers, Brian McIntosh, had this fantastic idea for explaining that lack of religion and also why edicts existed. He told me, and I thought it was great, it didn't go anywhere. I don't know if it got shot down or he didn't promote it, but his idea was that at some point — why, playing Tyranny, you can come across a cave that's really hard to get to and really hard to get into. Maybe you have to knock down a wall or something and you find an older man sitting there and you tell them: hey, I the way, he's free. And he goes, I cannot leave this cave, and you can eventually get him to explain that he is a God, maybe the god. And he saw when people started worshiping him and asking him for miracles. He saw how bad that was for them.

So he issued an edict that there could be no religion. The side effect of this addict unwittingly trapped him in the cave, because nobody's, nobody can see a god, because that would cause a religion, and it also meant that his ability to do edicts was stripped from him and distributed into the world, possibly in the towers, possibly where Kairos got it, possibly where you got it. By the way, there's spoilers for Tyranny in this.

Anyway, I thought that was a great idea and I really told him that I loved it. Nothing happened to it, don't know why, but anyway. So there's a little.

Story about The Tyranny that could have been. Anyway, my work on Tyranny was very similar to pillars. I did the abilities items, creature attacks, uh, magic spells. Internally these were all called spells, just like pillars, and I just continued my work on those because I was very familiar with that setup, having done most of it for pillars. I did not do the spell crafting UI in Tyranny, but I did support all the underlying Spell components.

So I thought that was a really neat system. It was really cool to be able to make a spell and put together exactly what you wanted and, — and I was very happy to support the work on that — doing that was a lot of work. It was done by Bryson till — I think he was the one in charge of it, um. So yeah, see, this is what happens when I have notes: I forget people's names and I forget exactly who did what. So, anyway, I started Tyranny in, like I said, March of 2015. In late 2015 or early 2016, obsidian started having, uh, late afternoon meetings on new IP and one of the owners asked me if I wanted to come and I said: no, I was really pleased.

Yeah, I'm just not. I have a lot of ideas, I've got all my idea books, but I'm just I don't feel like handing one of my IP ideas over to someone else to create and I don't feel like being a game director. So that was fine, until Anthony Davis, one of the programmers at obsidian, showed up at my door and he said: you really should go to the IP meetings. And I'm like Anthony, I don't want to make one.

He goes: how? How would it hurt to just go? You've got? Permission to go. You can just take an hour off the middle of the day and go sit in the conference room in the corner and listen.

Now, if you know Anthony Davis, he can be very persuasive, but not in a manipulative way, in a very puppy dog kind of way. He's like: just go, so I finally said: okay, I will go to the IP meetings. I went to them, there were some really good IP ideas thrown out, several of which I was like we should really be following up on these. I threw out one myself: um, which was my idea. It'll bubble in a nutshell was: let's put together a game that feels like fantasy and then it turns into science fiction. Um.

All of these were shot down, every single one: boom. And so I finally stopped going to those meetings and Anthony came. Back and he could go to the meetings and I'm like, nope.

And here's why people gave really good ideas. They were shot down for no good reason. There was no objective critique.

You have a whole video on how to give good critique. No good critique was given, basically, the person gave a good idea and they were told, yeah, no. And I was like I've had enough with this.

Finally, one of the owners came to me and said, well, they kind of had an idea for a game and they were hoping that someone would come up with a setting or IP idea that their idea would fit within, but that hadn't happened. And I'm like, well then, you should have been honest with people and said what you were looking for. That was when they said, well, what if we told you the idea and you could be the game director?

On it? And I said, no, I mean, this was four years after carbine and I was. I was done. I was absolutely done with being a game director.

Watch that video. I'm not repeating it here, but I was done. Let's just say that not only did, uh, one or two of the owners talk to me and Anthony, but when they asked me, like why I didn't want to do it, one of the things I said was that what I, what I really liked making IPS. That was when I did it with Leonard and Jason, and I really liked that back and forth of being able to work with someone. They agreed and we contacted them.

Leonard was interested, even though he was a blizzard. They literally hired him in April of 2016. So I was still doing some code on Tyranny, but I was now doing design work with Leonard, on the game that would become The Outer Worlds. I would say in April, May, June, I was a lot more out of Worlds than Tyranny, but Tyranny was supposed to ship that fall and so by mid-summer at the latest, I swung back onto Tyranny. Tyranny in fact had a bit of a Crunch at the end and I participated in that. That was just. It was a, it was.

It was not reasonable to expect someone to pick up all my code and debug it and optimize it. So I went back onto Tyranny and, if that sounds familiar, this is exactly what happened with pillars in South Park. I went from South Park to pillars and back to South Park and then back to pillars. Here I went from Tyranny to The Outer Worlds and then back to Tyranny, finished it that came out in 2016. And then, interestingly, I did.

Go back to The Outer Worlds but I also started on dead fire. There were some ideas they had for the sequeled pillars that they wanted to get a few spells done, and I worked on that. I I worked on the dead fire spouse system. Then that transferred to actually the program I mentioned, Brian McIntosh, and I worked with him a little bit on like handshaking, getting my code handed off to him. I also told him — I gave him a list of things like: this is the immediate thing I would have done, given some down time.

Here's how I would have refactored my code, because when code gets shipped and you're so desperate at the end and you're putting a lot of things in and you're fixing stuff, it becomes a little messy and I wanted to refactor it to be cleaner. Told him what I was going to do with that. I also remember telling him: you know, I would have loved to make turn-based pillars turn based, and we talked about how to do that, and Brian is the one who eventually made the turn-based mode for pillars 2. So thank him so, but after starting that dead fire spell in late fall 2016, I went right back and so Tyranny's out. Tyranny came out in November.

I went right back onto The Outer Worlds. So I think even by the time The Outer Worlds or by the time Tyranny hit the Shelf, I had finished the crunch on Tyranny, done some work on dead fire spells and then was back on The Outer Worlds. So I just realized a lot of me talking here wasn't even about Tyranny, but that's what you have to understand. I worked on Tierney as a senior programmer, primarily doing the spouse support. I'd occasionally have design chats with, originally, Chris Avellone. And then Brian Hines, and that was about it, and I even kind of slipped away before it even shipped to start the The Outer Worlds. But then I came back to help fix it and get it shipped. So that was pretty much my entire involvement in Tierney. So that's why I can't even answer a lot of Tyranny questions.

My answer would be: I don't know somebody else did that and my notes don't have exactly who. So I haven't been avoiding talking about South Park and pillars and Tyranny. It's just my involvement in them was less than a lot of my other games and I don't have notes on it and that's This is the best I can do. So that's most of what I remember about working on Tyranny. Um, I hope that puts it into perspective anyway, um, for all people asked for a Tyranny of. Rio, I hope this is what you wanted.

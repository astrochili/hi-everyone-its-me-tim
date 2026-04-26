+++
title = "How Fallout was made SPECIAL"
date = "2023-05-11"
id = "kgPwfHXiBjw"
status = "transcript"
tags = ["Fallout", "Character Systems"]
summary = "Hi everyone. It's me, Tim. Today I want to talk about how, in just two weeks, right near the end, about four or five months before Fallout shipped, we replaced gurps with special."
references = []
+++

Hi everyone. It's me, Tim. Today I want to talk about how, in just two weeks, right near the end, about four or five months before Fallout shipped, we replaced gurps with special.

Now this isn't going to be a video about why we had to do that — that's another video, maybe, if I ever feel like talking about that. But what I want to talk about is: have we managed to replace such an integral part of what you would think would be a game so quickly? And there's really two reasons for that that I'll get into. But they were that Chris Taylor, our lead designer, already had several Homebrew systems and they had one that looked really good and I'll tell you how, what that was and how we integrated it. And then the other reason we could replace, uh, the system mechanics so quickly was the nature of how Fallout came to be, and I know — I've talked and you may have read other places, that Fallout started very small, uh, just me, and then I was really championing Gertz. So let me talk about both of those.

First, the engine. I made several different engines, just playing around a lot of my own time. I made a voxel engine. You know 3D pixels — they were really hot in the 90s. I made a 3D engine and it was awful. And then John Price, programmer, came on board and made a really awesome 3D engine for the Star Trek games. So I went with the Sprite engine that I made.

At the same time I had started playing Gertz, before I even came to interplay. I played back in grad school, so by the time I started interplay it had been four years and — and I had made because I played group space a lot — I had made a tool called the gerp star system generator. You can probably still find it out there. It would generate a sector of the Galaxy according to rules in the Gert space rulebook and you could click on the different stars in the UI and it would tell you what the planets were. If you click on, each planet would tell you information about that and I had fun making that. So when I started introducing gurps to fellow players — and I've told some of those stories in my other video about why I like flawed characters — we would play all kinds of different groups.

That's what was the advantage of groups. We would play groups fantasy and group space and groups time travel. We would. We had one campaign where I said they could use any of the books they wanted. I call that groups everything and that was a hilarious campaign. To talk about that. At some point Chris and Taylor and Scott everetts had two of.

The funniest characters. I also tried playing one where you weren't allowed to use anything: no magic, no Sonics, and only the very most rudimentary skills and advantages and disadvantages from the basic set. We call that groups: nothing.

While I was doing all this, other groups started spinning up and playing their own sessions of groups and they said: you know what the character editor or the character creation is a little complex, especially when you had to tell people you can use these advantages but not these, and these skills but not these. So what I did was I made eight groups character editor and to help support all these different group sessions that were going on, it was completely modular. So the skills, the advantages, the disadvantages were all done in text modules that anyone could edit and you could. When you started at the editor, you're like I'm going to use these files for advantages and disadvantages and skills. And then I even made attributes into one because I'm like, well, everything else has a module, I'll just make attributes module and be done with it.

People loved it, there were a whole bunch of campaigns going on. Scott Campbell, the original lead designer Fallout, made a group vehicle editor. That's how in the groups we were. So that was probably around 92- 93. So Flash Forward three or four years. I've made Fallout, we made Fallout with the Sprite engine. Erps was put into Fallout as modules.

So in the middle of the combat system it would say: this guy attacked this guy, what's his chance to hit? And would say, well, how far away are they, what item are they using, what are their skills, attributes, whatever. But that was all tucked away in library calls. So when the call came to like, hey, we may be replacing gurps, how long would it take to do this? I met with Chris and Chris Taylor said: I have a really cool system I want to talk to you about.

Give me two days, so I spent those two days looking at the code and how everything was isolated into the libraries and I assisted that a little. I found a few things that weren't quite so isolated and I tried to clean those up. I thought most of them. I probably didn't get all of them.

Then a couple days later, Chris came to my office and he presented his system and I remember the. It was attributes, traits and skills. The attributes were strength, perception, endurance, charisma, intelligence and Agility was everything but luck. It was specia. Traits were a combination of advantages and disadvantages and that solved a problem we were currently having where, when you gm'd, a group's campaign, you would often tell players they weren't allowed to take certain disadvantages together, like if you were already blind, you couldn't take colorblindness in the.

In our Fallout version, we had to mark them as exclude, mutually exclusive. Sometimes, if you had these two, then you couldn't take this one. What we ended up doing was just, you know, Chris's idea of putting advantages and disadvantages together in a trait got rid of any need for that. You just took no trade or one trade or two trades, and you were done, and the skills were really good. Selection of skills that we could easily just redirect the, calls, from going to groups modules to going into this new game system, skill module. My suggestion at the time, though, is I said I really, really want luck because, uh, I had some really good experiences with luck, especially in group supers, with. Buying ridiculous luck and phenomenal luck, and so we put that in. We did two things: we sent it up the chain and we presented it to the team, the. I don't know if we got any feedback from anyone but Brian Fargo, but his suggestion and all he said was: when you go up a level in this new system, I don't think it's enough just to buy skills. I want to be able to buy something else. And Chris Wynn, why? What if we put back in sort of advantages? They were quite the same, but because there are no disadvantages, there was nothing we had to worry about balancing there, and also we're restricting it to you buy it every third level.

Chris made a bunch of perk trees. They were really good. Brian loved it, when we presented the system to the team, they really liked it. Uh, they thought it saw.

Some other problems we were having that I won't get into here, but some things we weren't sure how to solve that were coming up and testing. However, after the meeting, one of the team members, Jason swinn, came up to me and he goes: you know, Tim, you presented it and you called it a slips, the first letter of all the attributes. I was looking at that and I — I think you could rearrange them into a better word, special — and I was like: oh, Jason, I don't know. You know, special has some negative connotations.

Let me think about it I don't have to tell you. By the next day I was like: okay, Ace looked is out, specials in and the rest is history. And if there's two lessons to learn from this, it is that Chris Taylor did a whole bunch of heavy lifting, making a whole new system.

In days based on its Homebrew system, and thank goodness for modular programming — it saved the day. So that's the story of Fallout special system. I still call it a slips occasionally.

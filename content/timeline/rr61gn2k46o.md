+++
title = "Technological Evolution"
date = "2024-03-26"
id = "rr61gn2k46o"
status = "transcript"
tags = ["Game Industry"]
summary = "Hi everyone. It's me, Tim. Today I want to talk about technological Evolution."
references = ["Iw3bCdIvAj0"]
+++

Hi everyone. It's me, Tim. Today I want to talk about technological Evolution.

Specifically, I'm going to try to answer a question from bavid deckham 411, who asks: what was your experience with the technological Evolution we've gone through during your time making and playing games? Was it ever a source of stress or were you excited to keep up? I'll give you the tldw: it was exciting and stressful it's.

I'll have to go back a long time ago to explain it, but, like, even when I was a kid, we started getting little handheld games like kico, football and things like that. And then suddenly there was a pong unit out which you hooked up to the TV and then within a year or two, there was a console — the first console, Atari VCS, which took cartridges and you're like whoa, that's it started playing games that looked like they were in the arcade and you were like whoa, this is crazy. You know. That led to all kinds of things: cico, vision and television, Nintendo, just. Things just kept coming and coming.

As a consumer it's, and coming and coming as a consumer, it's fun. But also you had to realize that you could buy something and then literally the next year, sometimes 6 months later, it was obsolete. That really hit the stride with PCS. You would buy a PC and it would be obsolete within months as a better sound card or video card or processor or monitor came out.

So I'm not going to talk about that side. I'm not talking about the consumer side.

I'm going to talk about my experience, starting in 1981, of trying to make games where your target was constantly shifting. And this is the thing I've always told people: the huge difference between writing a book or making a movie or making a TV show is the pace of technological ch change in those don't h a candle to computer. I mean yes. They've developed new cameras and different lighting um Solutions and better microphones, but in general directing is the same now as it was maybe 20 years ago, 40 years ago.

That's not how it works in computer games. Every time something changed technologically it would make old games not work. It would make, it would open up a plethora of choices you could make for new games, way different than movies. Now have color, movies now have sound.

We're talking. You couldn't do realistic Graphics, now you can. How realistic, you know, you can add in cutcenes how many.

Well, now we have cd ROMs. You can add a ton. You have space for way more data. We can make higher resolution art. We can just it expanded exponentially at felt, like every year, and it was keep up or die. So let me walk through some of these choices I made. So the very first game I made, um that I started around 883 and it shipped in ' 86, was Grand Slam Bridge.

It may look like it's graphical, but this is all text based. This was put together in a text mode using asy characters that already existed. We didn't have to Define any, so because of this it worked on any PC. It still works.

Was it very interesting way of doing a game now? I then went off to grad school for a few years and when I dove back in to making games in 91 with B tail construction set, suddenly I was doing a game in VGA and VGA was the new hot thing in a sense, because when we did baril construction set, we had to put in support for the old mode, EGA and the even older mode, CGA. So VGA for 32200 resolution gave us 256 colors, but EGA. Only gave us 16, CGA only gave us four, and those four were predefined.

It was black, white, magenta and some purpley color — I don't remember what it was, or maybe it was magenta and move — and there were two different CGA modes. You either got black, white and these two colors or black and white and these two colors predefined. So good luck making Graphics you want in a low resolution where you can't even pick the colors you want.

Now, by the time I started Fallout in '94 — in early 94 in fact — I had to work this out exactly when I started working on it, probably January 94, because yes, I'm putting together a timeline for many reasons, but the very first meeting with Steve Jackson games to talk about gerps for the new game was in March 994 and that's where I can put a pin in it I know. The game was definitely in development by March of 94. It was just me, no one else would be assigned to it until August of that year. But I can say for sure in March 94, but probably a month or two earlier, by January or February, Fallout had begun. Development by that time.

VGA — this is what — three years after Bale, because I did Rags to Riches in between — by now we're up to 640480 resolution with 256 colors. That was a huge leap up. That's um almost five times. It's between four and five times the resolution of 32200. But to do this mode, which is called super VGA, you had to bank switch because the PC could only access 64k of memory and that mode required four and a half times that much memory. So you had to bank switch, there were the first few scan lines would be on One bank and then the next set of scan lines would be on the next bank and the next set of scan lines to be on the next bank. So depending where vertically on the screen you were drawing a pixel, you had to tell the video card switch to this bank.

Now I'm going to write into you. When we did Fallout, every video card Bank switched differently and you had to learn that and do it in assembly. No option, which meant you had to ask the um, the consumer: what video card do you have?

Hope they knew and sometimes it was different. It was is: do you have a tried at 9600 chipset a? Do you have a tried at 9600 chipset B? Do you have a tried at 9600 chipset C?

They Bank switch differently, if you didn't know, you could ask it to autod detect, which was not super 100% reliable, or you. Could just ask them to guess and we're say: guess something, I'm going to try to display a screen. Pray you don't crash, and if they could see something, then you could move on.

Lu IL Vasa came out. Vasa was the video entertainment standards Association.

I think you can look it up. Anyway, Vasa made things easier, but it didn't come out early enough for Fallout to fully take advantage of it. We shipped with a super VGA Vasa driver and we recommended that people download one if this one wasn't appropriate for you. So then you could just say: I'm in Vasa, go ahead and play. That worked better than trying to guess. But still also we discovered there was.

Fallout was the one and only Mac game I made, because when a new Mac OS would come out all the old software would break. There was no backwards compati compatibility and apple. Cared very little about games. I could do a whole video about that. I'm not going to, because I don't really care about Apple. I mean, I have't iPhone. I love it, but I'm going to show as much interest in apple as Apple ever showed in my games or the game industry, which is very little. But whenever a mac o new Mac OS would come out, it would in invalidate the game. In fact, like I said in another video, Once people can play Fallout Easier by playing the windows version on a Mac under an emulator or a partition where you've, where you've installed something to run a Windows like OS, better and easier than trying to get the Mac version running on a Mac.

So by the time Arcanum came out in 2001, we had up the resolution to 800 x 600, still 256 colors, but it was Vasa. Now, and Vasa made everything easier. Vasa cards usually shipped with a Vasa compliant driver, meaning you could just tell the card through a Vasa set of interrupts or API function calls Al. All you need to know is, hey, I want to run 800 x 600, 256 color, and we go, I got you, it's set up, and then, as you wrote um to it, you could just call a Vasa supplied Bank switching routine and it would say: I'll figure out how to switch banks for you. Rock on um.

By then we weren't doing Mac versions because I was like I'm done with this, but the windows and direct and especially directex versions kept updating, literally why we were making the game. New windows would come out, new, directex versions would come out, and it was hard to keep up. Now, yes, Windows had backward compatibility and that helped that.

Let you. Run games. It still lets you today Run games from a long time ago. But it's not perfect. It can be a little janky, it can cause some issues in HUD and um frame rate and things like that, but it works.

However, I'll give you an idea, just when we were making Arcanum, we started on Windows 95 and Windows NT, but then Windows 98 came out and then Windows 98 second edition came out and then Windows 2000 came out and then Windows Mi came out and then, right when we shipped, Windows XP came out. We had to check all of those. You have to check that your game works on all of them and not just does it start but it does its frame rate good, is it stable? Do some of the calls you're making into that version of the oper systems still work? And that was a pain.

Um, by the way, Windows cycled a new version every year. A new version of XP came out every year. For the rest of the time we ran tra — from 98 through — well, the new — the first XP — came out in 2001 — through 2005 when we shut down, there was just a new version of XP every year.

It's hard to keep up with that. But keep in mind I'm just describing making games that are 2D. Temple of Elemental Evil was our first game that had 3D video graphics usage. The backgrounds were still 2D, but the we had a 3D Collision mesh and we had 3D characters. So we had to go through the 3D API on the card and a lot of video cards came, out 3D. They all did 3D slightly differently. You tend to go through direct deex and do it that way, so you had to handle that well. Then, when we did Vampire just a couple years later, every was all 3D, and, yes, we used an engine, um, but everything was 3D. Then you had — it was a learning — a new way of making a game you had to worry about, you know, polygon, count, uh, your texture, sizes, all these things that you didn't worry about on 2D, because that was rendered into Sprites, and then you just had to worry about how big the Sprites were in 3D. You have to worry about a lot of other things as well.

Keep in mind, too, that for the programmers and the level designers, suddenly math is super important. You could probably have gotten by in the video game industry with no math if you were like narrative or even art — nope, not good enough. Trig was probably helping you out there — signs, cosiness, angles — but once you went, 3D — artists, programmers, especially — you had to know linear algebra, you had to know vectors, you had to know matrices and you had to know them well. So that was a huge shift in the industry. Luckily I'd gone to engineering school, so when suddenly people were talking about vectors and quorans, I'm like, yeah, I know that I knew programmers who didn't and they stayed 2D. I don't want to stayed 2D for the rest of his career, for the next 20 years. He just stayed 2D notes. I haven't even touched on languages.

My first game was in SE, um, Grand Sand Bridge. Every game was in C, until vampire, which was in C++. It stayed C++ until my first unity game, pillars of Eternity, which was CP. But then when we did outter worlds and unreal, we were back to C++.

You know I'll do a whole video on that. I could. I've talked for a. Long time. I could talk, I could do a whole video on languages, but let me touch a little on engines, because I do have a video on game engines. Um, I made my own engines from the very beginning in ' 81, all the way through to 2011. I made my own Engine, with one exception, uh, vampire Bloodlines, which was on the source engine and that was in.

That was from what- 2001 to 2004. So then, when I got to obsidian, they had some of their own internal engines that were proprietary. So, just so you know, we made um.

South Park was made on an engine that they had made for do Dungeon Siege 3, even though, You' never, the two games don't look at all alike, but once I did that game and we switched to pillars, then it was on Unity, we were using someone else's engine and unity doesn't give you source code. So you basically did whatever Unity said you could do, and if you couldn't do it you'd ask them. But who knows if it would get done. Then I finally The Outer Worlds. We switched on real whole new engine. You had to learn a whole new way of doing things in different language — C, from the C in unity, and you had to. But you had access to the engine. So if there's something you wanted to do, you could change the engine, but from on you were responsible for that change. Whenever you got an update to the engine, you had to fold your change back in. You had to merge It's the whole thing. Programmers know what I'm talking about, so this has been a long video. Let me just sum up.

Technology, technological Evolution has been going since the first day I was in. This industry in 1981, all the way up through now in 2024. It never ends. You need to accept it and get used to it. For anyone sitting there right now, no, you know, be around forever.

Andre will be around forever. No, it won't, and you're already starting to feel that maybe those things aren't going to be around forever. So new engines will come out. They'll get displaced, they won't keep up or they're change so dramatically from one version to another. You have to relearn everything, so I'm just telling you it never ends. This is both exciting, because you get to learn something new literally all the time. It's also stressful, because you have to learn something new all the time, and I can't think of nobody's really immune to this.

You may think I'll do narrative design. You get more dialogue, now there's voiceover. Now there's lip syncing. These are all. Things that factor into what you're going to do.

There's no escaping it, so my take on it is: embrace it and love it, because that's what this industry is all about — technological Evolution. So I hope that answers your question. Bavid deham- 411.

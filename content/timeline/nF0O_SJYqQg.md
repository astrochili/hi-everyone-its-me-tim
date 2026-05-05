+++
title = "Archiving"
date = "2026-03-23"
id = "nF0O_SJYqQg"
status = "transcript"
tags = ["Game Preservation"]
summary = "I talk about some best practices to archive your game-related assets."
references = ["kbHlwUS7d4k", "GYp00o-sewY"]
+++

Hi everyone. It's me, Tim. Today I want to talk about archiving.

I've archived things for a long time, so I understand the importance of doing it, of tucking away things that you will want to look at later. I've done that for a lot of things. I've talked about my notes on this channel so many times and I I link a video below about my best note takingaking practices, which then links to all the other videos about my notes and even where me taking so many notes probably came from. But I keep a lot of stuff. This shirt is probably 20 years old. But I want to talk about code in spec, specifically because I have kept code for decades.

Arcanum is already a quarter century old. It shipped 25 years ago And I started the code on that three years before that. So I have an a code archive that's 28 years old. So I think I know about archiving things. When I did my video on code comments — and I'll link that below — I mentioned adding changes and dates into comments to code changes you were making, because me, but, many people — I thought that was important.

But many people said: "No, Tim, that's what the source control is for. Use source control for those kind of comments". And yes, when you're doing a commit of source into your source control, you should put comments in about what got changed. But I also think that there's a case, or a set of cases, where you should leave an inline comment too. And that's when, if the change you're making is so important, because either you have to do it a particular way, like we chose this way and here's why, or this other really common way of doing it, which you may think about doing here, will not work. And it can be all kinds of things It could be. Don't do this sort. I've mentioned, like hey, this.

Array is almost always almost sorted. Don't do quicks sort here, or don't call the standard template library, because at the time of we were doing this standard template library sort, an array was implemented this way, which was really inefficient. Leave a comment like that, and here's why archiving: when you archive source code, you will frequently, just archive the source files in their folder structure and write them into some kind of storage.

That's offline and often offsite, and what that means is your source control may not be maintained. And I'll talk about how to maintain that but also why maybe that may be a bad idea. But first of all, let me tell you what I mean by offline and off-site. Offline is things like you don't want it on your computer or on a network drive somewhere you're going to write it off to a C.

CD, DVD, some kind of optical storage or even putting it up in cloud storage. You know, maybe put or you put on a thumb drive or something and then offsite. Well, that includes cloud storage, but you also may want to take that thing you just wrote to and not keep it in your office.

I've worked at offices that got broken into. Um an early Obsidian office, there was a car drove into the side of it and, uh, I don't know if it caused a fire or the sprinklers went off, but there was a lot of damage.

So you never know what's going to happen physically at your site. So you want to archive things, so they're offline and offsite.

Now a lot of people said "Oh, just source control will be there". Source control might change And this is something you have to realize. I'm not talking about wanting to store things for a couple months or a couple years, I'm talking about decades.

The source control you use may switch formats and then the format becomes unreadable. They may even go out of business. So that source control isn't there anymore for you to use.

I have, uh, had run into this problem with spreadsheets. I like to keep a lot of spreadsheets around of different things I've done. I have all my finances to the penny of what I've spent, what I've made, what I've earned and what I've spent since 1991..

But guess what? Those started out as Lotus 123 spreadsheets. How many of you listening to me know what Lotus 123 is? How many of you know how to load a Lotus 123 spreadsheet?

Even if I had kept the executable, I'm not even sure would run in DOSBox. So that's kind of a scary thing to think about, right? However? At one point I started using Excel and Excel could import Lotus 123. So I did.

Over the years, Excel has changed its format as well. They used to write out um, a particular format, and then they updated it and I think it had an X on the end or whatever, but it I had to read in the old spreadsheets and write them out. In the new format I keep the old ones and now I have the new ones, and also those go in the cloud as well. Now you may be thinking, "Hey, I'll just store it in source control and then put the source control executable in there too" Well, that's great. I hope that executable will still run for you. Windows has backward compatibility and it probably will work, even if, like I said, you have to bring up a DOSBox or, you know, run it under if you look. At the properties, they often have: run this as a Windows 7 app or run it as a Windows 10 app.

But Apple, I'm looking at you. Every time Apple puts out a new OS, their old stuff just doesn't work. So good luck trying to run an executable from 10, 20 years ago to recover your source control. So I highly recommend not storing it in that source control format. And remember again, I'm talking about storage. You're trying to store for the years and the decades here. So three things I think you should think about when you're planning to do an archive. First one: what to store? What are you actually going to put in the archive?

My code archives can be pretty small because it's text and it compresses really well. Art archives are not. The art archives for Arcanum were so large they didn't fit on anything.

We had at the time. They wouldn't go on a CD or a DVD disc, They would have had to be spread across multiple discs And instead we put them on that digital audio tape And now we don't have any way of reading those. Design compresses well, Sound compresses pretty well. There are formats that change, though. I mean we may have had waves or raws or AUGs or MP3s, but usually you can. You can recover those. One thing you may want to tuck away is some of the tools used to create the assets used in the game. If you had a tool for making dialogue or a tool for making maps, you may want to tuck that away, Not just as the ex running executable, but you probably also want to run away, tuck away the source code used to make those tools. I know when I archived — archived Arcanum, I also archived the tools for like world ed and a few other things we had, because I knew I may need to recreate that tool With art.

You also don't want to store the final art. You want to store the basic art, like the model, and then separately the textures, because you may want to upscale those later and you can't do that from the final rendered. Um, if you render it into a sprite or if you just store the final model format, you may not be able to backward recover all those things. So you want to store all those things as separate elements. So that's the what to store, now, how to store it. Do you want to compress it? What archive format are you going to pick? Zip, Do you think zip will be around?

Do you want to use your own compression? I've done that as well. Do you want? To store it optically? Do you want to put it on an external hard drive that you can put in a closet somewhere? Do you want to put it on a thumb drive?

Those do have lifespans, though. What you want to think of is what will be the most usable to me in a few decades. For me, that's been optical storage and flash storage and a couple external hard drives here and there. And then, finally, where do you store it? You may think I throw it in my desk drawer. Well, you may also want to think about putting something lockable — If not a lockable desk drawer, a safe, maybe a fireproof safe.

Remember, I've been in offices that have gotten broken into. I've heard of offices that had fires.

You may want to put it in the safe. You may also want to just go. You know what? I don't want it, here. I'll put it up in the cloud.

A lot of my stuff, my notes, even though they were physical written notes, I ran them through an optical character reader, converted them to digital and threw them up in the cloud. So now my notes are safe in the sense of I don't have to worry if my computer, my hard drive, explodes or my CD drive backup of those notes um, becomes unreadable or the physical notes themselves get lost in a move.

Yeah, I had a couple things go missing in the move. I think they didn't get packed or they fell out of a box or they were in among the packing paper or the bubble wrap and I didn't get them out of the back of the box. But a few things from that bookcase that were up in Seattle aren't here.

Anyway, I think, if you think of the what to store, how to store it and where to store it, that'll do you well. But remember, don't just think about: oh, I may need this in a few months, You may want this in a few years, or, like me, you may want this in a few decades. Think about how you will get that. Anyway, I hope this video helps future you.

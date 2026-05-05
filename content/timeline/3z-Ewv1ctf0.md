+++
title = "The \"Best\" OS For Game Development"
date = "2024-02-26"
id = "3z-Ewv1ctf0"
status = "transcript"
tags = ["Programming", "Game Development"]
summary = "I talk about the best operating system to make games for (not necessarily the best one to work in or even the best one overall)."
references = ["hZEosFcqmcU"]
+++

Hi everyone. It's me, Tim. And today I want to talk about the best operating system to make games.

For now. This is an answer to the question that Romo bomb asked, which is: hey, Tim, can you please talk about the best OS to use, in your experience, for programming and designing? Does it even matter for the user in those professional grounds? Yes, but I'm not going to talk about what I think the best one is to be doing that work in, because that's subjective. Some people like Mac OS, some people like Windows, some people like Linux and there's a million osses out there. I'm going to answer in terms of pure practicality.

Um, in other words, what should you know how to program in to make games? And that is Windows, and the short of it is: if you know Windows programming, that gets you access to the PC market and the similar Xbox Market, which is a big chunk of the market and has been for decades. Um, all you have to. Really do is additionally learn PlayStation and you've got a most of the market right there now. That also presupposes that you're going to learn subtype of C language so you can know C++ and C. But I'm only going to talk about os's now. You did say in my experience, so let me walk you through all the os's I've used and why they didn't make the cut.

Um, so way back in the late '70s I started on the Atari. I couldn't remember what the name of the OS was, so I looked it up in Wikipedia, listed as default OS. I don't think they called it anything, it was just. Or they called it dos, which is weird because that became what the IBM one was called. But under Wikipedia or under the Atari, I learned under their OS to program basic and assembly, and that let me do a lot of.

Stuff right there. I basically did things in basic, except for the things that had to be an assembly, either because that was the only way to access it, or if you really needed speed assembly. Uh, their play missile Graphics were a good example of you really want to do that in assembly. Then, very shortly after that, um, I jumped into Doss because I got a job at a game company when I was 16 and I was doing tools for them on the Atari. But they were going to make a game which turned out to be Grandam bridge on the PC under Doss. So I quickly learned Doss. We made Grandam Bridge Under dos, and this is where I learned an interesting thing about Doss: you can do anything you want, but you have to do everything.

Everything you want. You have to do the things you don't want to do, basically. It doesn't really give you much.

Oh, you want a pop-up window code, everything about that from scratch. Oh, you want a new font, do it by hand It's an interesting thing that Doss was so basic. Basically, it's a very thin layer over just what the uh chips on that motherboard provide to you, very thin layer, so you have to do everything. I went off to college while I was working on Grandin bridge and the college I went to, University of Virginia used a, an OS called Prime OS.

P? R I m?

O looks like Primos the band or Primus or whatever, but it's pronounced Primos, and it was on their Prime computers. So while I was in college — this was in the mid 80s — I learned a lot of different flavors of Unix um, which is what Primos was kind of like. It was also a weird mixture, of Doss and Unix, but it was more like Unix and we used those. They were basically micro computers hooked up to a Mainframe. Because I was at an engineering school with getting a computer science degree, in addition to learning all the hardware stuff, they tried to teach us a wide variety of languages. So in addition to C, which I already knew, in fact I could tell a whole story about something that happened to me in a class there.

I'll save that for another video. I also learned Pascal, which I had already kind of learned in high school, from the one computer science class my high school taught. We also learned prologue, snowball, Fortran, lisp, just a wide varray of languages, and that's where we learn different languages for different purposes. You going to do a lot of string processing, snowball. You want to do a lot of scientific calculations, Fortran.

So different languages supported different things when I went on to grad school. Straight from college I went to grad school in California at University of California, Irvine in the late ' 80s, early '90s. They were all Unix now I was. It wasn't that big of a jump for me — me because I'd been using Primos, which was a kind of a Unix flavor, but they used real Unix. I loved it.

Unix provided so many cool accessors to functionality in the OS and it was really fun. It really supported my hacky flavors. I would do fun things like send messages to my friends and have it look like one of them. I sent them a message: um from God in heaven, um, and he replied: Satan from hell it was. It was funny things you could do. But one thing I really loved about it was it had features that you still don't see in a lot of modern os's, one of them.

I'll give you a quick example how it handled files and directories. So a directory was just a collection of files, but files weren't just. Here's a bunch of data, oh, and we're going to label it. What files did is? They pointed to what was called an? Uh, internal node, an iode, and the iode contained all the information about. Here's the file. Here's all the sectors that store the data. Here's how they link together. The reason that was important was you could have two files in two different directories that pointed to the same iode, so they pointed to the same file, which means you open one of them and edit it, close it. When you open the other one, it's got the edits.

It was like a. It's like Windows. Um, what do they call it uh. When you make a link, a shortcut, a Windows shortcut, but it's not the same, because both of those files are really the file and what I mean by that is edit either of them. The file gets changed, if you delete one, the other one remains. Basically the inode, knows everybody who's pointing to it and as long as that number is greater than one, it doesn't delete the file. So if you want that file really deleted, you have to go to all the places that have that file as an inode and delete those files. What it meant was you could have, let's say, you wanted to store a picture. This is something that I really wish Windows did.

Let's say I had a picture, a family photo. I want to store that under Cane family, but since all my siblings are in it, I would also love that photo stored under all five siblings. Under windows I would have to make six copies of that photo, one for the thec folder and then one for each sibling folder, or use shortcuts, but the shortcuts aren't really the file.

What I love about how Unix would handle it is it would. There would be six files of that photo, but they're all the same photo. Edit one. They're all edited.

Um, try to delete. Delete it from one folder. It's not deleted, from the others, It's just a really nice way of thinking of files and it's how I thought of files. And then when i' go back to Doss or Windows, I'd be like: uh, by the way, speaking of back to Doss, when I went to work at interplay in the early 90s, back to Doss, I was at interplay pre — windows and one of the things I did was when I wrote ganal and I've got a whole video about ganol — I made a wrapper for all the stuff I wanted to do in Doss, including some things that I built on top of Doss like popup windows and things, and then I just said that's ganol, I'm going to code for ganol so someone else could write the windows version, and someone did, and someone else could write the Mac version and someone did. But we were just coding Fallout in ganal and it worked on all those other ones and I really like that.

Also, a lot of our — the early computers that um interplay bought to do rendering on were Sun computers and they ran irx, which was a very, very um strongly fa flavored version of Unix, and I knew Unix. So I was often brought in when the 3D Pro artists had a had a problem, like hey, I can't get this to work. Or I'm shut out of my account or whatever. I would go in and fix that. So while I was coding technically for Doss and windows, I was doing my own stuff for ganal and occasionally going in and do Unix stuff, now because when.

Why did I make all that g, all stuff? Because Windows ain't great. I'm not going to sit here and defend Windows.

Sometimes it's really hard to use it and it's really hard to code for. But I will tell you two nice, things about it is like Doss: if you can conceive of what you want to do, you can probably do it under windows and tons of backward compatibility. I'm still playing games from 30 years ago on Windows. I can't do that with apple.

Let me talk about that. I only made one game for the apple and that was Fallout, and I really didn't make it for that. I made it for ganal, and ganal had a Mac OS version. The reason for that is: in my career I haven't seen that Apple really cares in any way about games. They're there, they recognize them, they occasionally make a half-hearted effort, like gam sprockets, which then disappears, but they don't really care about them.

It's not. It's not. I can't see that being part of a board meeting going.

How do we expand our, game stuff? Yeah, because of um iPhone, there's a lot of G Apple games now, but I don't anything. They care about that, and the one of the problems is everything has to be done Apple's way and if you don't do it their way, screw you some. Sometimes you can't even do it, when we made Fallout, we had to process art files and we had thousands of them and they were processed separately for Doss, windows and PC, although I think Doss and windows were processed the same and then they were processed separately for Mac.

Well, guess what? For Windows, we WR a simple batch file that simply said: grab, go to this folder, grab star, do whatever the extension was for the art files and process them through this other application that had a console command version, whoa. Doing that on the Mac was a pain in the butt. I think we needed to do a third party batch file system and find something that accepted commands being given to it.

The biggest thing I remember was in this is in the mid90s — you couldn't rope. If you wanted to collect a bunch of files, you had to rope them. You know where. You slid the mouse over it and grabbed them all.

It wouldn't rope thousands. It stopped after, I think, 256, so you had to rope them in chunks, even from the same directory. The Mac guy started complaining that we had a thousand folders in one directory and I said they all belong there.

They're all one thing. These are all the art files Associated for a map. And he was like you shouldn't put more than 26.

I'm like that was, by the way, just the very beginning of Apple. People love to tell you if it's not something Apple supports, that you're doing it wrong and it's a weird thing. Um, my first iPhone couldn't send a text to multiple recipients. A friend of mine who's a Big Apple guy told me that wasn't a big deal, even though he was on my weekly dinner text that I sent out in the evening going hey, where we going to go eat, and I couldn't send those.

There were like 12 people on that. He said we'll send them individually, and I'm like, and when one person responds, hey, I don't want to do pizza this week, can we switch to you know Chinese or something, and I'm like I'm not sending 12 messages out, and when one person has a change, taking that and resending it out to 12, I said I'd rather just not be in charge of this anymore. And it was stupid because Android did support that from the very beginning. It was a weird. It's a weird fanaticism and it just drives me bonkers.

Um, anyway, that fall after Fallout, I didn't do anything on Apple anymore, so I don't really know what it's like to code on there. I know people like using it and I get why they do. It's a very consistent interface. It's very easy to use, easier than Windows, but I think what I can tell you. I will sum up after.

Four decades Windows W, it's just one. I used it the most in my career. It still is probably what I would use the most. It has the most games for it, especially if you include Xbox. If I was going to pick a runner up, it still wouldn't be Mac OS, it would probably be Unix or some flavor of it, Linux or something like that.

It's what's in the steam deck. You can run Windows games under Linux and so I'd probably pick that as my runner up. But right now, if you want to be a programmer and you want the most options on where to work and what games to work on, I think you got to go Windows as your OS.

I'm sure people will disagree. I'd love to hear the reasons why, but those are my reasons why and anyway I hope this answered your question, Romeo bomb.

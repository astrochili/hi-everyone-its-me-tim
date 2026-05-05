+++
title = "Min Specs And Ratings"
date = "2024-10-03"
id = "zN-mq4xh55A"
status = "transcript"
tags = ["Production"]
summary = "I talk about the process for determining a game's minimum (and recommended) specification, as well as its rating."
references = ["hZEosFcqmcU", "fHUAFYDzN3U", "AH0jo26TQ_c", "NfBcWu22wIE", "vQj5rJry4Pw"]
+++

Hi everyone. It's me, Tim. Today I want to talk about game minimum specifications and ratings.

This comes from a question from suin, who asks: how do games get their system requirements? Since Tim's a programmer, I'd imagine understanding the system is pretty important. But is determining the requirements part of the programmer's job, or QA, or marketing, or the producer? How much time you spent figuring that out? And is a game designed for a spec early on? For example, our game has to run on 480p and 128 Mega of Ram, or at the end, when the project is finalized, when everything that's going in is in and the minimum is then gauged.

Also ESRB, since it fits with the on the box information. Okay, that's a good set of questions. Um, it's a lot of questions. Um, and again, this Falls in that box of. It would never have recur to me to talk about this, because this is just one of those things that's always there.

It's my. I'm a fish swimming in water, so I'm not really aware of the water.

Minimum specs ratings: they always been around, it's just a thing you do and it's one of those things that I think modern game engines have made that a little easier because the engine itself kind of has a mpec and if you're not doing anything too crazy, your mspec is the engine's Ms speec. But that's not how it used to be. So let's talk about how that works.

Let me talk about Min specs first, and from I'll also talk about um recommended specs, because that's related, and then I'll talk about ratings. So minimum specifications: this is something that production is kind of in charge of but doesn't decide. It kind of goes through this Loop.

The Publishers will frequently ask for a minimum spec Target based on what common equipment is out there, like they don't want their sales reduced too much if. Your minimum spec is so high that people would have to go out and buy a new computer to play it. This was really important uh, 20 years ago when new stuff was coming out all the time — video cards, sound cards, uh, hard drive sizes — this uh one, and a quarter floppies went to 1.44, which went to CD ROMs, which went to DVD. This was a big deal.

Usually this is negotiated a little bit. I'm not usually involved in this.

They say what they want Min speec. You know we're like: okay, we're try to Target that. When you're making the game, programmers are usually asked what they think the Min speec will be, or just keep track of what they're doing and producers will monitor this things. These are usually things like: uh, low-end C, what's the lowest end CPU? Uh, how much RAM do you need? Uh, what kind of GPU do you need?

Um, this used to include sound card. It doesn't anymore. It's not tracked that closely. It's kind of just this thing that's always in the back of your head about H, how much memory am I using? What resolution is this going to be displayed in things like that?

Just to give you an idea of what that was like, back in the 90s, when I was making Fallout, I had already written the underlying Library called ganal that could support a bunch of different resolutions. Now for Fallout, we decided — and by we I mean me and the lead artist and actually all the artists, the — that it was going to be super VGA, which meant 640, 480, 256 color. That meant it needed a card that could run super VGA, and we used something called a Vasa driver, my previous game, Rags to Riches. I had to detect what video card you were using and determine how to set up that super VGA mode for Fallout.

We just said nope, Vasa drivers are common. You just need a Vasa driver installed. Fallout will be looking for Vasa driver if you don't have a Vasa driver here where you can go to download one. Now there was a very brief, narrow, tiny window where I remember talking to marketing about whether or not Fallout could be made VGA, and there were two ways to do that. It could either be reduced from 640480 256 color to 32200 256 color or to 640480 16 color.

Both of those had issues. The 32200 was too low res, there was no way to read any of the text in the game, which meant all anything that had text would have to be made a lot bigger with less text in it. We really couldn't go that way, so then I looked at 640, 4816 color and even I could see that didn't look right and my color blindness. So what saved me was I know I've talked about Diablo came along and suddenly people in marketing were like why can't we be like Diablo, why can't be real time, why can't we have multiplayer modes? And I was finally had to go: okay, I'll do that, here's the extra money and time I need.

And they went away. This time Diablo saved me. I pointed to Diablo, which had already come out the year before, and said: they're super VGA, they're 640, 480, 256 color. I think we're good, and everybody just kind of nodded and that was the last time it ever came up. So the so I talked about Publishers.

Talk about them in spec, govern, follow it or keep an eye on it. QA is what actually tests it at some point. In QA — and hopefully they do not wait until the end, a good QA lead will ask for the minimum spec, probably about halfway through development. Get a minimum spec machine set up in their office and maybe not all the time, but maybe once a week. Make one of the QA testers play on the minim minimum spec and just report.

Report back like: what was your frame rate? Uh, was everything? Uh, because you may have to move the some sliders down on things to make it run. Um, what that means is you may have to like, adjust the lighting, antialising, shadowing, you may have to turn those things off. Does it still look acceptable? What was your frame rate? Was it playable?

Those kind of things, that Loop of hey publisher, this is what we're looking at. Hey, programmers, what do you think is going on? Hey, QA, how are the test? Results? Which is monitored by someone in production. A producer will be doing This Loop is often followed so that, as the game is being developed, you make you make sure that the performance is pretty good on the minimum spec. That means good frame rate at a decent resolution, with some stuff turned off. Now, associated with that, they're usually keeping a set of recommended specs. The recommended specs are okay. These are the minimum specs. You — we don't recommend that you run it and we don't guarantee it will even run if you don't have these minimum specs. What we think you should have are these recommended specs. The target is this has a great frame rate with all of these really cool options turned on. B. It's our way of saying: if you want this game and it's a absolute visual audio, and feel best, this is what you need. Again, this is something that that goes through the pub programmer QA Loop, monitored by producer. Okay, the other, the third question, or the second question, but I made it the third because I wanted to talk about recommended spec — was the rating? Now in the US that's called the ESRB, which stands for the entertainment software rating board. Didn't used to exist, now. That's thing where it says t or M. In Europe it's called Peggy for the pan European game information. They do ratings, and in Australia it's the ACB, the Australian classification board. All of these look for different things, which is insane it's. I talked about this in the localization video.

Sometimes boobies are okay, sometimes they're not. Sometimes blood is okay, sometimes it's not. Sometimes you can have bones and flesh, sometimes you can't. Sometimes you can swear, sometimes you can't. Sometimes you can have cigarettes, sometimes you can't.

It's, just usually the publisher tells you what rating they want you to Target, because this is different in different countries. This means you have to do one of two things: you either don't include things that the most strict country says you can't have, or you make it easy to remove — usually, like cinematics, are easy to remove. If you have a creature, you can make an alternative model and just go: oh, I'm playing in this country. Use this model instead, if there's words, you can make a file of the words they don't allow and just get rid of them. So when it shows up in text it will be replaced with. You know, pound sign squigglies, if it's verbally said, it can just cut out the audio. This can lead to some very funny things. If you played Stick of Truth, you know that there were multiple scenes. I think it ended up. Being seven different scenes — that were cut out in different countries. I know it was cut out in Europe and in Australia.

There were things like the anal probe — uh, there was an abortion in there. These things all appeared in the North American version, but they were heavily censored in the other countries, usually by taking that part of the game and they just blacked out the screen or put up — I think they put up a funny picture. I think in Australia it was a koala crying and it was basically You — that's what you got to see. Sometimes you could hear it, sometimes you couldn't even hear it. Sometimes the sound was turned off too and it was just in Tech. Say, this is what happened, Boom.

At some point during your game development, the a form has to be filled out for what those different boards usually prod producers fill them. Out and then they submit a working version of the game, and the board comes back and says this is what we think the rating is. You ask for a rating and they usually come back and go: yes or no, we think you're this rating. They will tell you why, and so you can. You can adjust things and resubmit, but usually after a while — especially if you're working with an experienced team, they kind of know we've done things to get this rating and it's rare that you come back and they go. You need to change your rating.

The. All those boards, by the way, publish what their ratings info are. So you, have no excuse for not knowing. But sometimes it's pretty complex and it varies by country to Country. So we have to make decisions on whether to keep certain things, like I said, language, nudity, drugs, whether you want to keep them, change them or just get rid of them entirely.

Sometimes you consciously do this early on in development. I tend not to do that. I tend to be like this is what the game wants from me. Fallout wanted some wanted drugs, wanted some more mature things.

Arcanum, yeah, not as much, Temple, not as much. So it really depends on the game you're making. You can decide whether you want to self censor early or get censored later. It's really up to you anyway. Uh, suine, I hope this answered your questions.

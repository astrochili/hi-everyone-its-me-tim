+++
title = "Features: From Ideas To Implementation"
date = "2023-09-20"
id = "1gWQ8WVdZZc"
status = "transcript"
tags = ["Game Development"]
summary = "I talk about the process of taking a feature from an idea to a shipped implementation."
references = ["qmfZFoc53ss", "4XzaRlW2sio", "Qc8zuhaqWPM", "JOVgSfjWeVI"]
+++

Hi everyone. It's me, Tim. Today I want to answer a question from Wyatt's Vlog who asks: could you talk about the steps you take when exploring and implementing a feature?

Good question, also one that I held off a while on answering because it touches a lot of other videos: the three Challenge videos: challenging facing designers, challenges facing produce programmers and challenges facing artists. I'll touch upon those, also, the problem of doing credits: I'll touch upon that as well. So let me tell you how I go about exploring and implementing a feature in a game. So I'm gonna assume the game is already roughly designed, possibly already underway, and you have an idea for feature for it, because this is very different. This is a very different process than coming up with an idea for a game altogether.

For that, take a look at my video on brainstorming. So this is just: I have an idea for a feature for a game I'm working on first thing I do — and I know I've said — this repeatedly, I should have brought this up earlier — is write it down. If you have an idea, doesn't matter how small, how big, how complicated, how simple, write it down. I can't tell you how many ideas I have failed to do that for. And then a few days later, a few weeks later, I'm like: hey, what was that idea I had and I don't remember. So write it down at that point. If, when you have an idea and you want to consider putting it in a game, you that you have in development, at that point I run it by people.

This is not formal. I don't call a meeting. I may not have a design document.

I basically just use some people on the team and even some people at the company and even some people I know in the industry as sounding boards. There are some people I've worked with. That are really good at bouncing early level ideas off of and you may think, Well, everybody's good at that. No, there are some people that if you just bring them an idea like this, they almost always say no, they go no, no, or they can't even wrap their head around what you're talking about. They need to see mock-ups, they need to see specifications, they need to see a similar game doing it, and I'll talk about that in a second.

But, like Leonard Morris, keys are always been a good sounding board, even for non-art stuff. I mean especially for story and setting stuff. But sometimes I bounce a system mechanic off of it because he's played a lot of games and he's played all of our games and he's really good at going yeah, won't that cause this problem? Or isn't this a lot like this? Or didn't we try that already?

And it's just good to do that I also loved bouncing ideas off of Charlie Staples, who was the lead designer in The Outer Worlds. Our offices are right next to each other and I'd walk around the corner with my new idea face and I, you know, I can almost imagine he's like, what did you just think of? But he was really good, gave really good feedback.

The other thing I do at this stage is I look at games that have that feature, or similar games that maybe be missing that feature, and then I look at their reviews and not just the good reviews. This is something I use. Sites like Metacritic, anything that Aggregates reviews. I like to go to them and look at those games and go: did anybody talk about this feature? Or did anyone talk about this feature being missing?

Like. They wish they had this feature? Because that game's already shipped and you can see if they have a similar feature. You can see what if it caused any issues or people wish it was different. If it was missing a feature and people call it out, as I wish this feature was in there, you can see if anybody points out why it wasn't added. So, anyway, I often look at other games reviews for that reason.

So that was stage two. Stage three: write a specification. Write a formal specification.

Try to get everything down that's in your idea: every UI you think you'll need, what new art you think your need, what systems it's connected to. What features do you think it might be similar to in other games or what other games would have benefited from such a feature, what this game does for you. Write down the goals. Remember I talked. About this: when you write a design document, put the goals at the top that this design, this feature, is going to meet, so that way, when you have subsequent meetings on this, people can talk about one of two things: either they don't think this new feature of yours meets the goals you listed, or they question those goals, but those are two totally separate discussions. Also, you should say in some way how this feature connects to your pillars. You did write design pillars right. I got a whole video on that right: design pillars. That's exactly why they exist, so that when you come up with features like this, you can say: we have to have this feature. It directly supports this pillar, which is barely supported as it is.

I've gotten several features added to games that way, so, now that you've finished stage three and you have a written spec, run that by people in at obsidian. We did these specs um on Confluence so that way they could be edited and people could go and look at previous versions. But also, what you could do is, when you wanted people to look at it, you would ask for reviews by and you'd actually put their names in and put a little check box and that way you know if they've looked at it and finished the review, because when they put in all their comments, and when they're done and they put their last comment, they checked that box, which means they're not going to put any more comments on this version. And then you, when, those people have all checked it off, you can go in and see what they've commented on. This is the time for people — especially your programmers and artists, but other designers — to say things like: I don't think this feature is going to work, or I don't know if, how long we have to do it, or doesn't this contradict this other feature, or while this is going to require a lot of new art or new UI — basically all the stuff that's gonna be difficult about doing this. Or if they don't understand something, hey, you didn't really explain this.

How is this going to work? I don't understand this part.

Right here in those videos I talked about challenges that programmers and artists and designers face. This is a major cause of. Those.

Programs were off to be like, oh, they want to add a new feature. Artists are like, oh, we don't have time to add that art, and this is where all that comes out. So then you go to the next stage where you revise that spec. You try to address everyone's issues.

What's nice? About confidence? You can literally answer the questions they leave as inline comments. You can answer it and then, if they agree, you resolve it and it goes away. So you try to resolve as many of those things as possible. You write a new spec that addresses all of this. Boom, now you've got a spec for the feature that has passed all your leads and anyone else who owns that section of the game or wants to have a say in that section. So then you take that revised spec. Now in the old days, that's when I'd implement it.

Hey, I have got enough information, I'm going to code it right now these days it gets handed off to a producer who gets estimates from all the devs, especially the ones that looked at it and especially the leads, gets their sign off that this is something that's going in the game and puts it into the schedule and assigns it to people to work on. So at this stage, if you're interested, like hey, who's going to be doing my feature? You can see it in the schedule, the project schedule. When will it be put in? That's also on the project schedule.

It's an estimate, but at least you have an idea. So then it gets implemented and. At that stage what happens is when those features get invented because you have a. I used to talk to my executive producer every morning. You have a. I think we had a weekly or bi-weekly meeting where we sat down and talked about production and he would go over.

Here's everything that got put in, so it, when it gets implemented, it goes off to QA. He tells the head of QA: here's a new feature, just went in, please start testing it I often tested it myself. Like I mentioned, I'd come in early, I grabbed the build and I test those things myself because, especially I want to see how they, how they work and how they interact with other things and how close if the implementation was what was specked was just something QA won't necessarily look for. QA will say, hey, there's bugs, or it's really imbalanced, or it works badly with this other feature or has this interaction with this other feature. I look for all those two, but I also look for: is this what was asked for? I compare it to the spec and go. We said we wanted this feature and this is what we got.

Do those two match up? At that point and I used to meet with my QA lead, especially in the last few months. We meet every week. Weed talk about this feature. Go over his notes, go over my notes. Uh, anyone in QA ahead would give their notes to the QA lead.

Um, I keep saying him because in my head the last one was Taylor Swope, um on The Outer Worlds great query lead. Um, then you, meet, you talk about this and it revisions are put in. You talk to the producer and you go: hey, these things aren't quite right, they need to be changed.

That gets scheduled, time estimates. But for about how long it would take to do and when it will get done, that Loop between those two. Test it, revive, look at it, revise it that Loop happens frequently until you're happy with the feature or the game ships, whichever comes first. In many, many of my games — and I'm talking about this — the shipping comes first. For Arcanum. I'm not even sure that Loop even happened once. In Arcadium you're playing several features in The Identical way. They were implemented from the spec without any chance to balance or compare out and interact with other features.

That's what was great about The Outer Worlds is those Loops were maintained. So a lot of things got balanced, debugged out of Worlds was a very bug-free product. I was really proud of that, so at this point I said, okay, so the game ships.

Let's talk about credits, because I've mentioned this before. But now that we've walked through this process of inflonian feature, I could say, well, I, it was my idea, I get the credit. But then look at all the people who touched it. There are many people who may have said, whoa, that was your idea, but we, I heavily modified it or I pointed out all these problems and it got massively changed.

The program are implementing it. Say, oh, I found a way of implementing it with using these other systems or an artist. Go, hey, I modified that UI so it could support that. All these people had their hands on it and some of them may have had their hands on it for a lot longer than G. I had this idea, I wrote it down, I bounced it off. A few people wrote a spec. Three days later I washed my hands of it and walked away.

Meanwhile there's some program or artists that spent months on it. How do you credit that? Who? When somebody goes, who's responsible for that feature? Was it the person who originated it? Was it the person who worked hard on the revision Steps, either on the spec or after it was implemented, to get it right? Was it the person who spent the huge amount of time actually implementing? It, doing the code or the art that supported this feature? That's why it's really hard to do credits, because you're done, this feature is implemented, but so many people can point to it and go: I did That's why I find it hard to write credits with anything connecting them to any feature and why it's hard for me when, people ask on the channel to go: hey, Tim, who, did this?

That's a very different question from whose idea was this? Who implemented this? Who actually got it working correctly? Who balanced it? Those are all wildly different questions with often very different answers of what person did that? So that's why it's hard to answer: hey, who's responsible for this feature anyway, so this — you notice this stage, from writing it down to it shipped and you're trying to figure out the credits — is one, two, three, four, five.

Six, seven, eight, nine, ten steps, a lot of work by a lot of people, and it's only getting more complicated as games get bigger. I hope, though, why it's Vlog. This answers your question of how you go from exploring the idea of a feature to implementing it, to shipping it.

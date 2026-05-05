+++
title = "Game Development Caution"
date = "2023-09-27"
id = "LMVQ30c7TcA"
status = "transcript"
tags = ["Game Development"]
summary = "I talk about game development caution and how it seems to be affecting newer games."
references = []
+++

Hi everyone. It's me, Tim. Today I want to talk about something that, for a lack of a better phrase, I'm going to call game development caution.

Before I start and tell you three different stories — they're a little different, but then I'll tell you what I'm thinking about. When we made Fallout, towards the end, when we were really trying to get it out, we had two white boards. One white board had a list of features or content that weren't done yet, that really needed to get in, and the other whiteboard had a list of what the 10 most egregious bugs were, and next to each person, next to each one of these on these two different whiteboards, were listed the person who was assigned to it. We did it in a whiteboard like this so that people could come in the morning and look at it because this predated jira or Confluence or anything like that. They could come in, look at the Whiteboard and go: oh, I see something I need to jump on worked.

Fine. I don't think I heard any complaint about it.

People liked getting stuff off of that. If they saw something. I was like: I'm on that today, try doing the exact same thing 10 years later at carbine.

Overwhelmingly. People said: no, do not do that, I will quit. If you do that if I see my name on that whiteboard, I will quit. And I said: well, what if we don't put people's names next to it? I'll still quit. People will know it's me.

Story two: when we're making The Outer Worlds I wanted to put in this is probably a year, end of year two, so we're still a year away. The combat AI wasn't really in yet, so I asked for a very simple combat aggression code to be added. It was. This is how simple it was.

Every time an NPC got shot, they would see if. That person was on the list of someone who'd shot them. If they weren't, they'd add them to the list, which they matter with the amount of damage they just took. If they were already on the list, they'd just add the amount of damage they took. Whenever they're deciding who to attack, they attack the person at the top of the list, that's it.

That's all I wanted. Keep in mind, the advantage of that basic AI. You can make lots of changes later. You can make them that it has the one at the top of the list if it's different than the person you're attacking. The damage has to exceed the damage of the person attacking You by a certain amount before your change targets.

You can take distance into account. You can take whether you can reach them into account, whether you have a ranged. Weapon, into account. All that comes later. That's all I wanted.

Uh, it got put into the programmer production query queue and came back with an estimate of four weeks. I pushed back, saying the code I asked for was very simple — I've written it before, would take about 45 minutes.

It's basically, there's already a callback when you get hit, that's when you look to put them on the list, and there's a callback. There's a call when you want to pick a Target, that's when you look at the list and see which one you want to attack.

That's it. The programmer who got signed to came to me and said I need four weeks and I'm like why walk me through what you're going to do? And he goes: you don't understand, and I was like I've coded this three times, walk me through it. And he wouldn't, he left, he. Left. Angry lead programmer came back, started yelling at me, saying if he says he needs four weeks — and I'm four weeks, he needs four weeks, and I'm like, then I will do it, I'll have it done before lunch. And he said no, because no one, then people will have to support your code.

I'm like: well, let me walk through. I'm going to walk you through what I want and you tell me why this takes four weeks. He looked at what I wrote, which was about 10 lines of pseudo code on a whiteboard, and he goes: I'll come back. He came back about an hour later and said: what about two weeks? And I said: do I have any options here? Fine, two weeks.

Story three: Leonard and I talk about features all the time, whether it's dialogues or system mechanics or story setting. We get very into it. Our voices may. Be raised, we're jumping out of our chairs to draw things on whiteboards, we're pacing back and forth. I know I've mentioned this before, but Anthony Davis showed up at our door and said: you, guys have to stop yelling. Everybody's getting nervous. It's like Mom and Dad are yelling at each other.

Still don't know who. He met with Mom, but we explained that. Just us talking. We're not mad, but we're trying to tease apart exactly what to do and we're getting into it, so what do those three stories have to do with each other? I'm starting to see in the industry — I shouldn't say starting — in the last decade, the last quarter of my career, I'm starting to see this rise of what I can only call development caution, an abundance of caution, of padding estimates, uh, time estimates, of wanting to go around and check with a lot of people to see if something's okay, asking: should we do this? I'm not sure. Let's have a meeting frequently. People would want to have a meeting to discuss something, and those were the very people who would say: we have too many meetings, I can't get any work done now.

Caution can be a really good thing if it leads to less bugs, less stress. Also, I get the fact that, because games cost more now, your people are approaching it with this sense of caution, because you're not just going to be out a little bit of money, you're going to be out a lot of money if this game doesn't do well. The thing that worries me, though, is games can also be a lot worse because of caution, and everybody who's cautious kind of denies that they're like: no it'll, we're reducing bugs, we're in Pre.

Increasing life work balance. People are less stressed and I'm like, true, but with but you're also taking a lot less risk in a game, which in many games I think give them less charm. And, yeah, even games that have Jank have a lot of charm. My games have had Jank. Uh, I know people talk about Jank and other games. You know things where the AI acts in a bizarre way in certain circumstances or NPCs say weird things or do weird things. It can be Charming, but things have changed and I know games have gone from being an expression of an idea, of an, of like artwork from a particular person or group of people into a corporate driven, money-seeking instrument, and I get it.

There's a lot of money going into these. In a way, though, I would argue they always were. You always were making these with the idea that.

You know, I hope it sells a lot. We make money, but now designs are being driven by this. That's why we have microtransactions, it's why we have pre-orders, it's why we have what we're starting to see lately where games are. If you pay a little more, you can play it a few days or even a week early now. You can't always get blame the Publishers or the Developers for this.

If people didn't pay for it, they wouldn't do It's like spam, if everybody stopped answering spam tomorrow, it would go away. But because a tiny percentage does, it's there for everybody to see. But so I'm not really talking about the money driven part. I'm talking about how the caution is dampening down the ideas. It's why I want to double down on this. I've always thought the Indie space is a lot richer in ideas. Probably not.

Money, certainly not money — but they're much richer in ideas because they take less they take, they have less caution and take a lot more risk, and unfortunately, what I see then is um, aaa's that dip into indie games for features and ideas. By the way, it's not just Publishers and developers that I see all this caution with. I've seen a huge rise in caution in game journalism. It's become the norm that no one — what no journalist — wants to risk getting into an embargo situation where they're not given a, an early access code so they can't write their reviews earlier than other people. They're worried about not being invited to press events or, you know, junkets, I think they're called — so a lot of them have gone a lot more cautious in what they say.

I really miss the reviews. I'll name a couple, like Scorpio in the 80s and 90s, at desklock in the 90s and early 2000s, because those two people, those two reviewers, said what they thought.

If you put out a game, they secure you for all the things that were wrong with it, but then they praise you for everything that's right with it. Now it's sort of like: well, we really like this, but they don't want to like really double down on it because it may be something people don't like. So like, let's say, a journalist loves the diversity in the game, he may go. Well, I'm not going to say that that much because I don't wanna come across as being pandering, and also some people yell when you talk about that. So I just see a lot of the passion drain out of game journalism and they're really just trying to go for what can?

What kind of review can I write that generates the most? Clicks? And I guess this worries me because if I see this everywhere, if I see this in Publishers and developers and now new people entering the industry, they don't have this passion anymore. So you know what's the moral of all this I've got? I want to tell people: just go and make it, make what you want. You don't need a committee to sign off on it, you can always go back and change it. Or, if you make something and it turns out not to be good at all and unsalvageable, throw it away. But that that rapid iteration to get to some really good idea is a lot better than just being so cautious, that you basically creep up to a very mundane game that doesn't show any kind of passion in its development.

People can tell, so I started with stories. Let me end with those three stories and how they kind of got resolved. So I didn't even try to do the Whiteboard solution when I made our worlds.

What I did is I made my own Confluence page, called, like I was Tim kaine's top 10 or something. It was in my Confluence space and I wrote: here are the 10 biggest things I once looked at this week and there were a few producers who would look at that page all the time. What was great about this solution? Nobody could come and complain to me about it because it was in my Confluence space, my own personal but public Confluence space. Also, I'd like to point out that anybody could go to jira at any time and say what are the 10 most High prior, highly prioritized bugs and who are they assigned to. So we already had that whiteboard, virtually, but somehow it was okay that it wasn't called attention to.

For the combat aggression code, I think I settled on two weeks and I think it got done faster than that. Great, I got it I don't think I asked for anything after that. I didn't go and specifically ask for anything because I realized that I was being viewed as some sort of ogre when I knew something could be done faster, and there was no solution to it. Which is why, years ago, I started thinking: oh, this is becoming a problem.

Same thing with Leonard not yelling each other. We just kept doing it. We're like it's our office. We shut the door, we're not mad at each other, but this is the way we get things done.

Note noted that people know some people don't like it. We won't get things done like that with you and let me tell you, I think there were people who felt like they missed out on not being parts of those conversations. Some people would come over: uh, Charlie um had his office right next door and he would the lead designer on The Outer Worlds and he would come in sometimes and join in. Great other people didn't do that. You missed out and I think you missed out on some really fun, active, engaging conversations about game development. But that's the way things are going. So I'm not sure I have a great solution other than telling people, reminding people to be passionate. But I just kind of want to talk about this because it kind of ties into bigger teams and longer development time, bigger budgets, just this whole game development caution that's rising up in the industry. So there got that off my chest.

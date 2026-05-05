+++
title = "My First Professional Game"
date = "2023-05-22"
id = "3nLc-pULEhw"
status = "transcript"
tags = ["Careers"]
summary = "I talk about the development of Grand Slam Bridge, made by Cybron and distributed by Electronic Arts in 1986."
references = []
+++

Hi. It's me, Tim. Today I want to talk about the first professional game that I ever worked on.

I had fun yesterday talking about how to get a job in the industry and I said how I got my job. But this is the first game I worked on that shipped and it wasn't why I got hired at a company in 1981.. And that, by the way, was I was still in high school. My first purchase of parachute pants was still a couple years in the future and I wish I was kidding. I basically worked at this company doing tools, for artists, because the Atari 800 had really good graphics modes and that's why I was hired. But a couple years after I started they decided to make a bridge game — Bridge, the card game.

Now, it's interesting, they also changed their name about this time. I got hired in 1981 at Pegasus software, but they didn't do a copyright search and that name was already in use. So about a year, and a.

Half later, it switched to cybron, see, I told you naming is hard. So they told her, they told me I'd come back from to work full time in the summer. It was either the summer between high school and college or my first summer back from college, I don't really remember. I didn't take a lot of notes. Then I really started taking notes: um, my next game, because graduate school burns into you to take notes. But I was just a high school student. I thought I'd remember everything because it was also exciting.

So I came to work for a summer and they said: we're going to make a bridge game. The first thing I thought is: I don't play bridge. I don't know how to play bridge, I've never played bridge.

But they had hired someone — Nathan Schneiderman, who was a good bridge player. He couldn't code, so what he did is he wrote down the rules for bidding and, by the way, like 99 of bridge is just bidding, he wrote down rules and flow charts, and then I would convert those flow charts into C. The funny thing is they were using C even though they didn't really know C, and I'd learned C and Pascal in high school and then used it extensively in college, so I really knew. See well, um, also, the entire game was being done in text Graphics, which I will show you in a second. So I remember sitting down with the lead programmer, Fred Klein, and talking about things you could do in C.

Like I got to enumerations where you could actually use words instead of numbers, so you didn't have to say if your card was 50, you know one. You could say: if card dot suit equals spade and card dot uh rank equals Jack, you could put those in enumerations. Fred loved enumerations, then I showed him recursion. Fred did not like recursion. I walked him through why you'd use it and also why you wouldn't it wasn't a. You know, here's a hammer make everything into a nail situation. But he wasn't super happy with that.

But I remember what happened was I would play the game. I think after that summer, when I came back for winter break, I was playing the game and it was really slow to shuffle the deck, like one time I thought the game had hung because it was like three or four seconds, which is an eternity. You know you said new, deck and it used to sit there.

You're like what's happening, so I looked and the algorithm he was using was literally he. Had two arrays right there. That's pretty bad, but he would pull card. I'd pick a card at random out of the first array and then put it in the first slot. Then he'd pick another card at random to put in the second slot. But if he picked one that had already been picked, he had to pick again, which means, as that algorithm went along and most of the slots in this array were empty, he'd be picking slots were empty over and over again and the algorithm took longer and longer run. By the way, there is a chance — it is non-zero — that that algorithm will never finish.

I told Fred this and he was like: no, it's fine. People didn't wait a few seconds and I was like: what if we use the Fisher Yates Shuffle — something I'd learned and there was a Twist on it I can't remember the name. Of the twist, but it used one array. It was oven, which meant it just went through the array once and so, in other words, it was not only guaranteed to end, it would end a lot faster than the other one. These shuffles were now near instant, so he really loved that. So let me show you.

The game came out in 1986 and this was a cover and I thought that was pretty cool, you know. And also Electronic Arts published it I mean, how huge was that? I mean, Electronic Arts was big even back in the 80s, although for me it made me think of: uh, there was a basketball game they made, Larry Bird versus Dr J, which I thought was amazing, because when you dribbled and threw the basket and it broke the glass of the backboard and low res. But still in the 80s, everything was amazing. So I thought that was cool. I was like, hey, I have a game has shipped by Electro Electronic Arts.

Now we're still in college — um, oh. And let me show you the game too, because it was all done in text Graphics that looked like this: these are all done with character, ASCII characters. It looked pretty good for the time and it was fast because it would. This was a text mode, but now it looks kind of, you know, a little rough and ready. So anyway, that was it shipped in 86. I came back the next summer, in 1987, and I was supposed to work for them, but I think they were out of business, they were gone and so then I tried to get another job, um, through another friend, making a compiler, which I thought was really exciting. That fell through, and my mom, who's awesome. Let's establish, she was awesome — she said: you know, you are finishing college and you're about to go to grad school.

Why don't you just take the summer off and do nothing? It'll be your last summer to do nothing. So I didn't do anything. Did bother me, though, that, before they disappeared, that the guys at cyberon never sent me a copy of the game, but I didn't really think about it, I would. I saw a review of it in — uh, I might have been computer game strategy plus. This is a long time ago, and it would it reviewed.

Well, and I'm like this is great. So I went to graduate school. I got a master's degree in two years — actually a year and a half — and then, a couple years later, I was in my PhD and for various reasons, whenever I'd go into, I decided I don't want to. Do this anymore, so I set my resume around and it got picked up. Um, a local company, interplay, asked me to come in and do an interview and in the interview I was all excited because they wanted me to work on a Bard's Tale game. And I'm like, yeah, they guy. I was talking to Tom Decker, who would later on be my producer there for various titles and was the original producer on Fallout. He asked me a question about my resume. He said: you said you worked on Bard's Tale or you said you worked on Grand Slam bridge for Electronic Arts.

I'm like I did and I started telling him some stuff I did and he goes: now, wait, a minute. Here's he had. He reached up and pulled off a shelf a copy of the game. He goes: this is the manual. I said, oh, I've never seen. This, and he goes: look at the credits.

And I went: my name wasn't there, not programmed by, not additional programming by, not even thanks to. And what was weird is another programmer was missing. There was another programmer who worked on it besides Fred, and his name was missing too.

Mad, in fact. Tom told me later, when I was an employee at interplay, that he originally thought I was lying to try to get the job. But when he saw how mad I got about my name not being there and also the stories I had told about what I had done and what it had been like to work at that company, he was like: I believe you, by the way, I found out later that was pretty much par for the course.

Credits have been contentious for the last 40 years in this industry. There are some companies that, if you don't stay to the very end, they drop your name off the credits, which I think it's not illegal, but I do think that's unethical.

My rule was always: if you were there for majority of the time, or up to the end, or you contributed a major asset to the game — whether it's Code, art, design — you went in the, main section programmed by art, by, designed by. If not, you still went in the credits, but it was additional programming by, additional art by, additional design by, and my only exceptions were if you were only there for a short time and nothing you did ended up in the final game. Okay, you know, if you were there for two months and the game took three years to make and none of your code made it in, I can see not putting your name in, but you know, usually I did it's additional programming by. I was nothing in that, so I was mad. But I did end up getting that contract job which turned into Bard sale construction set, which then turned into an employee mint job doing Rags to Riches. So everything was good but I thought that was cool. It was my first experience with the industry. In hindsight I learned a ton of lessons that you would think I would have put to use, but those came later.

Things about being told things would be done quickly and they weren't. I mean, this is a bridge game. I thought it'd be done in a few months. It took three years. Uh, not having my name in the credits — um. Having a lead that discounted everything you said until you actually proved that what you were saying was right.

Optimization nightmares — there's a lot of things that happen on. This game that were a microcosm for things to come. But anyway, that was my first experience in the game industry, was not my last, and I will see if I can find a picture of me in parachute pants, but I don't think any exists, luckily. Have a good day.

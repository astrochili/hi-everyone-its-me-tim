+++
title = "Damage Numbers, Part 2"
date = "2024-04-01"
id = "96uGEA0r6Bo"
status = "transcript"
tags = ["Balance", "Combat Design"]
summary = "Hi everyone. It's me, Tim. Today I want to talk about damaged numbers again, because I already did a video on damage numbers, but that video was mostly about how they should appear in the HUD."
references = ["GTMdWT8Lb9k", "SL_aTjKsxok", "G_2kCbPO2sU", "DqL9R5PqE20"]
+++

Hi everyone. It's me, Tim. Today I want to talk about damaged numbers again, because I already did a video on damage numbers, but that video was mostly about how they should appear in the HUD.

And apparently what a lot of you wanted was: how do you actually pick damage numbers? And by that you meant the range of damage numbers, because once you have a range of damage numbers — like do you go from 1 to 10, one to 20, one to 100, one to a th000? Once you pick that range, that leads to a r, a subsequent range of damage, of numbers for hit points and bonuses and weapon damage and things like that. So I've talked about damage numbers as a HUD. I've also talked about the ranges you should use for skills and attributes. This talk is going to be very similar because a lot of the things I said in the skill and attribute talks, which I'll link below, are still valid here. Um, so, before I go about talking about the method, I use to do numbers, number ranges for damage, let me talk about just some stuff about numbers. Big numbers make people happy, when they hit something and they see two, they're not as happy as when they see 20 or 200 or 2,000 or 20,000. Now you may go wait, if the monster has 10 hit points, who cares if you're doing two versus the monster has 10,000 hit points and you do 2,000?

You're thinking here, you're not thinking here. A lot of people don't think about It's what they care about and you can dismiss this. But perception is really important.

It's why, if you look at old arcade games, it's often you know when you're shooting aliens, each alien's worth 100 points, and so you look at the score at the end and it's always like a thousand or 10,000 or 20,000. It always ends in two zeros and you're like why not just make each alien one point? And when you're done you might have 21 points instead of 21,100. And it's because people like the big numbers. It's that simple and that perception is really important, because your goal — remember your goal of the game is to have fun. People should be happy when they play your game. I have a whole video about random numbers and I'll link that below, and in that I talk about how random numbers seem to confuse and anger some people. You can make something random, but people don't seem to understand what random means.

What they really want is fair or uniform or well distributed. They don't want random, and so with damage is the same way. They don't really want, proportional. What they want is a feeling of power, a feeling of impact, and that's what big numbers give you. Big numbers also have another Advantage: if you intend to do anything as a percentage. So let's say you have a weapon and it says this increases your damage output 5%. Well, if you decide to have damage 1 to 10, 5% leads to a very small fraction. If you increase, even if you hit the maximum 10, the additional 5% is what 10.5. You know it's just. This isn't what you want, um.

So what I would recommend, is the way I do damage values, is I pick a range of what I want to do. Let's say I do 1 to 20, because I know I'm going to have some percentage values in there. Then you just spread out the design from there.

You're like: okay, if a sword does 1 to 20, then I can have a club do 1 to 10 and a dagger do one to five, and I can have damage bonuses of like plus one or plus two or plus three. Ooh, but I want strength to do damage bonuses too. Wait a minute, if, the maximum number I'm going to see is usually going to be 20 and I want all my strength scores and my attributes go 1 to 10 and I want each one of those to give a A plus and I want bonuses on the weapons, now you, find yourself going wait on that 1 to 20 range. I can easily get 10 from my strength and from the bonus on the weapon alone. That's half of the total range of that weapon. So instead of doing 1 to 20, you're now doing like 11 to 30. You, may be fine with that, or you may go wait a minute. That makes an awful lot of impact coming not from the weapon itself.

The person could pick up a dagger and still be doing, you know, 11 to 14. So you may want to go back and go. I want to switch it to one to 100. Now you have to ask yourself: that's a huge amount of variation, you know. You may, um that may be more Rand nness than you want, because somebody could do three and someone else could do 97. That's a huge variation. You may instead want to do a d10 * 10.

That still does. It still has a range of up to 100, but it's 10, 20, 30, 40, 50, 60, 80, 90, 100. This is important because no one will ever do less than 10 and on average you're going to be doing 55. And if you want to do percentage bonuses, like you know, plus 5%, plus 10%, it works on these bigger numbers. So you may also want to think about multiples of ranges like that.

From there I said, spread out the design. Now you have to think about: well, if I'm doing this much damage output, how many hit points should the enemy have? And at that point you want to think, well, how long do I want combat to last? You thought, think about the pace of combat and combat beats. And well, I want relatively low monsters to go down in three hits.

Well, if you're doing, let's say you're doing — the uh 1, to say let's say you're doing the uh 1 to 100 range, that means on average you're going to do 55 hit points. If you want them to go down on average in two or three hits, that means you should probably give them like 100 Health, maybe 110. So you know one hit won't take him down two. Hits might, three hits should, and then there's a chance that it may take four or five or six, or longer than that. So that's now. You have a pin on your enemy Health.

Well, what about more powerful enemies? What about bosses? Well, now you're like: well, if I'm going, if an average, you know regular creature goes down in three hits and has 110 hit points, and I want a boss to be really powerful, I'm going to have to give him a thousand hit points, you know, to make him last.

Well, wait a minute, maybe I should give him armor. Oh, maybe I should have armor.

Due damage threshold or damage reduction. Damage threshold is you have to do least that much damage or they take nothing. And damage reduction is that percentage of damage is removed from the attack. Tons of choices there, but you can spread out and see well. If I do this and I put a low value of those on regular enemies and a bigger value on bosses again, how many rounds will he last?

That's what you're trying to figure out. Out now this. There's a Converse here.

I've talked about how much damage the player doing to creatures you want to talk about. Well, how much is the creatures doing to the player? And if you want those to be roughly in parody, that means the damage on the player is going to be very similar, but there's usually more monsters. That means the players going to have health. How long do you want have to have health? How long do you want him to last, against what kind of creatures, at what level?

Well, that means the players hit points are going to not be 10 or 20, they're going to be hundreds. And then, if you want them, to deal with multiple monsters all doing this damage output, that's going to be thousands. So then you may go: well, I will have, I'll have monsters do less damage. Okay, if you want to give the monsters magical weapons or spells that increase, you know, like maybe there's a shaman who Buffs the enemies. If that buff is a percentage, you're back to the problem of: ooh, I'm not sure I want these small fractions, or most of the time the buff doesn't do anything.

Again, treat this like the proof of contradiction. You learned in math class where you were trying to prove that the square root of two is irrational, so you assumed it was rational. You did the proof, you ran into a contradiction. Therefore, your one assumption must be wrong.

Pick one thing — a damage range — and from there calculate everything: damage bonuses, enemy Health, boss, enemy health. Uh, enemy damage output, boss damage output, player Health. Figure all those things out and, along with the damage bonuses, on from attributes and from skills and from the weapons themselves. And what armor, how armor reduces it.

Just put numbers in for all of those and see if you like the output. If you don't go back to the first thing you did maybe damage uh range and tweak that, do it again, see how those numbers change. Maybe it's good everywhere except the damage on bosses and players. Well, maybe tweak how uh armor reduces that damage, because you're like, say that our game will encourage you to wear armor and we're going to put armor on all the bosses. You can do things like that. You can try to tweak where the problems are and affect it.

A lot of designers I know use spreadsheets for just this reason. The idea isn't that you will create, in you know 10 minutes, this perfect diamond of a design. You will instead work on how all your any choice here affects a choice later, and if you don't like that effect, change this choice or change another Choice. That's along the calculation, so you may do all this stuff and you really like all your numbers and you put it in, and then you get feedback like: the bosses are too easy. Well, do you increase the health on the boss? Do you give them better armor on the boss? Do you um say, hey, we're only using damage resistance, but I want to add damage threshold, just to bosses? You can do all that and see how it affects your numbers.

There is no one answer to this. It's very much try it and see. And keep in mind, though, what I say about perception. If you decide you don't have a lot of like percentage changes in things and you don't want a lot of big numbers, that's fine. It will have a reaction among many players about oo I. I don't feel a lot of impact here, especially if the HUD shows those damage numbers you may like. That it's really up to your design. So my Rec recommendation is: pick what you like, see where it leads in your design. If you don't like something, go back to whatever you P.

Put a pin in, change that value. You can have lots of things pinned and a lot of things unpinned that you're figuring out. You will eventually arrive at a nice damage range that you like. I think that's the best advice I can give you, and I know it sounds a little weird to say try it and see, but that's what all the designers do. You've got to put in your rules, see where they lead. You decide what rules to change and I hope that helped you come up with damage number ranges.

+++
title = "Toy Update, Part 3"
date = "2024-09-20"
id = "oCKPphehFGk"
status = "transcript"
tags = ["Toy Update"]
summary = "Hi everyone. It's me Tim."
references = ["wpbUuoyGPBM", "CA7gIg5b6_8"]
+++

Hi everyone. It's me Tim.

Are you ready for a toy update? This will be toy update number three. I'll link part two and the first one down below. But this is because I, when I did toy update 2 and I was showing off my space game with some ideas I had — um, I got so many good ideas of what to do with the shields on enemy ships that I had to do them. So I spent a weekend learning how to do shaders in, and it's not that bad. I thought I was going to have to do a lot more work than I did.

So let me show you, if you are using uh, the universal render pipeline, which is what I'm using, or the HDR, the highdefinition render pipeline, you basically already have Shader graph. So I just made a Shader folder, uh, went in there, right clicked and said create a Shader graph and boom, this is what I see. Now you can see that I get the vertex and fragment Parts.

They're already. In there, so what I did was I created a new variable, that's of type color, called Shield color, and I pipe that into the color on the fragment. And then I made a new node called Fresno, because one of my viewers had a great idea of using Fresno.

Effects are for a sphere, well, for any object, if your view is aligned with the normal, you know — so it's either pointing right at you or pointing away from it. Then it's pretty clear, it returns at zero and then, if it's orthogonal, it returns a one, which means when you put it on a, sphere, the sphere is clear in the center and gets brighter towards the edges, which is exactly what I want, and you can adjust that. So what I did was I — I - they already had this node under in the math nodes, under Vector. There was a Fresno, so I put that in there and then that got piped into the alpha input on fragment. I added the normal vew vector and the uh, the view V. The normal vector and the view Vector already exist as nodes. Pipe those in and then for the power variable, which, constrains how far out before the Fresno effect looks, if it's a really high number, you only see down the edges. If it's uh zero, the whole thing becomes opaque. You can, I, I made Fresno power a variable. Now let me warn you about a script issue I ran into, because you might run into it too.

If you look up in the corner here where it says Shield power and Fresno power, they're exposed like here's: this is Shield power, Shield power. I named Shield power and it the unity, put in some random name for it, I think. It was like vector 3core — a bunch of junk.

So I renamed it Shield power, just like the name. So the reference and the name are both Shield power. However it renames it, renames the reference. You can't have spaces in reference names, so it put an underscore in there. So my script didn't seem to be working. And then I realized: oh, even though I typed Shield space Power for the reference name, it made it Shield underscore power. So I'm back in my script and made it Shield uncore power and that's the variable that I control for what?

The color of the shields I want. Let's see what it looks. Okay, that was pretty cool, but that was just with the power fixed at 1.7, and what I wanted to do instead was when the shields first come on, they're just near the edge and as they get more and more, damaged, you start to see them everywhere. So you can just visually, when you glance at a ship, if you barely see a flicker there, the shields are running at full strength. As soon as you start to see most of the shields there, and they're glowing and they have color, which I'll talk about in a minute — that's when they're pumping away a lot of energy and they're very damaged.

Watch this warning. Okay, so what we saw there was is the shields took more and more damage. They kind of closed in on the ship one.

Several other viewers thought that my color scheme wasn't right, so I decided to come up with a new color scheme for the shields. The first thing I did was remember I said in the previous update that I just set the colors to change at certain set points, not this time. I actually made a gradient, so the gradient I wanted to use starts at White and then goes down through blue and yellow, into orange, into red. Red is really damaged because a lot of people you were saying red in their, your mind, means damaged. I made that into a gradient. That gradient is based on the number of Shield hits, um that are remaining. So when you have, when the sh, The Shield can take 10 hits and it's it hasn't and it hasn't taken any hits, then it looks white and then, if it's taken a ton of hits, it moves down to the red part of the gradient through blue, yellow, orange.

This is the code um, this is the code where I create the gradient and then this is the code where I use it. And now let's see what it looks like with the new reverse color. So I thought that was pretty cool.

Um, the one last thing remaining that I wanted to do on this update was — and it's something I want to point this out because I love it — another viewer said: hey, why is your targeting cursor opaque? Why don't you make it transparent? It'll be easier to Target things. Let me just say first of all, that is a. It's, yes, it's a simple idea, but it's very, very insightful and it's intuitive. And I hadn't done it. This was just trivial, was just taking the alpha, I was setting the color of the targeting cursor, just, I think color do green from Unity. I just went in and changed the alpha to 0.25 and now we have a. Isn't that so much better? It's a perfect example of sometimes there will be a simple idea with a simple execution and it just makes things better.

Anyway, most of that was. About me changing shaders, but I got that little tardan cursor change in there through. That's the latest update on my space game.

Think about making the whole HUD transparent, but I think it might be hard to read. If I do that, I don't know. What do you think I should do next?

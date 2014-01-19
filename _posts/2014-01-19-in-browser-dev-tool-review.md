---
title: Drag-and-drop In-Browser Dev Tools: A Review
layout: post
image:
 feature: keys_oasis.jpg
 title: A lonely spot of land in the Florida Keys
 credit: Michelle Hertzfeld
 creditlink: http://www.mhertzfeld.com/
author: Michelle Hertzfeld
tags: [design, front-end development, tools]
categories: [thoughts]
---
Wouldn't it be great if we designers/developers could just move bits of website around visually and get beautiful, well-structured code to work with out the other end? The stuff of dreams! If this is your dream, then this might be your year! In service of The Future, I tested (or attempted to test) four of the current front runners: [Webflow](https://webflow.com/), [Divshot](http://www.divshot.com/), [Froont](http://froont.com/), and [Jetstrap](https://jetstrap.com/). Read on for a summary and full reviews.<!--more-->

**Summary:** 2014 is going to be a great year. These tools are going to keep developing. At the moment, though, they're too difficult to use and are missing critical functionality (different in each) that means that there's a ways to go. But the day is coming! And (a surprise to me) out of the lot I liked [Webflow](https://webflow.com/), hands down. It's the only one that solved a problem for me, and I bet it did this by focusing it's product on core uasbility -- easy visual drag-and-drop and built-in dev hosting.

**Methodology:** I have a small, new project that needs to get going. The perfect time (the beginning of the process) to try to fit a new tool into my workflow. On to the reviews!

##Webflow

Webflow sez: "Create beautiful, responsive websites without code. Webflow is the top drag-and-drop website builder for designing and publishing custom, professional websites quickly."

###The Good
+ **Integrated hosting and preview solution.** Click a little rocket button (launch, get it?) and you've got a fully-functioning site to share with clients.
+ **Custom domain name.** Depending on the plan, you can pay a little extra and Webflow will take care of hosting with a custom domain. Plug and play, baby!
+ **Slick integration with Google Fonts and your TypeKit plan.** The way Webflow deals with integrations in general is pretty clear and easy.
+ **As easy a UI as possible in this field.** After testing several competators, let me tell you, Webflow's UI is the only one I didn't have to fight with.
+ **Provides ability to start with a blank slate.** This is a plus and minus. I don't want to have to override Bootstrap's native styles all the time if I'm just 'doodling' my designs. On the downside, I'm not sure yet what standard Webflow is using to do it's thing.
+ **Aimed at non-devs.** They do a good job of simplifying things and clearly have spent a LOT of time on user flow. I think even people without much web development experience will be able to figure this out.
+ **Exported clean code.**

###The Bad
+ **No in-browser code editing.** None! Want to add a span tag inside a heading to make a cool dropcap? Too bad!
+ **You are limited to what Webflow has already developed.** Webflow includes a solid base of parts that you can drag-and-drop onto its canvas, but there's nothing yet like the the Javascript pieces that comes standard now in frameworks like Bootstrap or Foundation. And since you can't add code...you see where I'm going here. There is a place to include external JS...I imagine you could spend a lot of time figuring out how to use this to do stuff, but that would be a time commitment, aka, the opposite of the reason I'm looking for a visual dev tool.
+ **Classes are a bit verbose.** As far as I can tell, there's no way to specify something like "all anchor tags under this div shall be blue." All you can do is add classes to specific elements. One must therefore be more verbose than one would like. Note: at least I could easily figure out how to style ALL h1, or ALL p, which is not something I could figure out in the other tools.

###Conclusions
This was the first tool I tested, and once I figured out that I couldn't see my code as I was working at all, I immediately scoffed and moved on thinking  "no WAY is this going to improve my workflow!" Ah, the hubris! Oh, the pride! It turned out that Webflow is the only tool I tested that was quickly usable and not a pain in the ass. And what it does, while more limited than other tools, it does well. Extremely well.

The code it exported looks pretty solid. Of course, it is not structured in the way I would normally structure my projects (I use Sass and this exports straight CSS), but it created a basic, fast, functioning prototype site that I shared with my client for feedback within 4 hours (this includes me learning the tool and doing initial design). It is a pleasure to be able to ditch Photoshop and work with something more interactive! It even automatically included some niceties, like the ease-down in-page slide effect.

Webflow can fit in as a design and testing tool, a fast prototyper. Right now, I can't imagine doing *all* of my development work in the tool, but to start projects, then export and re-factor into my normal flow, this could work (for a base site, there's not too much code -- I don't think it will take long to Sass-and-partial-ify). But then...$16 a month for a prototyper? Not sure. Maybe. I'll report back on how things go moving forward.

##Divshot

Divshot sez: "Fast, visual front-end development. As simple as a mockup tool. As powerful as a text editor."

###The Good
+ **In-browser code editing.** The interface looks like the in-browser Developer Tools we're used to. I felt very at home there.
+ **Really nice, interactive walk-through the first time you use it.** ...which you need because the UI is more complex than Webflow, perhaps necessarily as it provides more functionality.
+ **I get to use my Sass.** You can use css, sass or scss. It will compile...kinda.

###The Bad
+ **No blank slate.** You've gotta choose a framework to build on. There are several options, but this makes it difficult to use the visual editor as a 'blank slate' design tool.
+ **The way Divshot deals with files and file structure is a little obtuse.** You have to kinda guess at how to make your files fit together, and then how to make your files work once you download them. It works out if you've done web development with common frameworks before, but the barrier to entry will be too high for everyone else.
+ **Sass compiling was buggy.** After being so excited that I could set my workspace to how I usually use Sass, I spent more time than I wanted to (hours) trying to chase down compile errors. @import wasn't working, partials weren't working, random other stuff wasn't working. Maybe I just hit them on a bad day, but...yeah.
+ **What code where?** Never figured out where to track down already-implemented code. As in, when you're working with a framework, you use Dev Tools to see what code is already creating style and then build on that. Had no idea where to find that in Divshot. And so, how am I supposed to code on top of its included frameworks?
+ **Text editor yes, visual visual editor, not so much.** In the end, I wasn't sure what functionality I was getting. I could access all the text edit functions pretty easily, but I never figured out how to use the visual drag-and-drop part. And what I'm *not* looking for is someone to replicate what I already have (text editors and a server) online. this is adding.

###Conslusions
I came into this thinking Divshot would be the winner since it provided code inspection and Sass, but in the end I never got it working, and never figured out how to use the visual editor part of site. Oh well.

##Froont

Froont sez: "Responsive web design, the visual way. Design websites directly in the browser with a simple drag and drop interface."

###The Good
+ **Looks like it should be awesome.**

###The Bad
+ **The first time I tried it, I got overwhelmed/annoyed and gave up.**
+ **I tried again. Still couldn't get it's drag-and-drop stuff to work easily.** Kept clicking in the wrong spots, selecting the wrong thing, etc.
+ **What's with the name?** Let me tell you, it's a pain in the ass to search for tips and documentation -- Froont autocorrects to front, and just try looking for "froont center".
+ **Price.** $49 a month? Really? That's what I pay for Adobe CC.

###Conclusion
Webflow's UI is a billion times better. I'm not sure if Froont would have provided more functionality (since, as explained above, Webflow is fairly limited in what it does) but I never got there. I couldn't get off the ground at all.

##Jetstrap

Jetstrap sez: "THE BOOTSTRAP 3 BUILDER. Not just a mock-up tool, Jetstrap is the premier interface-building tool for Bootstrap 3."

##The Good
+ **Pass.** (See 'no free trial' below.)

##The Bad
+ **No free trial.** Seriously? I'm not paying you money to figure out that your tool sucks as much as all the others.
+ **Bootstrap only.** Apparently only integrates with Bootstrap, and I don't love Bootstrap (prefer Foundation or Gumby, at the moment).


###Final Conclusion
In the end, after a day full of testing and trying, the winner is (and I can't believe I'm saying this): [Webflow](https://webflow.com/). It doesn't do everything by any means, but it's the only one that actually abstracts the web development process enough and is intuitive enough that it becomes faster to do mockups with it rather than just rocking on Bootstrap or Foundation on your local machine with your own server from the start. Unfortunately, it doesn't have much flexibility. If what you want to do isn't implemented already, too bad, and I'm not sure I like it enough to pay $16 a month for a prototype tool.

Still, I'm really excited about the future of these tools! They will continue to improve. I think by the end of 2014 we're going to have some serious changes to the web design/dev process -- it will be a beautiful, beautiful day. Also, I'm really excited to see what [Macaw](http://macaw.co/) has in store. If that Alchemy engine does what it says it can, it could be a game changer.
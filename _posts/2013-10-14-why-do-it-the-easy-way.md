---
title: Why do it the easy way?
layout: post
image:
 feature: dock.jpg
 title: Dock in Annapolis, Maryland
 credit: Michelle Hertzfeld
 creditlink: http://www.mhertzfeld.com
tags: [Jekyll, GitHub, Markdown, Liquid]
categories: [thoughts]
---
"But why," I ask myself, "why should I use systems built by very smart people to suit a wide variety of website needs when I can spend time and energy making my own from scratch?" Why indeed.<!--more-->

Actually, in all seriousness, there are very good reasons for me, someone who traveled the path of web development from print design to html/css and now towards object-oriented programming, to practice building a blog from scratch rather than relying on something like WordPress to do it for me. The process of building programming logic is still relatively slow for me (and so more practice is good!), and it is tremendously important in modern web development (I think) to know how the gears in the background fit together. And, it's still kinda magical for me when if/then statement, etc, just **work**. Go magic!

(This is not to say, of course, that almost every time I have to fix a broken piece of Javascript functionality I don't want to put my first the screen and strangle the hamsters that I'm sure run the internet, but I digress.)

On the recommendation of [several](http://www.kinlane.com) [people](http://ben.balter.com/) and a good chunk of the internet, I went with the Jekyll/Liquid/GitHub killer combo. I want to learn more about versioning and the potential of something like GitHub to do more outside the programming paradigm (like make [government policy more open and accessible](http://project-open-data.github.io), for example).

There are many "get started with Jekyll" tutorials online and so I won't repeat them here. However, there **aren't** very many places to go to learn all those steps that the programmers skip since they're obvious (to them). And so, here it is: tips on how to do the "host your blog or site on GitHub with Jekyll" thing for designers. 

##Tips for Designers
###GitHub
+ Despite what every developer will try to tell you, GitHub is **not** actually very intuitive to use for non-programmers. The documentation, while pretty, is not thorough if you don't have prior experience. BUT! Stick with it, and if all possible get someone who's used to the git process to show you their workflow.
+ Speaking of, did you know that "git" is a thing? Yeah, I didn't either. GitHub is a specific online implementation of the [git version control process](http://git-scm.com/book/en/Getting-Started-About-Version-Control). Helps to know this fact to understand, then, GitHub and its purpose.
+ Note that GitHub's "just start here!!" process is a bit misleading because (to me) it makes it seem like you [download a thing](http://mac.github.com/) and you're good to go, and then there's also this online GitHub thing (they don't explain any interaction between the two). Actually, your computer and its local files work in tandem with your GitHub projects online--they're a team. You use GitHub through a combination of (1) a process on your computer (this can be command line or GUI)(the GUI is what GitHub prompts you to download when you sign up) and (2) a process on your GitHub account online. You work on local versions of your project through your normal file structure, and when you're ready use the GitHub GUI to "push" your file to your online "repository," or "repo," where then it is available for the world to see.
+ And so why do people get all pumped about this? Well, in addition to working on your own projects, GitHub gives you the ability to contribute to other projects. You can "clone" a project to your computer, create a "fork" of the original project that you edit and make better, and then, if you like, you can submit a "pull request" to the original owner of the project so she can accept (or not) the changes you made and merge them with the original project. Again, GitHub = not so intuitive. The terminology alone is a big hurdle, but, oh designer, you can do it!

###Jekyll
+ Jekyll a little piece of software that builds your site. That's its purpose in life. You will have to use the terminal to get it running, but once you change directories to the folder where your working files are and then set Jekyll to "watch" you can pretty much ignore it. [See more in the Jekyll documentation.](http://jekyllrb.com/docs/usage/)
+ Jekyll comes with a server -- super handy! You can set the server to run and watch your working files for changes, and then your local site will live at http://localhost:4000. Go nuts. If you also set [Sass](http://sass-lang.com/) to watch the right folder, everything will compile and build like a charm. **Pro Tip:** You can open tabs in terminal (I didn't know that till recently). So, I set Sass to watch in one tab, and Jekyll to serve and watch in another tab, and then can easily check both for errors if there are any issues.
+ When you're building your site locally, Jekyll will build your site to a folder called \_site. However, when you push your site to GitHub, get rid of that \_site folder. GitHub has Jekyll built in, and so it will serve your site correctly. Well, at least it should...
+ ...which leads me to configuration. There are always issues transitioning from local to live, and doing it through GitHub makes it a little more complicated. Check your \_config.yml settings, ask the internet -- it will eventually work.
+ Helpful resource on how to create a Jekyll site from start to finish: [Jekyll By Example](http://www.andrewmunsell.com/tutorials/jekyll-by-example/index.html#starting-your-website)
+ Work from an example: the [Minimal Mistakes Jekyll theme by Michael Rose](http://mademistakes.com/articles/minimal-mistakes-jekyll-theme.html) is a good place to look for how a Jekyll blog site might be structured.
+ Ready to take it to 11? Try these [Advanced Jekyll Features](http://www.divshot.com/blog/web-development/advanced-jekyll-features/)

###Liquid
+ Jekyll uses a templating language called Liquid to do its thing. Anything that Liquid can do, you can do. Anything that it can't do, you're SOL. Programmers get a little sad about this because they say Liquid is pretty basic, but just between you and me -- it's awesome. It's very simple to use, and so far does everything that I can think of.
+ There is a very nice intro to Liquid here: [Liquid for Designers](https://github.com/Shopify/liquid/wiki/Liquid-for-Designers)
+ I also really liked this [Shopify Cheat Sheet](http://cheat.markdunkley.com/) for Liquid reference (Shopify created Liquid). It helps you see what programming options are available in Liquid.

###Markdown
+ Finally, something easy! (No, really!)
+ Markdown "allows you to write using an easy-to-read, easy-to-write plain text format, then convert it to structurally valid XHTML (or HTML)" ([from the man himself](http://daringfireball.net/projects/markdown/)). Basically, you just learn some [very, very simple syntax](http://daringfireball.net/projects/markdown/basics), run your completed article/blog post/whatever through a converter, and out pops your HTML page. It makes blogging on the go super simple. For example, I now start posts whenever they come to me in Evernote using Markdown syntax, and then copy them over to GitHub when they're ready.
+ When Jekyll builds your site, it converts your Markdown into HTML as part of its process. I'm not sure if this is 100% built in or not. I had trouble with this locally and had to install a different Markdown converter as a Ruby gem and tell Jekyll to use it in my \_config.yml to get it to work locally. Once you push your site to GitHub, you should not have problems -- GitHub reads Markdown automatically.

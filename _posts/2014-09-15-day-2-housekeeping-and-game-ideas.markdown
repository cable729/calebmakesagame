---
layout: post
title: Day 2 - Housekeeping and Game Ideas
date: 2014-09-15
tags: [blog, daily, game-ideas]
time: 30
---

First, I'd like to start off by saying I had mixed feelings coming back the second day. Already? Yes, I know! Procrastination and motivation are hard tasks to fell. Thankfully, now that I'm working on this again I'm really excited to put up some of the game ideas I've been wanting to work on for a while.

## Part 1: Automate this shit!
I made a `rakefile`, basically a ruby batch file, that I can call from the command line to create a new post. You can view it [here](https://github.com/cable729/calebmakesagame/blob/gh-pages/Rakefile).

## Part 2: The bare necessities

<iframe width="420" height="315" src="//www.youtube.com/embed/9ogQ0uge06o" frameborder="0" allowfullscreen></iframe>

I wanted to embed a youtube video easily embed this video with markdown, but there's no default video embed markdown available. There is a [custom plugin available](https://gist.github.com/joelverhagen/1805814), but I found out that [GitHub Pages runs Jekyll in safe mode](http://ixti.net/software/2013/01/28/using-jekyll-plugins-on-github-pages.html). Basically, if I want to run custom plugins to do use the nifty code below

    {{ "{% youtube oHg5SJYRHA0 "" }}%}

I'd have to compile my blog locally and push it up. Maybe for another time.

# Trello

Everyone needs a backlog. For instance, I want to put analytics on this blog, so that goes in the backlog. Not terribly important. But also, it gives me a way to organize priorities and tasks. I may even use an agile approach and break off a certain amount of tasks each week. We'll see how things progress.

For now, you can view my backlog [here](https://trello.com/b/l6RlKpvs/caleb-makes-a-game-backlog).

# Game Engine

I took a look at Unity3D, which I've used a little bit, but had a hard time adjusting to. I don't mind that it'd cost me several hundred dollars to push out a game, but I'm not looking to make huge sums of money on this game (it will probably be free), so I don't really look forward to paying huge sums of money either.

On the other hand, Unreal Engine 4 can be bought for $19 plus 5% royalties. The royalties are calculated pretty low, too. Unless I ever made over 3k or 4k in a quarter (I can't remember) I wouldn't have to pay them a dime. The other plus of using UE4 is that I'd get to practice C++ using the engine that many AAA firms use. I'm sure LoL uses it or something similar, so it could be a way for me to move to the game engine team if I ever wanted to.

## Part 3: Game Ideas
So what the hell am I actually going to make? Good question. I have a couple of ideas.

# Run Kitty Run Remake

Check out this video if you (more likely than not) have no idea what the fuck RKR is. Yes, the name is silly, but give it a chance!

<iframe width="420" height="315" src="//www.youtube.com/embed/V81onQYG99Y" frameborder="0" allowfullscreen></iframe>

You back? Okay, so that is a solo run. Just one player soloing the first round. Usually it's a team of up to 10 or 11 players trying to get to the end together. When one player gets "tagged" by a wolf, he sinks into the ground. His teammates can walk over him to bring him back. The goal is to round the maze several times and get to the center.

I had a TON of fun playing this map in my Warcraft 3 days. I was actually a member of Clan F0lk, a RKR clan, and was pretty high up in the ranks. I had a blast playing that game with all the cool people from that clan, but now Warcraft 3 is all but dead and so is the clan. I'd love to bring back some of those experiences.

# Tower Defense Creator

I love TDs, and Warcraft 3 had the best of them. Stuff like Wintermaul Wars (two teams of 3 have to balance building towers and upping their recurring gold income by sending creeps, in order to take out the enemy lives by getting creeps through their defenses), Line Tower Wars (similar, but solo instead of team), Wintermauls (one team works together), and many more kept many players addicted to the game for a long time.

Looking back now, so many of these games were horribly imbalanced. WmW had a terrible feedback loop. If you got behind early, you pretty much lost. Maybe nostalgia is getting the better of me.

# Some other ideas
On my last day at Microsoft, I organized a game idea session. We got a ton of great ideas together. I'll see if I can find them later and post a few more up. Right now I'm leaning towards RKR 2.0, but I'll have to do some digging, because a lot of the ideas were pretty darn good.
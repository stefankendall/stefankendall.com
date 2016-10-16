+++
Categories = [
]
menu = "main"
date = "2015-05-15T22:52:24-04:00"
title = "April's game, Stock Story"
Description = ""
Tags = [
]
+++

I've always liked gamebooks and choose your own adventures.
[Give Yourself Goosebumps](https://en.wikipedia.org/wiki/Give_Yourself_Goosebumps)
defined my childhood, and I can remember many of the stories and mechanics from the books.
Most recently I've loved the work of Inkle Studios on [80 days](http://www.inklestudios.com/80days/) and the
[Sorcery!](http://www.inklestudios.com/sorcery/) series. These games are top in class in games currently made for the iPad. They hire real, actual writers for their games, and it shows. There are few "bad guys and egg heads" and deep stories in a branching, complex world.

I thought it would be fun to play with some of the mechanics needed for a
choose your own adventure, so I built [Stock Story](https://itunes.apple.com/app/id988245189).

<img src="/files/stockstory1.png" style="display:inline-block;width:49%"></img>
<img src="/files/stockstory2.png" style="display:inline-block;width:49%"></img>

## Stock Content

One of the constraints I put on the project was using nothing but stock material, aside from the story. All audio, images, and even the app icon are built using content from 

[shutterstock](http://shutterstock.com) ($143/month) and [audioblocks](http://audioblocks.com) ($99/year).

The audio for the project was a much better deal than the images, although you might recognize a few on other parts of the site. As it turns out, inkle studios offers a [choose your own adventure book creator for free](http://www.inklestudios.com/inklewriter/). Build your story, then publish to kindle for some small fee or output a json file that you can use however you want. Markers, conditionals, paragraph joining - it has it all. This saved a significant part of the challenge of the project, since all I had to do was write a json file handler instead of build a story format myself. The json schema seemed odd at first until I realized how incredibly robust it is for crafting any kind of story.

## Writing is hard

And it takes a long time. All told, I wrote 4,129 words for the story with 17 unique endings. This didn't leave much time for editing, and a huge portion of the game I thought I could build I had to cut.

## ...and so is flowing text

SpriteKit has no UILabel, no fancy-schmance auto-flowing auto-sizing line-wrapping class to display text. In SpriteKit, you get one line of text and you can set the font. Justification? Word wrap? What's that? In the end I wound up computing string sizes and manually flowing text, which wasn't the best and really made me appreciate the tools we have that make these sorts of problems trivial in normal applications

I tip my hat to you, whichever team built UILabel. You the real MVP. 

## ...and so is scrolling

You open Facebook.app/Twitter.app and scroll up and down willy-nilly. Items pop into view and everything is smooth and wonderful.

SpriteKit has no UIScrollView. I didn't have the time to build a solution myself, so each adventure is a one-way trip. 

## Retrospective

### The Good

- Stock images are better than you think, and they have more uses than late night commercial filler. I see stock images EVERYWHERE now, and I'm amazed how much I missed this before.
- Audioblocks is super cool and very inexpensive. I now have a go-to for both games and apps/demos/software.
- **I** wrote a (short) story! Good or bad, **I** hit the release button. **I** am now hyper-aware of sentences **I** write that begin with **I**.

### The Bad

- **I am not a good writer**. I do believe it's a skill that can be improved, so I hope to do that. I've downloaded [Writing Great Fiction: Storytelling Tips and Techniques](http://www.audible.com/pd/Self-Development/Writing-Great-Fiction-Storytelling-Tips-and-Techniques-Audiobook/B00P026PZC) as a first step toward learning to tell better stories. Stories permeate everything: video, documentation, debate, discussion, and even sales. People love stories, so it's important to learn how to tell them.
- More a tech demo, less a game. *Sorcery!* and *80 days* both have mechanics that make them more than just choose your own adventures, but while I tried to add a little extra by adding mini-games, I only had time to build one, so that fell flat.

## The Next Game

The start of each month will serve as a time to look back on the last game and plan the next. This leaves about two weeks for development and a week for release: screenshots, app icons, and the other hoops required to publish an app. So what's the next game? I'd like to build a proper side scroller, and maybe look into game center if I have the time. 
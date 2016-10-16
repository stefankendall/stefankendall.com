+++
Categories = [
]
menu = "main"
date = "2016-10-15T22:52:24-04:00"
title = "April's game, Stock Story"
Description = ""
Tags = [
]
+++

I've always liked gamebooks and choose your own adventures.
[Give Yourself Goosebumps](https://en.wikipedia.org/wiki/Give_Yourself_Goosebumps)
defined my childhood, and I can remember many of the stories and mechanics from the books.
Most recently I've loved the work of Inkle Studios on [80 days](http://www.inklestudios.com/80days/) and the
(Sorcery!)[http://www.inklestudios.com/sorcery/] series. These games are top in class in games currently made for the iPad. They hire real, actual writers for their games, and it shows. There are few "bad guys and egg heads" and deep stories in a branching, complex world.

I thought it would be fun to play with some of the mechanics needed for a
choose your own adventure, so I built [Stock Story](https://itunes.apple.com/app/id988245189).

<img src="/files/stockstory1.png" style="display:inline-block;width:49%"></img>
<img src="/files/stockstory2.png" style="display:inline-block;width:49%"></img>

## Stock Content

One of the constraints I put on the project was using nothing but stock material, aside from the story. All audio, images, and even the app icon are built using content from 

[shutterstock](http://shutterstock.com) ($143/month) and [audioblocks](http://audioblocks.com) ($99/year).

The audio for the project was a much better deal than the images, although you might recognize a few on other parts of the site. As it turns out, inkle studios offers a choose your own adventure book creator for free. Build your story, then publish to kindle for some small fee or output a json file that you can use however you want. Markers, conditionals, paragraph joining - it has it all. This saved a significant part of the challenge of the project, since all I had to do was write a json file handler instead of build a story format myself. The json schema seemed odd at first until I realized how incredibly robust it is for crafting any kind of story.

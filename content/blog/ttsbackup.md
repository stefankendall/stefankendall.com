+++
Categories = [
]
menu = "main"
Description = ""
Tags = [
]
date = "2016-07-21"
title = "npm install -g ttsbackup"
+++

So I published a tool on npm. If you play [Tabletop Simulator](http://store.steampowered.com/app/286160/) (and you probably should),
then you've probably downloaded a few [mods](https://steamcommunity.com/workshop/browse/?appid=286160) by now.

There are hundreds of great mods, but unfortunately the half life on any given mod is terrible. Mods disappear constantly, and that means you can't play them any more, even if you installed them locally!

A mod breaks when:

- ...it gets popular and the creator hosted files on dropbox, and dropbox has transfer quotas.
- ...the author pulls the mod off of the workshop for any reason. Sorry!
- ...any of the places the author put files goes down. Like imgur. Or pastebin (lol). Or some random german website (this really happens). Or dropbox or google drive.

The point is that there are way too many points of failure, and there's no reason for it.

Wouldn't it be great if you could fully copy a mod locally, and host it on something like your personal dropbox? Even if you play with your friends **all the time**, it's incredibly unlikely you would ever hit your bandwidth limit. And if you do, I'm sure one of your friends has dropbox, too.

This is why [ttsbackup](https://www.npmjs.com/package/ttsbackup) exists.

Instead of losing mods you've played forever, you can download all their images and models, and then create a new mod file that points to your copies of the files. So the flow goes something like this:

1. run ttsbackup
1. pick a mod
1. pick a download location
1. give a base url for the new mod (like `https://dl.dropboxusercontent.com/u/<youruserid/`)
1. pick a name for the mod backup

And that's it! You've saved a mod forever. No one can take it from you, and no shitty web host can go down to ruin game night.

If a mod has already become broken, there's also a "ttsbackup recover" command, but it probably won't work. Tabletop Simulator loads files a little weird; images in decks and bags don't actually load until you pull them out of the deck or bag. So if you haven't seen literally every card and model in a game, you don't have the full game.

Backup your mods early and often, and you won't lose them. Happy gaming!

p.s: I'm considering making this a native mac app. I'd support windows, too, if not for every cross-platform UI framework being godawful in this nascent age of technology. Ah well.
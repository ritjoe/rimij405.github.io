---
title: "Waiting for Godot"
date: 2019-02-05 03:38:25
categories: 
- [blog, hfoss]
tags:
- open-source
- class
- game development
- game engine
- documentation
- Godot
photos:
- /images/posts/waiting-for-godot/editor-live.png
---

# Waiting for Godot #

![Godot Logo.](/images/posts/waiting-for-godot/godot/logo_512px.png)

This week I'm working with [Godot](https://godotengine.org/), a free and open source cross-platform game engine released under the very permissive [MIT license](https://opensource.org/licenses/MIT). Let's get to it.

<!-- more -->

## The Game Engine I Waited For ##

The Godot homepage has this neat little tagline:

> **The Game Engine You Waited For**

The joke? [*Waiting for Godot*](https://en.wikipedia.org/wiki/Waiting_for_Godot) is a play by [Samuel Beckett](https://en.wikipedia.org/wiki/Samuel_Beckett), in which the main characters wait for the arrival of someone named Godot ... who never arrives. Although it was originally written in French, Beckett's English language version of the material was voted, "the most significant English language play of the 20th century," in a 1990 poll conducted by the British Royal National Theatre.

Godot was formed in 2007 by Juan 'reduz' Linietsky and Ariel 'punto' Manzur. According to Linietsky, the name *Godot* was chosen to represent their never-ending wish of adding new features to the engine, always pushing off an exhaustive product. It wasn't until February of 2014 - seven years later - that the source code would be published on GitHub and it wasn't until the end of that year for Godot to reach version 1.0 - it's first stable release.

## Features ##

At the time of writing this, Godot's last stable release (v.3.0.6) was released in July of 2018 - and development is on-going. The engine itself runs on several operating systems, including [Windows](https://en.wikipedia.org/wiki/Microsoft_Windows), [macOS](https://en.wikipedia.org/wiki/MacOS), [Linux](https://en.wikipedia.org/wiki/Linux), [BSD](https://en.wikipedia.org/wiki/Berkeley_Software_Distribution), and [Haiku](https://en.wikipedia.org/wiki/Haiku_(operating_system)). (*Fun fact about Haiku - it's an open source operating system supported by Haiku, Inc., a non-profit organization based in Rochester, New York, founded by [Michael Phipps](https://www.haiku-os.org/blog/koki/2009-11-28_history_channel_2003_interview_michael_phipps/), Computer Science graduate of Rochester Institute of Technology, Class of '97*). Games made with Godot can target desktop, mobile, and web platforms, using Godot's export template system. It's easy to create custom builds as well, if the existing templates don't cut it.

### Compact ###

Godot is a small engine - roughly 20 MB in size - and is very easy to compile. It comes with a built-in debugger, profiler (with graph plotting and time seeking), that allows for projects to be modified, even while they're running. Changes made while live are persistent - a design choice that some engines don't have.

### It's in the Node ###

Godot adpots a Scene- and Node-based hiearchy as its approach to game development. Everything in Godot is a Node and nodes can be (infinitely) nested. The visual editor that comes with Godot makes it friendly, inviting, and easy-to-use for creators at any level of the game development pipeline.

Godot's configuration and project files are version control friendly - feel free to make liberal use of your diff command. Godot also utilizes a custom scripting language (GDScript) that was written explicitly for the engine - GDScript's syntax is also supported by GitHub, so it enjoys some of the same privileges of its older cousins.

### Scripting ###

While GDScript is a Python-like language meant explicitly for Godot, it's not the only one available. The latest stable release has full C# 7.0 support (using Mono), support for a visual scripting system using blocks and connectors, and full native C++ support without the need to recompile the engine (through the use of a core-module dynamic). The GDNative aspect of the project exposes the engine's native C symbol API that allows developers to create and utilize bindings to other languages if they so wish - bindings already exist for Python, Nim, and D, among other languages.

### Animation ###

Everything in Godot was built with animation in mind: from bones and objects to function calls themselves, everything can be tweened. 

## Godot vs. Unity ##

![Picture of editor.](/images/posts/waiting-for-godot/editor.png)

Godot supports both 2D and 3D game development. While this is what draws the largest comparison to the [Unity3D](https://unity3d.com) game engine, there are three crucial differences. By all means, Godot is not a perfect engine, but, knowing where it excels can help you make a decision about which engine to choose.

### No Nest To Call Home ###

Unity doesn't allow you to use nested prefabs; all prefab instances will overwrite internal prefabs once 'nested'. While Unity encourages composability over inheritance, it seems like a missed area to not allow prefabs to be components and children of other prefabs. Godot's node-based system gets around this issue.

### Pixel Perfect 2D ###

Unity3D developers can create 2D games, but, it often comes with the overhead of running a 3D game engine on top of that. Godot's 2D engine is fully dedicated 2D and is not just a repurposed 3D approximation of 2D. This advantage allows developers to create pixel-perfect gameplay, utilize 2D lights and normal maps, and animate 2D rigs with skeletons and IK. Unity can get the job done, but, your mileage may vary.

### Unity is Proprietary ###

Unity3D is free as in free pizza. It's not an open source game engine, unlike Godot, so when you want to expand a particular feature set, you're stuck waiting for the Unity team to get around to fixing it.

## Godot vs. Cocos2d-x ##

![CocosCreator Logo.](/images/posts/waiting-for-godot/cocos-creator.png)

If you're looking for an alternative to Godot, [Cocos2d-x based editor CocosCreator](https://cocos2d-x.org/) is a great open source engine with its own community supporting it.

## Ease of Use ##

![Chrome Trip by @enthus1ast](/images/posts/waiting-for-godot/chrome-trip.gif)

*[Chrome Trip by @enthus1ast](https://code0.itch.io/chrome-trip). A downloadable, open source multiplayer game created with Godot for the GitHubGameOff 2017 jam.*

Godot is special because of its ease of use. Ariel Manzur, co-founder of OKAM Studios and Godot, led a team of industry newcomers in the design of adventure game *Dog Mendonça & Pizzaboy*. Godot, in some ways, was built by its founders to help express the desire for a more visual approach to game development, without necessarily sacrificing the power that comes with engines like [Unity3D](https://unity3d.com) and [Unreal](https://www.unrealengine.com/en-US/what-is-unreal-engine-4).

Teachers at a West Virginia high school have used Godot as a way to address the state's 2016 [coding, app, and game design curriculum](http://careertech.k12.wv.us/OCTIWebsiteRevisions/16Clusters/InformationTechnologyMainPage.html).  There's plenty of room for students to learn game development while introducing them to the concept of free (as in free speech) software.

## Open Source & Diverse Community ##

There is no question behind Godot's status as free, open source software. On November 4th, 2015, Godot joined the [Software Freedom Conservacy](https://sfconservancy.org/). On June 22nd, 2016, Godot received a $20,000 Mozilla Open Source Support (MOSS) "Mission Partners" award to incorporate Web Sockets, WebAssembly, and WebGL support. It has the acknowledgement of the big names in open source, and, the community is very active. There are currently 4,045 open and 11,267 closed issues on the [upstream repository](https://github.com/godotengine/godot/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc). The project has been [forked more than 3,800 times](https://github.com/godotengine/godot/network/members) and there are currently [263 open pull requests](https://github.com/godotengine/godot/pulls?q=is%3Apr+is%3Aopen+sort%3Aupdated-desc). 

It is a thriving, vibrant community. This year, the first ever *Godot Sprint* was held in Brussels, two days before [FOSDEM 2019](https://fosdem.org/2019/) and [GodotCon 2019](https://godotengine.org/events/#godotcon). Contributors were able to meet in order to encourage completion of C++ engine features, writing of documentation, and creation of teaching materials for new developers. These are signs of a strong open source project that will be a mainstay for years.

There are several ways to get involved with the community:
- IRC [freenode.net#godotengine](https://webchat.freenode.net/?channels=#godotengine).
- [Discord](https://discord.gg/zH7NUgz).
- [Matrix](https://matrix.to/#/#godotengine:matrix.org).
- [Facebook](https://www.facebook.com/groups/godotengine/)
- [Reddit](https://www.reddit.com/r/godot)
- [Twitter](https://twitter.com/godotengine)
- [Steam](https://steamcommunity.com/app/404790)
- [YouTube](https://www.youtube.com/c/GodotEngineOfficial)
- [Godot Forum](http://godotdevelopers.org/)

## Support Development ##

If you aren't interested in contributing to the Godot project as a developer, consider donating monthly via [Patreon](https://www.patreon.com/godotengine) or directly via [Paypal](https://godotengine.org/donate). Godot's donations are processed by the Software Freedom Conservancy and used to hire developers based on contracts that are made transparent to all supporters.
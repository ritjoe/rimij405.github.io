---
title: 'Quicklook: What''s The Scoop?'
tags:
  - open-source
  - class
  - shell
  - powershell
  - scoop
  - unlicense
  - Windows
  - quicklook
categories:
  - - blog
    - hfoss
date: 2019-04-03 01:18:07
---

# What's the Scoop? #

[Microsoft's releasing more open-source software](https://opensource.microsoft.com/), but, everyone knows it doesn't matter if your distro doesn't have a good shell.

This isn't about how [PowerShell sucks](https://outsourcedguru.wordpress.com/2016/02/22/why-powershell-sucks-so-badly/comment-page-1/) or how its source has been released under the [MIT](https://github.com/PowerShell/PowerShell/blob/master/LICENSE.txt) license so that naysayers can [contribute](https://github.com/PowerShell/PowerShell/blob/master/.github/CONTRIBUTING.md) the very features they believe are missing (or help address the over [1,800 issues](https://github.com/PowerShell/PowerShell/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc) open at the time of writing this blog post). No; this is about making PowerShell better with a Scoop.

## What is this software? ##

[Scoop](https://scoop.sh/) is a command-line installer for Windows that was made to help make PowerShell a bit more *digestible*. Appreciating scoop requires a decent understanding of the context behind PowerShell and the Windows security system in general.

### PowerShell Problems ###

Microsoft, created PowerShell with cmdlets (`command-lets`) - lightweight scripts that perform a single function - and created a Verb-Noun naming convention to help reduce [command memorization](https://docs.microsoft.com/en-us/powershell/scripting/learn/learning-powershell-names?view=powershell-6). This is quite neat if you're just getting started with terminals, shells, and Windows' awkward brand of system administration - genuinely, I am a big fan of making things more accessible for new users.

Nothing's clearer than a command that says, `Stop-Service`, and it doesn't take a senior SysAdmin to understand what a `Get` Verb command might do to a Noun - good things I'm sure! However, the trade off tends to work against developers who **do** begin to memorize the more frequently used commands. 

PowerShell's are quite literally *verbose*. While some commands have aliases they aren't necessarily the most familiar. `Get-ChildItem` is [listed as the command that](https://www.pdq.com/powershell/), "gets the items and child items in one or more specified locations." It's aliases? `dir`, `gci`, and `ls`.

Most other commands, however, might be clear and transparent in meaning - but they lack any reasonable alias. No Unix developer is going to spend time configuring their aliases in Windows PowerShell when they can simply boot up [Linux Bash on Windows](https://docs.microsoft.com/en-us/windows/wsl/install-win10).

Scoop helps by providing familiar tools from the bash environment and making them available to PowerShell. For example, `scoop install curl` will allow you to use the `curl` tool on PowerShell under your user account. 

What does vanilla PowerShell do? [It has aliased](https://superuser.com/questions/344927/powershell-equivalent-of-curl#comment995042_591311) the `Invoke-RestMethod` cmdlet as `curl` and `wget` while utilizing an entirely different syntax.

Don't want to use the cmdlet? The related PowerShell commands aren't much better: 
`(New-Object System.Net.WebClient).DownloadString("http://www.example.com/hello-world.html","C:\hello-world.html")`.

Speaking of which...

### Windows Security ###

Want to install something in Windows? I hope your pointer finger is ready.

![Image of a User Access Control dialogue box on a Windows system.](/images/posts/scoop/uac.jpg) 
*When I'm not on the internet, I don't expect pop-ups.*

Introduced with Windows Vista, the User Account Control (UAC) is a part of Windows' authentication and security suite. In the great scheme of things, this is the force behind the dialogue boxes that will interrupt your mojo whenever you try to make sure your installer isn't employing any [dark patterns](https://en.wikipedia.org/wiki/Dark_pattern).

There is no way to turn off UAC's pop-up functionality on Windows. Scoop, however, is not like PowerShell and it certainly is not like Windows. It doesn't concern itself with things that it doesn't need to care about.

See, scoop understands something that all good Unix developers understand: you don't need to sudo to install every little thing on your system.

The [collections](https://github.com/lukesampson/scoop/tree/master/bucket) of [programs](https://github.com/lukesampson/scoop-extras) that scoop provides an easy installation for are filled with examples where this is true. 

I do not and I **should not** be giving administrative access and permissions to installers for most programs. Most applications don't need to be installed to the `C:Program Files` directories - there are many that can operate in a standalone (even portable) capacity.

## Why get this? ##

Besides bettering your life, scoop is also a scriptable framework. It's encouraged if you're looking for a way to consistently setup environments on Windows systems that have access to PowerShell.

## Who created this? ##

The original creator [@lukesampson](https://github.com/lukesampson) hasn't submitted a new commit since mid-2017. At 787 commits, he still stands as the second biggest contributor.

The core developer, [@r15ch13](https://github.com/lukesampson/scoop/commits?author=r15ch13), on the other hand **started** in mid-2017 and now has over 5,610 commits.

It doesn't take a [git by a bus](https://github.com/tomheon/git_by_a_bus) to see that the wealth of knowledge about this project is not distributed enough to keep it from perishing should @r15ch13 decide not to continue development.

Get it while you can.

## Where can you find it? ##

You can find scoop's source on its [github repository](https://github.com/lukesampson/scoop).

## What's the license? ##

Scoop is actually 'licensed' under the "[Unlicense](https://unlicense.org/)". This is a specific way to for developers to dedicate work to the public domain. The license itself combines a copyright waiver similar to that from the public domain SQLite project with the no-warranty statement from the MIT/X11 license.

It's the antithesis to 'all rights reserved' - this license is a bit of a '[no rights reserved](https://creativecommons.org/publicdomain/zero/1.0/)' situation.

## Can I contribute? ##

Since the time of writing, the last pull request was created 8 hours ago; it's very active. In fact, the one disadvantage is that it's become a burden on the current community.

GitHub contributor [@h404bi](https://github.com/h404bi) submitted an [issue](https://github.com/lukesampson/scoop/issues/2939) last New Year's Eve asking for the community to consider the fact that Scoop never releases a version that is 'explicitly' stable. The other developers agreed.

As it stands, they have yet to finalize a new workflow but their main challenge is separating the buckets - the name given to collections holding program installation settings and metadata - from the core of the program. 

It's a relatively small codebase and the documentation is more than enough for someone interested in getting started with how it works.

## Caveats about PowerShell ##

It is silly to realistically expect PowerShell to work like Bash. Even if the Verb-Noun dynamic gets tiresome, PowerShell is far from the only option available to users on Windows systems and people are always encouraged to use what they know best.

PowerShell is open-source; and so is scoop. These are both examples of what community development can support. The best part is the freedom to modify your environment however you see fit...

***

...That is, until you remember that Windows 10 is still a proprietary operating system and that nice OpenSUSE distro I have running a KDE Plasma desktop environment is sweet, sweet FLOSS.

After all things considered, perhaps it is with a bit of irony that in order to get scoop on Windows, you'll need to be prepared to install it using plain old PowerShell.

`iex (new-object net.webclient).downloadstring('https://get.scoop.sh')`

(And you might come across a UAC error when you try this too).
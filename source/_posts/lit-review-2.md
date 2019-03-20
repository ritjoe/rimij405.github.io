---
title: 'Literature Review #2: Roads and Bridges'
date: 2019-02-17 22:16:03
tags:
  - open-source
  - class
  - bugs
  - issues
  - documentation
  - reading
categories:
  - [blog, hfoss]
---
 
 # Review: Roads and Bridges: The Unseen Labor Behind Our Digital Infrastructure #

This is the second of several literature reviews for content relevant to the humanitarian free and open source software course. In this entry, I will be reviewing *[Roads and Bridges: The Unseen Labor Behind Our Digital Infrastructure](https://github.com/ritjoe/hfoss/blob/master/assets/roads-and-bridges-the-unseen-labor-behind-our-digital-infrastructure.pdf)* by [Nadia Eghbal](https://nadiaeghbal.com/).

<!-- more -->

***

## The Basics ##

Nadia Eghbal is a Protocol Labs researcher based in San Francisco and is the author of *Roads and Bridges*. Eghbal explores the production and economic models behind open-source software, and had [previously worked at GitHub](https://www.linkedin.com/in/nadiaeghbal/), building programs, products, and partnerships to better support open-source developers.

In July of 2016, Eghbal published *Roads and Bridges*, a deeper look at the maintainance required of our digital infrastructure. Likening this massive support system (with an unprecedented demand) to physical infrastructure (*a la* roads and bridges), Eghbal draws out support for the great work that open source developers do - and highlight the challenges that come with sustaining that infrastructure.

In addition to writing longform research on open-source software, Eghbal has written extensively on the subject in [shortform](https://medium.com/@nayafia) and has been a part of [podcasts that highlight](https://changelog.com/rfc) the [culture of open source](https://hopeinsource.com/).

You can find more of her research on her personal website, [here](https://nadiaeghbal.com/research/).

## The Gist ##

Eghbal's work is a detailed retelling of the open-source history, reaching as far back as 1998, when OpenSSL was first created between a group of security experts in the UK. OpenSSL - a cybersecurity project that is known for enabling websites with the ability to transmit sensitive data over the internet - was recently susceptible to Heartbleed, a dire security flaw overlooked by its handful of maintainers. 

But, OpenSSL is used by millions around the world - the internet wouldn't exist as it does today without it. OpenSSL's problems are indicative of a recurring issue in the open-source community's narrative: the use of free software without the support to maintain it.

***

## The Good ##

- 1) There is a great encouragement in the writing to reuse and borrow from what others have created before.
- 2)  Free software makes building empowering software accessible and possible to those with limited funds.
- 3) The sheer size and wealth of material that Eghbal presents is crucial and necessary to understanding the full context of open source history: the fact that such material has been released for free access to all is just as telling of where Eghbal stands on the conversation.

***


## The Bad ##

- 1) New developers who consistently build projects using tools from others before them may never gain a deeper understanding of the work they create.
- 2) Developers without a deep understanding of the work that they create rely on possibly insecure services and infrastructure that could collapse - the more who use a particular project as a dependency without understanding it, the greater the risk becomes of system-wide failure. (See: [NPM/Node pre-release mayhem](https://github.com/npm/npm/issues/19883)).
- 3) The greater the gap in skill, the harder it will be for younger developers to fill the holes left by older developers. People can't work on software forever and it needs to be maintained; but software today is, "deteriorating," due to the lack of funding and contributions (pp. 76).

***

## Q&A ##

- 1) What organizations are actively contributing to the problems at hand?
- 2) What can be done to keep companies investing in open source over the years?
- 3) Are our communities of software too big to fail? NodeJS? Others like that? What can we do to combat degrading and insecure code?
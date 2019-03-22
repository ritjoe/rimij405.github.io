---
title: "Community Archictecture Analysis: KDevelop"
tags:
- open-source
- class
- architecture
- documentation
- analysis
categories:
- [blog, hfoss]
---
# Community Architecture Analysis #

## Background ##

As part of the Humanitarian Free and Open Source Software (HFOSS) course offered at RIT under the IGM program, students were split into separate groups in order to perform a community architecture analysis on a software project of their choice. This exercise serves to engage students with the practice of evaluating the health of open source community projects from various perspectives.

This report showcases the findings of such an analysis on the KDevelop project. KDevelop is a free and open-source feature-full, plugin extensible, cross-platform IDE for C, C++, Python, QML/JavaScript, and PHP. KDevelop’s [earliest version](https://marc.info/?l=kde-announce&m=90648146015087&w=2) (0.1 Alpha) was released in September of 1998 by developers Sandy Meier, Stefan Heidrich, and Stefan Bartel. Since that time, KDevelop was [rewritten](https://marc.info/?l=kde-core-devel&m=98598814600661&w=2) by Bernd Gehrmann for it’s 3.x release sometime in March of 2001, rewritten again with a plugin-based architecture for its 4.x release, and was ported to Qt5 and KDE Frameworks 5 for the 5.x release. 

As part of the KDE® family of applications, KDevelop is just another member of a well-established and robust free software community. The KDE® Community’s earliest form took shape as part of an [announcement](https://groups.google.com/forum/#!msg/de.comp.os.linux.misc/SDbiV3Iat_s/zv_D_2ctS8sJ) from Matthias Ettrich in October of 1996 — Ettrich was searching for developers interested in creating a, “consistant, nice looking free desktop-environment,” [*sic*] under the project titled: **Kool Desktop Environment**.

## Team Members ##

Nic Hartley | [nxh9052@rit.edu](nxh9052@rit.edu)
Joshua Schenk | [jks7743@rit.edu](jks7743@rit.edu)
Ian Effendi | [iae2784@rit.edu](iae2784@rit.edu)

## Git By a Bus Results ##

— Pending results from Nic —

***

## Callaway Coefficient of Fail ##

— Pending results from Joshua — 

***

## Alternative Analysis Results ##

### About The ‘Openness Rating’ Tool ###

Our alternative tool for the community architecture analysis is the Openness Rating review, created by OSS Watch, an independent, non-advocacy service provided by free and open source software consultants. As said on their homepage, “OSS Watch provides unbiased advice and guidance on the use, development, and licensing of free software, open source software, and open source hardware.” In partnership with [Pia Andrews](http://pipka.org/standard-bio/) [@piawaugh](https://twitter.com/piawaugh), the Openness Rating tool is a diagnostic model that evaluates how ‘free and open’ a particular piece of software is. Waugh 

To perform an assessment, the tool asks questions as it pertains to the software’s legal issues, data formats and standards, available knowledge, project governance, and the market climate. These questions are based off of the paper *[Foundations of Openness](http://pipka.org/wp-content/uploads/2008/07/Foundations-of-openness-V2-release.pdf)*, written by Pia Andrews (publishing as Pia Waugh) and Randy Metcalfe, and are used by OSS Watch as part of their own consultancy work. Each question asked has a predefined set of answers - once all of the questions are selected, the tool is able to provide the ‘openness rating’ that serves as a benchmark for how free and open the software is. 

#### Strengths ####

— Pending thoughts from Ian on strengths of this analysis tool — 

#### Criticisms ####

— Pending thoughts from Ian on weaknesses of this analysis tool. How can it be more effective? — 

### Results ### 

The following sections list the question posed by the tool alongside the answer that best fits what we know about the KDevelop project.

#### Legal Issues ####

**Is the license recognized as a common Free and Open Source license?**
`Both OSI and FSF approved.` *(KDevelop is licensed under GNU GPL version 2).*

**Who has permission to run this software?**
`Anyone.`

**Are all project dependencies clearly documented and license compatibilities audited?**
`Yes, but the audit process is undocumented.`

**Who is permitted to examine the human-readable source code of the software?**
`Anyone.`

**Who is permitted to adapt or modify the source code of the software?**
`All licencees.`

**Who is permitted to redistribute the modified or unmodified source code of the software?**
`All licencees.`

**Does the license permit sub-licensing of rights?**
`No.`

**Does the license also grant a patent license to the licensee?**
`No.`

**Is the licensee required to make modified or unmodified source code available if they redistribute the code?**
`Yes.`

#### Data Formats and Standards ####

**Is there full public disclosure of the majority of data and communication formats used in the project?**
`Yes.`

**Does the project rely on any closed proprietary standards?**
`No.`

**Are there any direct costs associated with any standards used?**
`No costs.`

**Are the majority of standards used approved and published by any of the following standards bodies: W3C, IEEE, IETF, OASIS, or ISO?**
`No.`

**Does the project use documented project management processes such as XP, SCRUMM, or PRINCE 2?**
`No.`

**Does the project support unicode through the use of encoding like UTF8?**
`Yes.`

#### Knowledge ####

**Which publicly available communication or dissemination mechanisms does the project use?**
`Documentation section of website.`
`Publicly writeable wiki.`
`Version control system.`
`Email lists or online forums.`
`Instant messaging/IRC.`
`Issue Tracker.`

**Does the project discourage major project communications outside the approved channels selected above?**
`Yes.`

**Are project decisions ever made in a non-public environment?**
`No.`

**Is any project knowledge purposely kept private?**
`No.`

**Who is able to access all the (non-private) project knowledge?**
`Anyone.`

**Is there any financial or legal barrier to accessing or acquiring some or all knowledge in the project?**
`No.`

**Is there any technological barrier to accessing or acquiring the knowledge of the project?**
`No.`

**Is the knowledge stored in publicly published data formats (with appropriate metadata) that will make it accessible over time?**
`Yes.`

**Is any of the project knowledge available in more than one language?**
`Yes. Over 10 languages.`

**Who is able to contribute to the project knowledge?**
`Anyone.`

**Are there public archives of the knowledge?**
`Some publicly available archives.`

**Are there documented data recovery processes in place?**
`Don’t know.`

**How good is the user-specific public documentation?**
`Documentation is easy to access, easy to read, complete and highly appropriate for the user.`

**How good is the developer-specific public documentation?**
`Minimal developer documentation.`


**Are there documentation sources external to the project?**
`2-4 good sources.`

#### Project Governance ####
**Is there clear leadership in the project?**
`Yes.`

**Are the structure and policies of the project clearly and publicly documented?**
`Partial (includes one or more of the above items).`

**Are there publicly accessible behavioural guidelines for the project?**
`Yes.`

**Is there publicly accessible and easy to find documentation about how to participate in the project?**
`Yes, for both users and developers.`

**Is the project leadership elected by the project community?**
`No.`

**Who is able to contribute to the project development?**
`Participants willing to register in some way.`

**Are contributors required to sign a document stating they have the necessary permissions to make their contributions?**
`No.`

**Who is able to obtain commit rights to the project development?**
`Partially self appointed, partially meritocratic group.`

**Is there a single point of failure or control for committing changes to the primary project source?**
`No.`

**Who is able to obtain easy access to and use the software?**
`Anyone.`

**Is the software easy for users to access, install, and run so it can be trialled (for those who have access)?**
`Yes, there is a fully automated installer.`

**The software release cycle (including snapshots and major releases) is…**
`Consistent and predictable.`

**Is it easy to acquire, build, configure, and install the source code from scratch?**
`Yes.`

**Is there an avenue and structure for recourse beyond the project maintainers?**
`Yes.`

#### Market Climate ####

**Are there any costs or barriers to setting up a business around the project?**
`No.`

**Are there any technical barriers of entry to setting up a business around the project?**
`No.`

**What proportion of the core developers are from the one company, institution, or department?**
`Don’t know.`

**How many contributors have some or all of the time they spend on the software paid for?**
`Don’t know.`

**Is the project applicable to more than one industry?**
`No.`

**Which revenue models are available to a new business looking to build a revenue stream around the project?**
`Customization.`
`Support and maintenance.`
`Proprietary extensions.`

**How many organizations offer commercial software development and code customization services on the project?**
`1.`

#### Summary ####

The results are broken down for each category and are listed below:

```
Legal Issues: 79%
Data Formats & Standards: 69%
Knowledge: 81%
Project Governance: 76%
Market Climate: 42%
```

These results can also be found [here](http://oss-watch.ac.uk/apps/openness/shared.html?d=P3A9S0RldmVsb3AmbD0wLjc5MzEwMzQ0ODI3NTg2MjEmcz0wLjg3NSZrPTAuODE0ODE0ODE0ODE0ODE0OCZnPTAuNzYmbT0wLjQxOTM1NDgzODcwOTY3NzQ0).

The ‘Openness Rating’ tool suggests that the KDevelop project is sustainable over the long run. The biggest challenge facing KDevelop’s longevity is in dealing with the market climate. Although a powerful and popular program, there isn’t much in the way of commercial support. KDevelop does have the influence of the KDE Community on its side: KDE developers are likely to support KDevelop as with any of the applications that remain a part of the KDE family.

## Important Links ##

IRC: [#kdevelop](https://webchat.freenode.net/?channels=kdevelop) on freenode

Source:

https://github.com/KDE/kdevelop
https://cgit.kde.org/kdevelop.git *(Mirror repository)*
https://github.com/krf/kdevelop *(Mirror repository)*

Mailing List Archive(s): 

https://mail.kde.org/pipermail/kdevelop/ , 
https://mail.kde.org/pipermail/kdevelop-devel/

Documentation:

http://www.kdevelop.org/index.html?filename=HEAD/features.html *(Feature list)*
http://www.kdevelop.org/index.html?filename=HEAD/requirements.html *(Requirements)*
http://www.kdevelop.org/index.html?filename=HEAD/branches_compiling.html *(Compilation instructions)*
http://api.kde.org/extragear-api/sdk-apidocs/kdevelop/doc/api/html *(KDevelop IDE API documentation)*
http://api.kde.org/extragear-api/sdk-apidocs/kdevplatform/html *(KDevelop Platform API documentation)*
https://userbase.kde.org/KDevelop4 *(User documentation)*
https://techbase.kde.org/KDevelop5 *(Developer documentation)*

Other Communication:

https://forum.kde.org/viewforum.php?f=218 *(KDE KDevelop forum board)*
https://reports.kde.org/en/projects/kdevelop-extragear-kdevelop/commits_report *(KDevelop commit breakdown by author)*
https://bugs.kde.org/enter_bug.cgi?format=guided&product=kdevelop *(Bug tracking system for KDE community)*
https://phabricator.kde.org/dashboard/view/8/ *(Phabricator instance for KDE family of applications)*

Project Homepage:

https://www.kdevelop.org/

Developer Blogs:

https://www.kdevelop.org/developer-blogs

***

## Community Architecture Analysis ##

A.  Describe software project, its purpose and goals.

KDevelop is a cross-platform, multi-language integrated development environment (IDE) under the KDE Community banner. KDevelop is free and open-source software, providing support for a variety of markup and programming languages through its extensible plugin-based architecture with additional localization support in several languages. 

Most KDevelop contributors are volunteers who work on the project in their spare time, but, there are currently **four Core Developers**:

- [Kevin Funk](mailto:kfunk@kde.org) (Co-maintainer)
- [Sven Brauch](mailto:svenbrauch@gmail.com) (Co-maintainer)
- [Milian Wolff](mail@milianw.de) (Generic Manager)
- [Aleix Pol Gonzalez](aleixpol@gmail.com) (CMake/Run/Kross/Git Support)

KDevelop is a reliable and powerful environment for developers and is FLOSS software. As part of the KDE Community, this application also joins the goal of making a consistent Kool Desktop Environment.

B.  Give brief history of the project. When was the Initial Commit? The latest commit?

The earliest days of KDevelop found its first 0.1 Alpha version announced on the [kde-announce](https://marc.info/?l=kde-announce&m=90648146015087&w=2) mailing list - on September 22nd, 1998, developers Sandy Meier, Stefan Heidrich, and Stefan Bartel hosted the unstable tarball package on KDE's FTP server. KDevelop has changed significantly since those early days, and its most recent long term support (LTS) incarnation - [KDevelop4](https://github.com/KDE/kdevelop/releases/tag/v4.0.1) - was released nine years ago on July 16th, 2010 ([Commit 79ca761...](https://github.com/KDE/kdevelop/commit/79ca7610af2e303d7ed8940d4fd3798b9786d96e)).

It wasn't until the next year, on January 9th, 1999, that the initial work started on KDevelop was moved into a version control system ([Commit f12757c...](https://github.com/KDE/kdevelop/commit/f12757c0f4c72b06e9dd77b096250c6f04d7cae1)). Described as version 0.2, developers Meier, Heidrich, and Bartel were joined by Ralf Nolden, Jost Schenk, and David Barth. It was during this import into a git repository that the origins of the source code were documented. KDevelop's original source code drew from KWrite - a text editor in the KDE family maintained by Jochen Wilhemy - and that connection between the applications remains present today. At the time, KDevelop also included test code from 'kswallowwidget' that was later removed in the [next year](https://marc.info/?l=kde-commits&m=94979406811303&w=2).

At the time of writing this entry, the most recent commit ([Commit d5e3e27...](https://github.com/KDE/kdevelop/commit/d5e3e27bb2720d84adda95de07a728a9e61c866f)) to KDevelop's [master](https://github.com/KDE/kdevelop) branch was authored yesterday by Thibault North ([@tnorth](https://github.com/tnorth)) - a member of the Fedora project based in Switzerland - and committed by Milian Wolff ([@milianw](https://github.com/milianw)) - a core developer of KDevelop based in Berlin, Germany. The most recent release, [v5.3.2](https://github.com/KDE/kdevelop/releases/tag/v5.3.2) ([Commit 48bdc10...](https://github.com/KDE/kdevelop/commit/48bdc10109ca5c0db6938b9eb89ea6890212cbf8)) was published by Kevin Funk ([@krf](https://github.com/krf)), a co-maintainer of the KDevelop project, based in Cologne, Germany.

C.  Who approves patches? How many people?

According to the commit review reports on the project's [Phabricator](https://phabricator.kde.org/dashboard/view/8/) dashboard, there are a couple of consistent names that appear to be in charge of reviewing commits that are authored. While each of the core developers - Kevin Funk, Sven Brauch, Milian Wolff, and Aleix Pol Gonzalez - are listed as recurring reviewers, it seems that the option to review and approve patches are open to anyone willing to do the work.

The KDE Community even provides [documentation](https://community.kde.org/Infrastructure/Phabricator#How_to_review_someone_else.27s_patch) for new contributors who are interested in reviewing patches and performing quality assurance on new commits and pull requests. In practice, there were *five* unique reviewers that would approve commits.

D.  Who has commit access, or has had patches accepted?  How many total?

The GitHub [repository](https://github.com/KDE/kdevelop) (and by extension, its mirrors) list 282 unique contributors to the master branch (excluding merge commits). Of those contributors, only four contributors that have been active in the last three years have 1,000 or more commits. This being said, the numbers may be skewed as some core developers, like Milian Wolff, both author and approve patches. Of the contributors who are not presently reviewing patches through Phabricator, there are three with 1,000 or more commits. There are at least 25 other contributors with 100 or more commits over the lifetime of the project.

KDevelop's [homepage](https://www.kdevelop.org/kdevelop-team) lists 14 inactive core developers, 2 active contributors, and 4 remaining core developers. If including patches for localization efforts, there are roughly 9 different languages that have supporters.

In theory, anyone can contribute. Contributors who wish to join the project need only [contact](https://www.kdevelop.org/contribute-kdevelop) the core and active developers via the IRC channel or developer mailing list. Those who have created a new patch without going through that process can also post a request directly to the project's Phabricator instance. It seems that anyone who follows the developer documentation and reaches out can gain access.

E.  Who has the highest amounts of "Unique Knowledge?" (As per your "Git-by-a-bus" report. If there is a tie, list each contributor, with links if possible)

— Nic — 

F.  What is your project's "Calloway Coefficient of Fail?"

— Joshua — 

G.  Has there been any turnover in the Core Team? (i.e. has the same top 20% of contributors stayed the same over time? If not, how has it changed?)

— Joshua —

H.  Does the project have a BDFL, or Lead Developer? (BDFL == Benevolent Dictator for Life) If not, what is the structure of its leadership, and how is it chosen?

— Joshua —

I.  Are the front and back end developers the same people? What is the proportion of each?

— Joshua —

J.  What have been some of the major bugs/problems/issues that have arisen during development? Who is responsible for quality control and bug repair?

— Nic — 

K.  How is the project's participation trending and why?

— Nic — 

L.  In your opinion, does the project pass "The Raptor Test?" (i.e. Would the project survive if the BDFL, or most active contributor were eaten by a Velociraptor?) Why or why not?

— Nic — 
M.  In your opinion, would the project survive if the core team, or most active 20% of contributors, were hit by a bus? Why or why not?

— Nic — 

N.  Does the project have an official "on-boarding" process in place? (new contributor guides, quickstarts, communication leads who focus specifically on newbies, etc...)

There is a general [invitation](https://www.kdevelop.org/contribute-kdevelop) for contributors to contact developers on the IRC or through the mailing list if they want to get started. Unfortunately, there doesn't seem to be one, singular 'on-boarding' process that new contributors can utilize to get used to the process. A trip to the [linked documentation page](https://userbase.kde.org/KDevelop4) opens with another invitation for people to help extend the documentation itself; it can be overwhelming to join the project if you're not sure how to get started. The documentation that does point to something useful for new contributors was found on a [mirror repository](https://github.com/krf/kdevelop), as opposed to the main one.

O.  Does the project have Documentation available? How extensive is it? Does it include code examples?

There is several avenues for documentation - including for users, developers, and translators that are a part of the localization effort. Unfortunately, since the release of KDevelop5, the most recent documentation for developers and users has been lacking. With that said, KDevelop4 has been documented extensively. Discussion about using KDevelop also takes place across the many blogs by developers; KDevelop's homepage provides access to an [aggregate list](https://www.kdevelop.org/developer-blogs) that pulls from some of them.

P.  If you were going to contribute to this project, but ran into trouble or hit blockers, who would you contact, and how?

The core developers via IRC or the mailing list. Technically, you could contact the developers directly via their email, however, there's a better chance of getting a timely response when sending this feedback through the mailing list. In addition, conversations about challenges in the public space are healthier for the growth of any FLOSS community - archived discussions in the public space allow future developers the opportunity to learn from the past.

Q.  Based on these answers, how would you describe the decision making structure/process of this group?  Is it hierarchical, consensus building, ruled by a small group, barely contained chaos, or ruled by a single or pair of individuals?

— Joshua —

R.  Is this the kind of structure you would enjoy working in? Why, or why not?

— Personal responses required for this question. — 

***

### Presentation ###

The presentation is being created [here](https://slides.com/iae2784/deck). It is made with the Slides platform.

Slides is built with the help of many great open source frameworks and projects including [Iconic](http://somerandomdude.com/work/iconic/), [Font Awesome](http://fortawesome.github.com/Font-Awesome/), [Entypo](http://www.entypo.com/), [IcoMoon](http://icomoon.io/), [Broccolidry](http://icomoon.io/), [WebHostingHub Glyphs](http://www.webhostinghub.com/glyphs/), [Material Design Icons](https://github.com/google/material-design-icons/blob/master/LICENSE), [jQuery](http://jquery.com/), [Ace](http://ace.c9.io/), [Modernizr](http://modernizr.com/), [Moment.js](http://momentjs.com/), [Spectrum](https://github.com/bgrins/spectrum) and [KaTeX](https://github.com/Khan/KaTeX). The developers contribute back to the community by maintaining [reveal.js](https://github.com/hakimel/reveal.js), an open source HTML presentation framework.


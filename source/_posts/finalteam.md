---
title: 'Sugarlabs Activity: Team Proposal'
tags:
  - open-source
  - class
  - architecture
  - documentation
  - analysis
  - Sugarlabs
categories:
  - - blog
    - hfoss
date: 2019-04-2 01:52:05
---

# Sugarlabs Activity - Team Proposal #

This blog post serves as a proposal for the creation of an educational *activity* on the Sugar Desktop Environment. Sugar is a collaborative, open-source learning platform for children maintained by [Sugar Labs](https://sugarlabs.org/), the team behind the award-winning learning platform.

## Team Members ##

The core developers behind this proposal are members of the [Humanitarian Free and Open Source Software](http://hfoss.rocfoss.org) course and community at the [Rochester Institute of Technology](https://www.rit.edu/).

* Nic Hartley
* nxh9052@rit.edu

* Joshua Schenk
* jks7743@rit.edu

* Ian Effendi
* iae2784@rit.edu 

## Project Overview ##

Our team seeks to create a cohesive, unified platform experience for our activity's *learners*. Learners are tasked with practicing their mathematical foundations for fractional arithmetic operations, like whole number division and multiplication. We plan on using PyGame to power our activity. [PyGame](https://www.pygame.org/) is a game engine written in [Python](https://www.python.org/) and [C](https://en.wikipedia.org/wiki/C_(programming_language)), released under the [LGPL](https://en.wikipedia.org/wiki/GNU_Lesser_General_Public_License) license.

### Scenario 1 ###

In the first section, learners must weigh suitcases at baggage claim to make sure that they aren't over the safety limit. Suitcases are given a 'fraction' as a weight and they must decide whether it is equal, over, or under the safety limit - which will also be given a 'fraction' as a value.

### Scenario 2 ###

In the second section, learners are encouraged to slice pizza using the exact angles customers order. Learners can use their pointer device to select the exact lines and angles that they need, mimicing the experience of using a protractor digitally.

### Stretch Goal ###

Tying these elements together is a score system that learners can cash in at an in-activity, fictional storefront, where they can redeem points for unlockables. This third portion of the idea needs to be fleshed out - however, it serves as a thematic force that pulls it all together. Learnes who do best with extrinsic forms of motivation may find themselves revisiting the scenarios in order to do better. By keeping each slice of gameplay short, episodic, and replayable, we invite learners to revisit the work that they've done.

## Educational Goals ##

Our team will create a Sugar activity that targets users who are learning or reviewing 4th-grade level appropriate mathematics. The Sugar platform was born out of the international [One-Laptop-Per-Child](http://one.laptop.org/) project and every country's pedagogy and curriculum is different. For the sake of this project, we've examined some of the standards used in the United States' K-12 grade school system.

### 4th Grade Level Mathematics ###

According to the [Common Core State Standards Initiative](http://www.corestandards.org/Math/Content/4/introduction/), instructional time on mathematics for 4th grade students focuses on *three* ***critical areas***:

1. Developing understanding and fluency with **multi-digit multiplication**, and developing understanding of dividing to find quotients involving **multi-digit dividends**;
2. Developing an understanding of **fractional equivalence**, **addition**, and **subtraction** of fractions with like denominators, and **multiplication of fractions** by whole numbers;
3. Understanding that geometric figures can be **analyzed** and **classified** based on their properties, such as having **parallel sides**, **perpendicular sides**, **particular angle measures**, and **symmetry**.

For a time, the Math4Team maintained a [curriculum chart](https://wiki.sugarlabs.org/go/Math4Team/Resources/Curriculum_Chart) for 4th Grade mathematics on the Sugar Labs wiki. Based off of the [Massachusetts Curriculum Framework for Mathematics](http://www.doe.mass.edu/frameworks/current.html), there came to be a working list of standards and an accounting of Sugar activities that satisfied the implied learning goals. In review of both Massachusetts' and New York State's [Next Generation Mathematics Learning Standards](http://www.nysed.gov/common/nysed/files/programs/curriculum-instruction/nys-next-generation-mathematics-p-12-standards.pdf), one can find - at least for mathematics - that they all agree with the Common Core's emphasized *critical areas*.

### Enriching Learners with Technology ###

Today, digital media and entertainment that targets children are facing more scrutiny than ever before. Outlets have written about malicious content creators on social media platforms whose [disturbing videos](https://www.bbc.com/news/blogs-trending-39381889) - featuring animated violence and graphic content inappropriate for children - are hidden behind fake, but official-looking, artwork of characters children have become familiar with.

Sugar Labs has the [security goals](http://wiki.sugarlabs.org/go/Human_Interface_Guidelines#Security) to protect children against five categories of *bad things* software can do:

1. Damaging the laptop;
2. Compromising privacy;
3. Damaging the children's data;
4. Doing bad things to other people; and
5. Impersonating the child.

This is only one of Sugar's [key design principles](http://wiki.sugarlabs.org/go/Human_Interface_Guidelines/Design_Fundamentals/Key_Design_Principles). By reflecting on all eleven of them, can we move closer toward our goal of **enriching learners with technology**:

1. Performance
2. Usability
3. Simplicity
4. Reliability
5. Security
6. Adaptability
7. Recoverability
8. Interoperability
9. Mobility
10. Transparency
11. Accessibility

All of these principles, amongst other project topics for Sugar developers , were written into the [Human Interface Guidelines](http://wiki.sugarlabs.org/go/Human_Interface_Guidelines), published in 2006.

In the long run, our framework of 'episodic' mini-games could be focused around a returning core character that learners may find appealing - organizations such as [Sesame Workshop](https://www.sesamestreet.org/) leverage their IP to maintain a familiar atmosphere for learners amidst changing content. In a case with an unlimited amount of resources, I could envision creating a public domain character that other educational organizations and non-profits could use in order to create a hub of games that children easily recognize by titular characters. In some ways, a community sourced commons for edu-tainment.

## Assets ##

There are plenty of resources available online that host graphic art and sound assets in the public domain or licensed under compatible Creative Commons licenses. 

## Other Ideas ##

While deliberating on this, we thought of other game ideas for the proposed Sugar activity:
- Solving grade-appropriate math questions in a short amount of time for the following subjects:
    - Simplifying simple fractions
    - Add/subtract/multiply/divide small numbers
    - Maybe word problems?
    - Factorization
- Solving math puzzles to shoot missiles out of the sky before they hit the Earth.
- A clone of the [2048](https://en.wikipedia.org/wiki/2048_(video_game)) video game that focused on fractional math.
- A pizza cutting game that focused on complex fractions (instead of angles) that could be played like Fruit Ninja.
    - Learners are encouraged to cut the pizza quickly with no or little guidelines to help build their sense of 'fraction' size.
- Smoothie making game where you need the right portions. Those portions can be requested by randomly ordered/generated customers with a fraction and an ingredient.

*****

## Deadlines ##

These are the following deadlines we are planning to operate with:

| Date | Time | Assignment |
|------|------|------------|
| Thu, Apr 4 | 11:59 PM (EST) | Final Project: Proposal |
| Wed, Apr 17 | 11:59 PM (EST) |Final Project: Proof of Concept |
| Wed, Apr 24 | 11:59 PM (EST) | Final Project: Prototype |
| Fri, Apr 26 | 11:59 PM (EST) | Final Project: Playtest |
| Mon, Apr 29 | 11:59 PM (EST) | Final Project: Presentations & Peer Evaluations |
| Wed, May 1* | 11:59 PM (EST) | Exam - Final Project: Presentations |

*Final exam time is from 8:00 AM to 10:30 AM in room MSS-2175.

A more detailed timeline can be found below.

## Division of Labor ##

Nic and Ian have already worked together to get the [repository up and running](https://github.com/rimij405/hfoss-final-2019). Ian has started to look at PyGame. The original plan to have three individual mini-games was revisited after this length process. Instead, the team has decided to go with two scenarios. Whomever is unassigned to either of those two main scenarios is responsible for building the thematic connection between the two of mini-games and working on getting our game to play nice with the Sugar environment.

Ian created the timeline below in order to provide more context to what we expect to accomplish. After proposals are submitted and approved, we'll be able to tackle these in a consistent fashion. Prior to the next immediate milestone, our group seeks to be more specific and intentional behind the design of our mini-games.

## Workflow ##

On a quick note about workflow, we're interested in following a modified version of the [GitFlow](https://leanpub.com/git-flow/read) workflow, particularly using 'master', 'develop', and 'release' branches. We likely will not incorporate feature branches, putting our approach somewhere between GitFlow and [Trunk Based Development](https://trunkbaseddevelopment.com/). Any feature branches we do have will be short-lived (akin to Trunk Based) and any release branches will likely be merged back into the master (like GitFlow).

## Timeline ##

The following timeline shares an overview of the milestones we wish to complete, when we wish to complete them by, and the tasks we believe ought to be associated with them.

### Overview ###

| Date | Milestone | Key Deliverable |
|------|-----------|--------------|
| Thu, Apr 4 | M1 | +Completed Proposal |
| Tue, Apr 9 | M2A, M2B | +Technology, +Assets  |
| Tue, Apr 16 | M3 | +Proof-of-Concept |
| Sun, Apr 21 | M4 | +Prototype |
| Thu, Apr 25 | M5A | +Playtest Preparation |
| Sat, Apr 27 | M5B, M5C | +Playtest Revisions, +Presentation |
| Mon, Apr 29 | M6A, M6B | +Wiki Entry, +Release Build, +Peer Evaluations |

### Milestone 1: Complete project proposal ###

We aim to complete the final project's proposal as soon as possible. We will choose one main idea and then rank one or two backup ideas that we wouldn't mind doing in the event our proposal isn't accepted. They wouldn't be bad to have if our proof-of-concept and prototype also don't work out for the initial idea.

We will also make sure that we discuss everyone's skillset, programming language proficiency, past development experience, and external obligations or commitments that might impact our ability to do work.

**Deliverables:**
*Due: Thursday, April 4th, 2019*
- [x] [Request an account](https://wiki.sugarlabs.org/index.php?title=Special:UserLogin) for the SugarLabs Wiki.
- [x] Review the [Activities](https://wiki.sugarlabs.org/go/Activities) that already exist on the platform.
- [x] Review the [curriculum chart](https://wiki.sugarlabs.org/go/Math4Team/Resources/Curriculum_Chart) from the SugarLabs Wiki*.
- [x] Review the [NY State Math Standards](http://www.nysed.gov/curriculum-instruction/new-york-state-next-generation-mathematics-learning-standards) prior to coming up with an idea.
- [x] Discuss development experience, skillset, etc.
- [x] Determine one or two ideas for the final project.
- [x] Discuss the project proposal.
- [x] Individually submit blog post for final project proposal.

**We're not limited to the options on the curriculum chart, however.*

### Milestone 2: Pre-Production ###

For this milestone, we aim to set up our development environments and prepare a list of the assets that we need for the final project.

#### 2a: Technology ####

Our development environment and remote repository will be prepared by the end of this milestone.

**Deliverables**
*Due: Tuesday, April 9th, 2019*
- [ ] Review [application development guide for the OLPC X0-1 laptop using Python](https://www.ibm.com/developerworks/linux/tutorials/l-sugarpy/) from IBM.
- [ ] Review [contributor and developer documentation](https://github.com/sugarlabs/sugar-docs) from SugarLabs.
- [ ] Decide license* for the final project.
- [ ] Initialize repository on GitHub or GitLab with README, LICENSE, and .gitignore markup.
- [ ] Add '[Hello World](https://github.com/sugarlabs/hello-world)' starter project code (or [equivalent](https://github.com/FOSSRIT/sugar-quickstart)) to the project repository.
- [ ] Ensure project builds from local development environments without error.
- [ ] Backup stable build in a safe location.
- [ ] Decide on how documentation will be done for the final project.
- [ ] Rank project features in terms of completion priority; keep dependencies in mind.

**Suggestion: MIT License due to it's permissiveness?*

#### 2b: Assets ####

A fleshed-out list of the assets that we believe we'll need should be created at this time. This doesn't mean we'll collect our final assets - it only means we'll have temporary, placeholder assets ready and can prepare for the art that we need down the line, as we get closer to a minimal viable product.

**Deliverables**
*Due: Tuesday, April 9th, 2019*
- [ ] Determine content necessary for the game.
- [ ] Create a wireframe of the graphical user interface.
- [ ] Create storyboard of the menus and game screens necessary for the game/state machine.
- [ ] Create list of art assets that we must produce (UI?, Sprites?, Fonts?, Animations?).
- [ ] Create list of audio assets (SFX?, BGM?).
- [ ] Find art assets with a compatible license.
- [ ] Find audio assets with a compatible license.
- [ ] Create preliminary attribution or credits text file that list assets we intend to use.

### Milestone 3: Proof-of-Concept (POC) ###

The proof-of-concept demonstrates the feasibility of the activity's single core feature. This will depend on what we decide the game should be. This differs from a minimal viable product and a prototype in scope.

**Deliverables**
*Due: Tuesday, April 16th, 2019*
- [ ] Choose single core feature that we wish to demonstrate.
- [ ] Complete the proof-of-concept.
- [ ] Add additional features, if time permits.
- [ ] Patch and revise proof-of-concept, if necessary.
- [ ] Test proof-of-concept build made in a fresh local environment.
- [ ] Test proof-of-concept build made on lab machines.
- [ ] Backup stable build in a safe location.
- [ ] Submit proof-of-concept to 'poc' branch on remote repository.
- [ ] Merge changes into master branch once stable, if necessary.
- [ ] Update documentation with installation instructions.
- [ ] Update developer documentation to be more informative.

### Milestone 4: Prototype ###

The prototype is larger in scope than a proof-of-concept, but, it is not necessarily to the scope of a minimal viable product. The expected features for this milestone change depending on the game being developed.

**Deliverables**
*Due: Sunday, April 21st, 2019*
- [ ] Fix bugs from previous milestone.
- [ ] Patch and revise prototype based off of peer feedback.
- [ ] Add remaining features to prototype.
- [ ] Test prototype build made in a fresh local environment.
- [ ] Test prototype build made on lab machines.
- [ ] Backup stable build in a safe location.
- [ ] Submit prototype to 'prototype' branch on remote repository.
- [ ] Merge changes into master branch once stable, if necessary.
- [ ] Update documentation with installation instructions.
- [ ] Update developer documentation to be more informative.

### Milestone 5: Polish, Patch, & Present ###

This milestone is about wrapping up loose ends, polishing rough features, and patching out any remaining bugs with the program. This is split between the playtest and the presentation.

#### 5a: Playtest Preparation ####

The playtests will take place on *Wednesday, April 26th, 2019*. There are several steps that we can take in order to prepare for the playtests.

**Deliverables**
*Due: Thursday, April 25th, 2019*
- [ ] Fix bugs that prevent the prototype from building.
- [ ] Prepare user documentation for a student. (Language must be simple).
- [ ] Prepare user documentation that might accompany a parent/teacher/caregiver.
- [ ] Ensure instructions in-app are clear and proofread.
- [ ] Ensure a stable build can be run from the lab machines.
- [ ] Ensure a stable build is on someone's flash-drive for the playtest.

#### 5b: Polish ####

After the playtests, our focus should be on polishing work using the feedback we collect. This means resolving any outstanding bugs or feature requests in order to have our minimal viable product.

**Deliverables**
*Due: Saturday, April 27th, 2019*
- [ ] Fix bugs from previous milestone.
- [ ] Patch and revise MVP based off of peer feedback.
- [ ] Add remaining features to MVP.
- [ ] Test MVP build made in a fresh local environment.
- [ ] Test MVP build made on lab machines.
- [ ] Submit MVP to 'MVP' branch on remote repository.
- [ ] Merge changes into master branch once stable, if necessary.
- [ ] Update documentation with installation instructions.
- [ ] Update developer documentation to be more informative.

#### 5c: Present ####

There are a specific set of questions that need to be answered in a post-mortem presentation. To ensure we cover all the parts on the rubric, the generative questions have been listed as some of the tasks below. The presentation will be given on one of two days: either *Monday, April 29th, 2019* or *Friday, May 1st, 2019*

**Deliverables**
*Due: Saturday, April 27th, 2019*
- [ ] Record screenshot/capture video recording of application usage.
- [ ] Slide: About the project. What is it? What are its main mechanics?
- [ ] Slide: Is the code clearly licensed under an OSI-compatible license?
- [ ] Slide: How does the code work?
- [ ] Slide: What are some of the best pieces of software you wrote? Why?
- [ ] Slide: What are some of the worst pieces? Why?
- [ ] Slide: Does your source repository contain clear written instructions for future developers? (eg. How to setup their environment to work on your project?)
- [ ] Slide: What <TODO> items did your team leave remaining?
- [ ] Slide: Does it work on python on a normal machine?
- [ ] Slide: Does it work on Sugar?
- [ ] Slide: What do you think of your code quality and git commit history?
- [ ] Slide: Did you make a wiki entry at sugarlabs.org?
- [ ] Slide: What stumbling blocks were there?
- [ ] Slide: What successes?
- [ ] Slide: What would you have done differently?
- [ ] Slide: What would you have worked on if you had more time?
- [ ] Proofread the slides before the presentation.
- [ ] Ensure presentation is formatted correctly when in performance mode.

### Milestone 6: Publish ###

The final milestone is mostly about submitting outstanding work.

#### 6a: Publish Project Files ####

This requires us to publish our files and write information on the Sugarlabs wiki.

**Deliverables**
*Due: Monday, April 29th, 2019*
- [ ] Create entry and link to the project information to the [RIT Math4Team projects wiki page](http://wiki.sugarlabs.org/go/Math4Team/RIT/Projects).
- [ ] Add appropriate user documentation to the wiki.
- [ ] Add appropriate developer and contributor documentation to the wiki.
- [ ] Merge outstanding (stable) changes to the master branch.
- [ ] Test `master` branch build in a fresh local environment.
- [ ] Test `master` branch build on lab machines.
- [ ] Release binaries for production usage.

#### 6b: Submit Peer Evaluation ####

This follows the rubric's expectations for peer evaluation.

**Deliverables**
*Due: Monday, April 29th, 2019*
- [ ] Write 200-1000 words, per teammate in your individual evaluation.
- [ ] Indicate what your teammates contributed to the project.
- [ ] What skills did they pick up this semester?
- [ ] What skills should they develop further?
- [ ] Give a numeric score (1-10) for them and justify it.
- [ ] Email your evaluation to your [instructor](mailto:deejoe@mail.rit.edu).
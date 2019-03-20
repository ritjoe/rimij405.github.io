---
title: "Literature Review #1: Bug Reporting"
date: 2019-01-30 22:16:03
categories: 
- [blog, hfoss]
tags:
- open-source
- class
- bugs
- issues
- documentation
- reading
photos:
- /images/posts/lit-review-1/documentation.jpg
---

# Review: How to Report Bugs Effectively #

This is the first of several literature reviews for content relevant to the humanitarian free and open source software course. In this entry, I will be reviewing *[How to Report Bugs Effectively](https://www.chiark.greenend.org.uk/~sgtatham/bugs.html)* by [Simon Tatham](https://www.chiark.greenend.org.uk/~sgtatham/).

<!-- more -->

***

![Image of laptop with code.](/images/posts/lit-review-1/coding.jpg)

## The Basics ##

At the start of the essay, the author, Simon Tatham, modestly titles himself a professional and free-software programmer. Tatham, however, is famous for creating and maintaining [PuTTY](https://en.wikipedia.org/wiki/PuTTY), an open-source implementation of Telnet and Secure Shell (SSH) clients for Unix and Windows platforms. It's fair to say that Tatham has experience with reporting and solving bugs in open-source software.

From the jump, Tatham plainly states the purpose of this guide: reading it will help developers write, "clear, helpful, *informative* bug reports." By appraoching the written work with prepared examples and instances of unhelpful reporting practices, Tatham is able to help readers troubleshoot their own bug reporting practices. Notice you're following a bad practice - this enables you to safely learn from that mistake and adjust course.

You can find this essay on Simon Tatham's personal website, [here](https://www.chiark.greenend.org.uk/~sgtatham/bugs.html).

## The Gist ##

This guide helps users report bugs to programmers. It's written in such a way that it prescribes approaches that the user can undertake when reporting a bug. It is precise, in explaining just how important detail is to the programmer, for users reporting bugs.

***

![Photo of a lightbulb doodle, pinned to corkboard.](/images/posts/lit-review-1/good-idea.jpg)

## The Good ##

- 1) Clear, practical examples that a user can review (if given the time) for writing their own bug reports. (The poor formatting, however, is Bad item #1).
- 2) The summary at the end of the entry is something that I wish more articles and blog posts had, especially when it comes to development and software tutorials.
- 3) It comes in several different languages!

***

![Image of someone staring at a laptop with concern.](/images/posts/lit-review-1/thinking.jpg)

## The Bad ##

- 1) The lack of spacing and formatting on the webpage makes it very diffiuclt to read. I want to be able to come back to this page while writing a bug report, scan for advice on the section I'm writing, and complete my report as quickly as possible.
- 2) This is written from the perspective of the user and the user alone. While useful for other developers for providing informative bug reports, the generalized presentation doesn't help programmers know what questions to ask. That process is something you'll learn largely from practice, experience, and a strong understanding of the codebase. This isn't necessarily a bad thing, but, this can be a barrier for new contributers.
- 3) It doesn't mention what users should do in the event repositories are archived. I think it would have been a good note to address what options they have - even one as simple as, "Find a new project that fulfills your needs if you don't have the time/resources/skills to continue working on this one."

***

![High exposure photograph of a question mark drawn with neon light.](/images/posts/lit-review-1/questionmark.jpg)

## Q&A ##

- 1) Is this work up-to-date? Are there new best practices for reporting bugs?
- 2) What cases are there where a user shouldn't freeze and should try to act quickly to document the issue?
- 3) What about situations where an open-source project is led by programmers who aren't receptive to beginners filing incomplete bug reports and are rude about it? Should there be dedicated bug handlers? Does it factor into the decision to make a hostile fork?

***

## Follow-Up ##

If I'm being honest, as I am reading this for class, a lot of this was already clear to me due to best practices in communicating issues that need debuging among team members in my past programming projects. That being said, I would agree that this is an essential read for those looking to get involved with bug reporting and helping with documentation.
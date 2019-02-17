---
title: "Meetup: BrickHack V"
date: 2019-02-17 12:02:02
categories: 
- [blog, hfoss]
tags:
- open-source
- hackathon
- meetup
- nodeJS
- react
- mental health
photos:
- /images/posts/brickhack-v/brickhackv.png
---

# [BrickHack V](https://brickhackv.devpost.com/) #

**BRICK CITY'S PREMIERE HACKATHON**

> [BrickHack](https://brickhack.io/) brings **designers, developers, and all sorts of makers** together for 24 hours to create something from nothing. Mentors and industry representatives will lend expertise and watch as you dive into **learning, developing, and producing a unique project**. Expect lots of free food, swag, coffee, and all-you-can-print 3D printers! From the novices to the experts, from designers to enginers, **this one's for you!**

See this video below for a recap of BrickHack 2018.

{% youtube 0fOUf1JwzBs %}

## The Event ##

BrickHack V took place between February 16th and February 17th of 2019. Hacking ran from 12:30 PM - 12:30 PM, and I was there for every second!

BrickHack is an annual invention marathon open to any student (that registered in advance). This year, BrickHack's fifth event took place in the Clark Gym located on the Rochester Institute of Technology's campus. There were over **600 participants** at this year's hackathon - all of them broke into groups (or worked alone) and had 24 hours to invent, create, learn, build, and innovate!

Students from Cornell, Binghamton, NYU, Waterloo, University of Toronto, Northeastern, UMass, RPI, and Univesity of Buffalo (as well as some CUNY students), were in attendance!

### Venue & Vendors ###

BrickHack is sponsored by many companies, but, a significant amount of support is given to [CodeRIT](https://coderit.org/) by the [Major League Hacking](https://mlh.io) (MLH) organization. MLH is the official student hackathon league; they support over [200 weekend-long invention competitions](http://mlh.io/events) every year and have cultivated the skills of more than **65,000** students around the world.

Missed the event? There were several sponsors present (such as [Wegmans](https://www.wegmans.com/), [Datto](https://www.datto.com/), [Google](https://www.google.com/), and much, much more). Some vendors, like [Verizon](https://www.verizonwireless.com/), were touting the *edge-of-their-seats-blazing-fast* **5G** technology. Others were more than excited to get students to create more things with their products, like [Unity3D](https://unity3d.com/). 

Many of these groups sponsored food, dinner, and talks meant to encourage students to take their development and hacking careers in new directions.

Unity held a workshop regarding careers and their famous game engine. A representative from [ACV Auctions](https://www.acvauctions.com/) - a company specializing in automotive consumer resale - spoke about working at their company. Wegmans spoke about the importance of data, and encouraged groups to reuse and remix their public data to reshape a narrative in interesting ways.

### Highlights ###

Participating groups had the chance to submit their projects for the chance to win certain prizes, based on criteria posted near the start of the event. Over **$19,304** were offered in prizes!

Some of the more notable prizes were:

- Datto's Most socially impactful project.
- RIT's Simone Center's Most Commercially Viable Product.
- BrickHack's 'Hack Our Health' award for the product and/or application with the most promise in benefiting the mental health needs of college students.
- Verizon's Best use of 5G currencies in immersive media.
- and, Unity's Best Game, among many others...

## Mood Swing ##

![Logo for Mood Swing](/images/posts/brickhack-v/logo.png)

> "Track your mood across several days and see an overview of how you've felt."

We created a mood tracker application that allows users to take control of their own data. Users can self-host a MongoDB instance and interface with it using our code to keep track of their mood (a range from happy to sad), hours of exercise, hours of sleep and cups of coffee in the last day.

This application was built with: `javascript`, `react`, `bash`, `git`, `mongodb`, `mongoose`, `node.js`, `lucidchart`, `google-chart`, `vscode`, `vim`, `nano`, `visual-studio`, `webstorm`, `trello`, `google-drive`, `discord`.

### A Look at the Team ###

Taking the initials from our team, we came up with the name 'Chef Bicc'. Take a look at who made this product:

Carson Bloomingdale 
{ [DevPost](https://devpost.com/carsonbloomingdale)
[Portfolio](https://carsonbloomingdale.com/) }
> Carson worked on the front-end, implementing ReactJS in order to showcase the Mood visualization.

Claire Chen
{ [DevPost](https://devpost.com/ClaireChen)
[Portfolio] }(https://www.linkedin.com/in/claire-chen-a4a288172)
> Claire helped develop behaviors on the React-powered client.

Ian Effendi
{ [DevPost](https://devpost.com/rimij405)
[Portfolio](https://rimij405.github.io/) }
> I worked on the REST API (powered by an Express.JS server) that powers the application's tracking abilities. I created controllers, models, and routes, using a mongoose module to handle connecting to MongoDB.

Henry Farr
{ [DevPost](https://devpost.com/hfarr)
[Portfolio](https://www.linkedin.com/in/henry-farr-a191b6172) }
> Henry hosted the production webserver on his personal system; this project was his first time using NodeJS (and JavaScript in general).

### Features ###

We knew that we wanted to create an open-source application that could track personal data and empower those who stick with the program.

Our original idea was to allow users the chance to select a daily mood from a series of emoji, and, allow them to show an average 'mood' based on a date range that they chose. In addition to mood, users would be able to keep track of other daily life events (such as drinks of water, hours of sleep, hours of exercise, and meals in one day). From there, users are able to take the data they own and visualize the results across a day, a week, a month, and even a year.

### The Frontend(s?) ###

We created an intentionally detached API for the backend to allow a community of mindful users the opportunity to create a cross-platform ecosystem.

Our interpretation resulted in a React-powered web client, but, there was discussion of creating a native Flutter/Dart mobile application.

### The Backend ###

The exposed API is powered by [MongoDB]() and [NodeJS](). We want to make sure that our backend remains scalable and accessible from multiple endpoints: each mood entry is stored in a Binary JSON (BSON) format, taking up little space while remaining quick to query. 

The data itself is flexible and the JSON document format offers many avenues to converting for use in other ecosystems. The goal of keeping the backend detached is to keep development agile and flexible. 

NodeJS's non-blocking I/O was perfect for our needs. We had to choose between a [SOAP-style](https://www.soapui.org/learn/api/soap-vs-rest-api.html),  a [REST-style](https://medium.freecodecamp.org/building-a-simple-node-js-api-in-under-30-minutes-a07ea9e390d2), and a [RPC-style](https://scotch.io/@alloys/how-to-build-an-rpc-based-api-with-nodejs) API. 

SOAP wraps payload information in an XML format, making it language-agnostic. REST models domain resources and entities, making CRUD operations available for all the data. RPC is great for interacting with the backend through commands/procedures.

At the end of the day, we chose to go forth with an RPC API. But nothing's stopping us from adding to our system. The API endpoint contains, importantly, an 'API Version' field that can be queried to choose how we (and others) want to handle their data in the future.

### Data Ownership ###

![Screenshot from the application.](/images/posts/brickhack-v/screenshot.jpg)

We've released the code under the permissive open-source [MIT License](https://opensource.org/licenses/MIT) to encourage other people to take control of their data, and keep track of their mental health without having to pay for an application.

Use the `frontend` branch to get access to a react-based web-client. Use the `backend` branch to get access to the MongoDB-powered data store.

Or, write your own frontend to interface with the API!

You just need a place to host the database!

## Post-Mortem ##

### Challenges ###

We split up into two groups to tackle two sides of this application. We wanted to make sure our client was detached from the backend; getting from a prototype to a place where we could cleanly test functionality in the client took work. The biggest challenge came down to communicating endpoint expectations and clarifying how our JSON payloads (for both requests and responses) would interact.

### Next Steps ###

Encouraging developers to build upon the framework we've laid out is a great start! That said, we have more features in mind. We entertained creating a cross-platform suite of clients and thought about using Google's Dart/Flutter combo to create a robust native mobile client.

## See More ##

[DevPost Submission](https://devpost.com/software/brickhack-v-chefbicc)

[GitHub Repository](https://github.com/rimij405/brickhack-v-chefbicc)
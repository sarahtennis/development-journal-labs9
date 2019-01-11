---
templateKey: blog-post
title: Week 1 in Labs9
date: 2019-1-11T12:00:10.000Z
description: The Coffee Taster’s Flavor Wheel, the official resource used by coffee tasters, has been revised for the first time this year.
tags:
  - labs9
---

## Project
# Knowledge Without College

Knowledge Without College is a job board that connects employers with talented job seekers who may not have a college degree. This paid job posting service encourages employers to emphasize the skills desired in an employee rather than focusing on formal education.

## Team Progress

GitHub Handle: sarahtennis

![contribution graph](/img/week-1-contribution-graph.png)

## Tasks Pulled

### Front End
* Ticket 1
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/10
  * Trello: https://trello.com/c/GFkaxsJE/38-sign-up-email
* Ticket 2
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/10
  * Trello: https://trello.com/c/0EmnZy7C/39-sign-in-email
* Ticket 3
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/10
  * Trello: https://trello.com/c/BAi1jGih/40-sign-out
* Ticket 4
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/28
  * Trello: https://trello.com/c/RNP7HpdY/49-react-organization

### Back End
* Ticket 1
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/2
  * Trello: https://trello.com/c/A400GlZq/37-build-express-server
* Ticket 2
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/17
  * Trello: https://trello.com/c/deQrTgBO/48-additions-to-migrations

## Analysis

My most difficult task this week was implementing Firebase authentication (Tickets 1-3 for the Front End). Having no previous experience with this service, a lot of time was spent reading documentation and looking through tutorials and examples. A thorough tutorial that I ended up using with the Firebase documentation was: https://www.robinwieruch.de/complete-firebase-authentication-react-tutorial/. 

The process for creating an account through Firebase is straight-forward and intuitive. Once the account is created, you are provided with configuration variables that will be needed for the client to interact with the authentication system. Next, I followed the tutorial to implement Firebase within our React app. As an optional addition, I added React context to prevent multiple instances of Firebase for a single client and to make passing authentication data through the app easier.

The Firebase documentation provides functions for communicating from the front end. Currently I have sign up and sign in working for accounts using email and password, as well as sign out that will be accessible for all forms of authentication. These functions were tested manually through basic forms and buttons and verified through the Firebase online console.

![firebase users](/img/week-1-firebase.png)

## Reflections

This is my first time working on the same project with multiple people, and it is hard! For our previous projects I worked alone and got used to doing things "my way." Learning to accept compromise and not try to be involved in everything are two of my personal goals.

From the beginning our group dynamic has been comfortable with all members contributing to discussions. I tried to help solidify the group by discussing guidelines and the project structure, but my approach was a little controlling. In the coming weeks I'm going to work on taking a step back and focusing on my own assigned tasks.

Overall I appreciate how well we work together and look forward to building an awesome project with my team members.

## Milestone

### Deployment Links
 
* Front End: https://knowledge-without-college.netlify.com/
* Back End: https://knowledge-without-college.herokuapp.com/
  * Use /test to view server response.

### User Models

* ![user model](/img/week-1-user-model.png)
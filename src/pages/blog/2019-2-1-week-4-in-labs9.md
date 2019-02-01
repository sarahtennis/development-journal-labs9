---
templateKey: blog-post
title: Week 4 in Labs9
date: 2019-2-1T12:00:10.000Z
description:
tags:
  - labs9
---

## Project
### Knowledge Without College

Knowledge Without College is a job board that connects employers with talented job seekers who may not have a college degree. This paid job posting service encourages employers to emphasize the skills desired in an employee rather than focusing on formal education.

## Team Progress

GitHub Handle: sarahtennis

![contribution graph](/img/week-4-contribution-graph.png)

## Tasks Pulled

### Front End
* Ticket 1
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/160
  * Trello: https://trello.com/c/8F6AvUut/99-default-avatar
* Ticket 2
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/148
  * Trello: https://trello.com/c/Z1jixVnc/98-new-account-information-form-new-design
* Ticket 3
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/142
  * Trello: https://trello.com/c/AA2rYyVO/91-sign-up-single-jop-vieww
* Ticket 4
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/142
  * Trello: https://trello.com/c/IwScbThf/92-reset-password
* Ticket 5
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/135
  * Trello: https://trello.com/c/K1G1xRwS/90-sign-in
* Ticket 6
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/155
  * Trello: https://trello.com/c/qf2bY49k/101-sign-in-sign-up-redirect

## Analysis

This week the focus was on create a professional look for the project. One of my team members made mock-up design files for each page at three different break points. From here we divided the views between us and started working on the basic structure of each page. After everyone finished the desktop view, we met to discuss the smaller details that would help give the project a cohesive look (ex. padding, margins, font sizes, etc.).

I had the sign up, sign in, and reset password views and the new account information modal. The most difficult aspect of the design for me was creating a responsive full page background. My solution was to use a large, non-repeating url background with the background-size value cover, but the images used currently load slowly so I am going to look into compressing image files without losing quality or size to create a better user experience.

![sign in view](/img/week-4-styling1.png) 

In addition to styling the new account information modal, I also corrected the sign in and sign up redirect logic and conditinoally displayed the modal on the landing page depending on if an authenticated user has already filled out the form. As a group we discussed wanting to strongly encourage the user to fill out the form, but not force him to if it is inconvenient at that time.

![new account modal](/img/week-4-styling2.png)

One task that I picked up was to create a default avatar image for users who did not upload a new image. Originally I tried to find a license free image that we could use, but ended up creating my own in GIMP to avoid needing to credit an external source. I hosted my image on ImageShack with a trial account, but will need to move it somewhere else after the trial ends.

The new account information modal will set the user's 'avatar_image' within the database to the url for the default avatar if he does not upload another image through Cloudinary. I also manually went through the deployed database and added the url to the accounts with empty 'avatar_image' values to avoid having to log into each test account.

![default avatar](/img/week-4-default-avatar.png) 

## Reflections

## Whiteboard Interview

* Min Heap: https://youtu.be/Yft3kYjlCMo

## Milestone

### Deployment Links
 
* Front End: https://knowledge-without-college.netlify.com/
* Back End: https://knowledge-without-college.herokuapp.com/
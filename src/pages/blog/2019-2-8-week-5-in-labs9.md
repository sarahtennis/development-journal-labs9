---
templateKey: blog-post
title: Week 5 in Labs9
date: 2019-2-8T12:00:10.000Z
description:
tags:
  - labs9
---

## Project
### Knowledge Without College

Knowledge Without College is a job board that connects employers with talented job seekers who may not have a college degree. This paid job posting service encourages employers to emphasize the skills desired in an employee rather than focusing on formal education.

## Team Progress

GitHub Handle: sarahtennis

![contribution graph](/img/week-5-contribution-graph.png)

## Tasks Pulled

### Front End
* Ticket 1
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/194
  * Trello: https://trello.com/c/cyn1A98k/103-rehost-default-avatar
* Ticket 2
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/185
  * Trello: https://trello.com/c/Ly64B3B7/110-standardizing-button-colors-transitions
* Ticket 3
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/194
  * Trello: https://trello.com/c/wMvTr6So/114-bug-race-condition-settimeout-in-update-profile-component
* Ticket 4
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/194
  * Trello: https://trello.com/c/jPqI4P5L/115-bug-unable-to-set-active-collegedegree-to-false-in-edit-job-view-after-initial-creation

### Documentation
* Ticket 1
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/173
  * Trello: https://trello.com/c/7XtGWXPs/13-readme
  * Content Provided: Data Models, PostgresQL Set up, Firebase
* Ticket 2
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/168
  * Trello: https://trello.com/c/mtvOadtN/113-license-file

## Analysis
The majority of the work I completed this week was fixing bugs after manually testing the project as a user and helping with documentation. I was not able to finish as much as I had intended due to sickness, but I can always work on it more before the WEB14X Capstone Defense.

I went through and made sure that all links and buttons had the same animation and color scheme based on action type. They are currently using the same simple transition on hover.

![hover animation](/img/hover-animation.gif)

Within the update profile component a race condition was being handled using setTimeout, but this delay still did not guarantee that the component had access to a user object in props before making a server request (in which case the browser throws an error). To fix this, I added a state boolean to track if the server request had been attempted. In componentDidMount, if the user object was truthy on mount then the boolean would be set to true and the server request would be fired. I added logic for componentDidUpdate that if the request had not been attempted and the user object was truthy on update, set the boolean to true and send the request.

![race condition fix](/img/race-condition.png)

After handling the race condition, the render function of the update profile component displays:

<table style="border: 1px solid black;">
<tr><td><em>Condition</em></td><td><em>Display</em></td></tr>
<tr><td>Undefined user object in props</td><td>Loading image</td></tr>
<tr><td>Null user object in props (no authenticated user)</td><td>Redirects to landing page</td></tr>
<tr><td>Truthy user object, no account information in database</td><td>New account information modal</td></tr>
<tr><td>Truthy user object, account information in database</td><td>Account information with edit, change password, and billing actions</td></tr>
</table>

## Reflections
Mid-week I got sick and spent the majority of a day in urgent care and then the ER for very minor surgery. Through this my team members have been unbelievably kind. I felt as though I did not pull my weight this week, not a feeling I like, but they took care of everything I couldn't help with. Once we redo the video for the WEB14X Capstone Defense I will make sure to contribute as much as possible.

Labs has been a stressful, educational, and in the end rewarding experience.

## Milestone

### Deployment Links
 
* Front End: https://knowledge-without-college.netlify.com/
* Back End: https://knowledge-without-college.herokuapp.com/
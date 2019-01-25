---
templateKey: blog-post
title: Week 3 in Labs9
date: 2019-1-24T12:00:10.000Z
description:
tags:
  - labs9
---

## Project
### Knowledge Without College

Knowledge Without College is a job board that connects employers with talented job seekers who may not have a college degree. This paid job posting service encourages employers to emphasize the skills desired in an employee rather than focusing on formal education.

## Team Progress

GitHub Handle: sarahtennis

![contribution graph](/img/week-3-contribution-graph.png)

## Tasks Pulled

### Front End
* Ticket 1
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/108
  * Trello: https://trello.com/c/dG34yVzg/15-add-edit-job-page
* Ticket 2
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/106
  * Trello: https://trello.com/c/dG34yVzg/15-add-edit-job-page
* Ticket 3
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/106/
  * Trello: https://trello.com/c/RTYxEKY8/76-billing-page

### Back End
* Ticket 1
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/102
  * Trello: https://trello.com/c/CC2el3OR/79-finalize-jobs-server-endpoints
* Ticket 2
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/95
  * Trello: https://trello.com/c/RWOdFllr/77-search-categories
* Ticket 3
  * GitHub: https://github.com/Lambda-School-Labs/labs9-job-board/pull/86
  * Trello: https://trello.com/c/1dB6vozM/68-user-creation

## Analysis

My largest contribution this week was finalizing the server end points for the jobs table and connecting them to the Post Job, Edit Job, and Billing pages on the front end. 

I created an end point to receive all jobs for a user, but the only user reference easily available to the front end is the one provided by Firebase. To receive the jobs for each user I had to do an inner join between the 'jobs' and 'users' table and made sure not to include anything from the 'users' table.

On the front end, the necessary component does not always receive the Firebase id before componentDidMount is called so I used conditional statements to make sure the id has been received before requesting the user's jobs from the server.

![get jobs by user](/img/week-3-get-jobs-by-user.png) ![fetch jobs](/img/week-3-fetch-jobs.png)

A friend of mine has always preached, "Protect your database!" When I was creating the post and put requests for jobs, I used a basic data types objects to prevent the database from seeing malformed data. I tested the end points in development and production.

![update job](/img/week-3-update-job.png) ![data types object](/img/week-3-data-types-object.png)

## Reflections

This week was probably the most stressful. With the shortened week due to holiday the group spent some late nights working on finishing the MVP functionality. The project is starting to come together though and is nearly feature complete. We have had to spend a lot of time fixing small bugs once code that worked locally has been deployed and that has definitely slowed us down.

## Whiteboard Interview

* Minimum Number of Jumps: https://youtu.be/8E-ER5c9UD4

## Milestone

### Deployment Links
 
* Front End: https://knowledge-without-college.netlify.com/
* Back End: https://knowledge-without-college.herokuapp.com/
  * Use /test to view server response.
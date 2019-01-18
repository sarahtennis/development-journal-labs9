---
templateKey: blog-post
title: Week 2 in Labs9
date: 2019-1-18T12:00:10.000Z
description:
tags:
  - labs9
---

## Project
### Knowledge Without College

Knowledge Without College is a job board that connects employers with talented job seekers who may not have a college degree. This paid job posting service encourages employers to emphasize the skills desired in an employee rather than focusing on formal education.

## Team Progress

GitHub Handle: sarahtennis

![contribution graph](/img/week-2-contribution-graph.png)

## Tasks Pulled

### Front End
* Ticket 1
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/65
  * Trello: https://trello.com/c/ZY8zKf1R/55-redirect-page
* Ticket 2
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/73
  * Trello: https://trello.com/c/VA0cqoB3/64-side-menu-views-based-on-login-status
* Ticket 3
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/42
  * Trello: https://trello.com/c/wcFgCNez/31-auth-with-firebase
* Ticket 4
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/65
  * Trello: https://trello.com/c/AXv4WgyY/65-remove-facebook-oauth

### Back End
* Ticket 1
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/49
  * Trello: https://trello.com/c/1UKixyZs/56-login-table-migrations-seeds
* Ticket 2
  * Github: https://github.com/Lambda-School-Labs/labs9-job-board/pull/65
  * Trello: https://trello.com/c/WWOAHf25/67-change-from-sqlite3-to-postgresql-in-development

## Analysis

This week I cleaned up the authentication functionality and added a redirect page when signing in with Google OAuth. I removed Facebook OAuth for now (commented out within the code and disabled on the Firebase console) to prevent uncommon use cases while working toward the minimum viable product.

Originally I used React context to manage the authenticated user, but I'm in the process of reworking the authentication files to pass the authenticated user as props instead to make it easier to access during development. I spent a lot of time researching how other developers handle the authentication state.

![sign-up](/img/sign-up.png)

![sign-in](/img/sign-in.png)

![reset password](/img/reset-password.png)

## Reflections

After some difficulties with our back end deployment, things starting picking up!

It has been getting easier to work in a group. We keep a group video chat open at all times, but we divide up the work and conquer. We completed the milestone requirements for this week and discussed which parts of next week's milestone we'd each start on.

## Milestone

### Deployment Links
 
* Front End: https://knowledge-without-college.netlify.com/
* Back End: https://knowledge-without-college.herokuapp.com/
  * Use /test to view server response.
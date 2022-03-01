# Week 2 tasks

This week we start development! Have a look at the role(s) you are fulfilling on what your tasks are.

> This week, the mentors will be a little more available than normal to help get a good start. The education director will also be at the meetings to make sure that everything is going well and/or answer any questions about what to do in certain situations. This is only for this week, during the next week(s) the amount of support will get lowered until you can do it all yourselves.

Have a look at the [tips](../TIPS.md) for a successful project.

# Week tasks:

- 1. Daily meeting organiser specifics
- 2. (Dev) Developer tasks
- 3. (QA) QA Engineer tasks
- 4. Getting settled in

## 1. Daily meeting organiser specifics

If you are the daily meeting organiser you have an extra task this week. Every day on the time decided on Sunday it is up to you to share a link to a video conference. To facilitate the meeting, have every team answer the following questions:

- What did you do yesterday?
- What will you do today?
- Are you blocked?

Avoid vague answers like 'I worked on my feature' or 'I will fix a bug' as that doesn't help anyone. The goal is to give everyone an idea of where you are or what you are going to do so that everyone can place the code you are writing in the bigger context or even give tips on how to solve the problem you are facing.

For example, if someone says that they are going to build a context today to provide multiple components with access to the logged in user name, someone else may say that if they could add the e-mail to the context as well it would help out with their feature.

Remember that a sprint is a team game and it will help you so much to understand the code base if you have an idea what everyone is working on.

If someone is blocked, it is time to figure out how to unblock them. If they are waiting for another team to finish, the other team may need to shift priorities or already push part of their code to allow the first to continue. If they are stuck on some problem, it is up to the whole group to decide who is needed to help fix the problem and reprioritize the tasks for the day.

## 2. (Dev) Developer tasks

If you are a Developer, you will have the following responsibilities every week:

- On Sunday you will get assigned a feature and a group. As that group you are responsible for building that feature that week and will demo it in the next Sunday's meeting. The QA team will fill the ticket with test scenario's
- If another team needs a code review then the rest of the team needs to prioritise it to get the PR through. Every PR requires 2 other developers to approve the code that goes in and should not be merged until that is the case. This is to ensure code quality, but also helps others keep track of all the code that gets added to the code base. During a code review, be critical and feel free to ask for explanations if you do not understand a part of the code. In the future you may have to work on a feature that builds on top of the code you are reviewing so it is a good idea to know how it works!
- You are also responsible for informing QA and fixing any bugs that they find

Remember to have small and easy to review PRs, as mentioned in the [tips](../TIPS.md)

If you are unsure of what to do or want to confirm you are doing the right thing, then contact your tech lead!

## 3. (QA) QA Engineer tasks

If you are a QA Engineer, you will have the following responsibilities every week as a team:

- look at all of the features being built and write up test scenarios for each of them in the ticket itself. This will help ensure that the devs and yourself are clear on what the feature needs to do. You will also want to think of the test scenarios that you can automate and create an issue per scenario to automate it and add it to the backlog
- if a dev feature is ready then it is up to you to ensure that all of the test scenarios are covered by manualy testing the deployed version. If there are problems, then report the issues to the developers in the PR. Some issues may be minor and can be fixed in a later sprint, if that is the case, then make a new issue and add it to the backlog. _We leave the decision up to the team during the project, usually this would be decided with the Product Owner there._
- go through the QA Theory of the week
- at the start of the sprint the team will decide to add a couple of automation issues to the sprint to be completed. If no feature needs testing, then this is what to work on.

## 4. Getting settled in

This will be your first week of working in an Agile team so a lot will feel unfamiliar. To help you out, keep the following things in mind:

### 4.1 Daily standups

Remember that during the first week of daily standups the Education Director will be there to make sure that those are going according to plan. After the standup is done, feel free to ask any questions about the way of working to get it cleared up as soon as possible.

### 4.2 Preparing for the retrospective

Keep in mind that at the end of the week you will have a retrospective as that is a part of every agile team. The goal of the retrospective is to look at the way the team is working and identify the positive and negative parts of it. Then, as a team, adjustments to the way of working can be made to make everyone

If during the week you encounter something that really helped you, or hindered you, then write it down somewhere. In the retrospective you will be asked the following questions:

- What went well?
- What can we improve?

This can be in relation to the team, the way of working, the technologies used, etc. Anything that needs to be highlighted! It will be harder to come up with these on the spot, keep a list for yourself.

### 4.3 You are a team!

Although we do split you off into pairs and assign a ticket this is merely to indicate how to start the week. During the week you will run into complications that others may have run into before. Sometimes just having 10 minutes of help from someone else will allow you to get unstuck and move faster as a team. Once you are done with your ticket, check with the rest to see where you can help out. Either the team finishes everything or the team failed.

### 4.4 Developers & QA roles do NOT have a wall between them

You may sometimes feel that something is not part of your role, but that is an old way of thinking. You may not be as experienced a developer as a QA or you may not be that good of a tester as a developer but that should not stop you from helping out if the team notices a bottle neck. If there are a lot of tickets waiting for testing, then as a developer you can jump in and run through the test scenarios to help get those tickets through! Our QAs have quite some developer experience already, so if you see that not enough tickets are reaching the testing stage, start programming!

The great thing about Agile teams is that the goal is clear and although everyone has their specialties these are not defining. The team either succeeds or fails together!

### 4.5 Testing is not just on the QA role

Sometimes we here people in the developer role say: 'why should I test, the QA is here right?'. Although we love your faith in the QA, testing is a shared responsibility. Generally, unit testing and component testing is not the QA's responsibility, they are there for you as a developer and are therefore the developer's responsibility. This is why these types of testing were part of the main curriculum and why end to end testing was not.

# Week 6 tasks

This week is a little different. You've now experienced how it is to work in a development team and it is time to refocus on getting that job. That means that this week is focused on making the project something that is CV worthy.

# Week tasks:

This week's tasks in a row:

1. Clean up!
2. Final presentation
3. General Assessment
4. (QA) Theory
   - SSDLC
   - SQL/JS injection

## 1. Clean up!

Working as a group under pressure will always create some things that are not optimal. In the business we call that `technical debt` and it is time to clean some of that up. In the meeting on Sunday you have created a list of things to work on! As there is nothing assigned, it is important to communicate with each other what you are working on so that work is only done once.

During clean up you will probably also encounter some more problems in the code/app as you now take a closer look. Remember the tip to keep your PRs small and focused so if you encounter something, try not to fix it in the same PR but add it to the list to fix later. That way every PR has one focus and is easy to review.

## 2. Final presentation

Everyone who has helped you on the project would love to see what it has become in the end, so on the last Sunday you will hold a presentation to show it off. The guidelines for the presentation are:

- The presentation should be 15 - 20 mins long. Quality over quantity!
- In addition to being informational, make it fun!
- It’s up to you to choose who will be featured in the presentation. But make sure 3 people get to speak.
- Use slides to support your presentation. Make sure the order is logical and the buildup makes sense for outsiders. The slides should contain only a few keywords and images are highly appreciated.

The structure of the presentation needs to be as follows:

- Introduction: Introduce the team, technologies used, showing the UX of the frontend
- Technical accomplishments: Technologies used, what were some of the technological challenges and how did you solve them. The challenge here is to make it as specific as possible. Choose 1 or 2 examples in the application. Ask your mentor for help if needed.
- Social accomplishments: how did you work in groups, what worked well and what didn’t, what were some of the challenges in the project? Again, please be as specific as possible!

After the presentation, you will probably get some questions about how it went, what worked and what did not, etc. Anyone in the class can answer these questions, not just the people doing the presentation!

## 3. General assessment

This week you will also get a post in the class channel to schedule a time for your general assessment. Read more about it in the [week7 tasks](../week7/MAKEME.md). If no post is up, then poke the Education Director!

## 4. (QA) Theory

This week we will discuss some concepts that we have deemed out of scope for this project all around security testing. An actually deployed application with user data may always be subject to attacks by hackers. As a QA engineer you are also responsible for trying to find these vulnerabilities.

### 4.1 SSDLC

As you know by now, a software development life cycle (SDLC) is a framework that defines the process used by organizations to build an application from its inception to its decommission. Over the years, multiple standard SDLC models have been proposed (waterfall, iterative, agile, etc.) and used in various ways to fit individual circumstances. It is, however, safe to say that in general, SDLCs include the following phases:

- Planning and requirements
- Architecture and design
- Test planning
- Coding
- Testing and results
- Release and maintenance

In the past, it was common practice to perform security-related activities at the end of the process and before releasing. This after-the-fact technique usually resulted in a high number of issues discovered too late . It is a far better practice to integrate activities across the SDLC to help discover and reduce vulnerabilities early.

It is in this spirit that the concept of the secure SDLC (SSDLC) arises. A secure SDLC process ensures that security activities such as penetration testing, code review, and architecture analysis are integrated in the development effort. The primary advantages of adopting a secure SDLC approach are:

- More secure software
- Early detection of flaws in the system
- Cost reduction as a result of early detection and resolution of issues
- Overall reduction of intrinsic business risks for the organization

Considering the advantages of SSDLC, promoting this approach is part of your job as QA engineer.

The following course explains the foundation of secure coding, which will help you understand how can security can be integrated in SDLC:

- [Programming Foundations: Secure Coding](https://www.linkedin.com/learning/programming-foundations-secure-coding/)

### 4.2 SQL/JS Injection

QA engineers wear many hats, mostly they wear the users' hats to validate how users will interact with an application ... but they can also wear the _hacker_ hat!

Ethical hacking is aimed to identify vulnerabilities and fix them before the hackers exploit them to execute an attack.

One of the most common attacks is SQL Injection. Learn how to use SQL injection to expose data and wear your _hacker_ 🎩:

- [SQL Injection](https://www.youtube.com/watch?v=G6t1HxgTyfg)
- [Practicing with SQL injection](https://www.hacksplaining.com/exercises/sql-injection)

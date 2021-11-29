# Week 2 tasks

This week we start development! Have a look at the role(s) you are fulfilling on what your tasks are.

> This week, the mentors will be a little more available than normal to help get a good start. The education director will also be at the meetings to make sure that everything is going well and/or answer any questions about what to do in certain situations. This is only for this week, during the next week(s) the amount of support will get lowered until you can do it all yourselves.

Have a look at the [tips](../TIPS.md) for a successful project.

# Week tasks:

1. Daily meeting organiser specifics
2. (Dev) Developer tasks
3. (QA) QA Engineer tasks
4. (QA) Theory
    - Test plans/scenarios/cases
    - Gherkin
    - Creating (Bug) issues

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

## 4. (QA) Theory

This week the work starts and for the theory we will focus on knowledge that will help you communicate with the developors. We'll start with discussing the terms `Test plan`, `Test scenario` and `Test cases`. Next we will discuss the language `Gherkin` which provides a simple and concise way to describe what is expected from a feature. Lastly, we will go over how to create issues for bugs that you may find.

### 4.1 Test plans/scenarios/cases

We need to consolidate our testing ideas for specific features and be able to communicate them through a test plan so that everyone knows what the feature is required to do.

Learn how you can do that by reading the following resources:

- [What is Test Scenario? Template with Examples](https://www.guru99.com/test-scenario.html)
- [How to Write Test Cases: Sample Template with Examples](https://www.guru99.com/test-case.html)
- [The One Page Test Plan](https://www.ministryoftesting.com/dojo/series/the-testing-planet-2016/lessons/the-one-page-test-plan)

Examples :

- [Web Application Testing Checklist](https://www.guru99.com/complete-web-application-testing-checklist.html)
- [The Software Testing Planning Checklist](https://www.ministryoftesting.com/dojo/series/the-testing-planet-2019/lessons/the-software-testing-planning-checklist)

### 4.2 Gherkin

Not everyone can speakc JavaScript but almost everyone can speak [Gherkin](https://cucumber.io/docs/gherkin/reference/)!

Gherkin is a domain specific language created especially for business behavior descriptions without the need to go into detail of implementation. Since it's tied to the behavior, it's strongly conncted with Behavior-Driven Development (BDD).

Example:

```
Given I visit "/login"
  When I enter "Bob" in the "user name" field
    And I enter "tester" in the "password" field
    And I press the "login" button
  Then I should see the "welcome" page
```

Did you understand the desired behavior? Then you speak Gherkin too ;)

Master the Gherkin language by getting to know the syntax here:

- [What is Gherkin?](https://www.guru99.com/gherkin-test-cucumber.html)

Extra resource: [Gherkin Reference](https://cucumber.io/docs/gherkin/reference/)

### 4.3 Creating (Bug) issues

Imagine you have your test scenarios (translated into Gherkin or not), and while executing them something went wrong ... you're not seeing what you're supposed to see, the actual behaviour is not as the expected behaviour!

Then you might have caught a bug 🐞! To know what is a bug and what are the kinds of bugs .. watch this:

- [Testing Essentials - What is a bug?](https://www.youtube.com/watch?v=jvBoKXDCvLE)

To communicate a bug to the developers we want to discuss the art of 🐞storytelling.

> Testers are storytellers. Coming from a communications background, one of the striking parallels I have made since working in quality assurance and software testing is that an important part of their role is to tell short stories through immediate product feedback. One powerful storytelling device they use to achieve this is: the bug report. (By Anneliese Herbosa)

- [The Art Of The Bug Report](https://www.ministryoftesting.com/dojo/series/the-testing-planet-2019/lessons/the-art-of-the-bug-report)

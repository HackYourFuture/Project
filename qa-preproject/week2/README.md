# Reading Material QA PreProject Week 2

## Agenda

These are the topics for week 2:

- Test plans/scenarios/cases
- Gherkin
- Creating Issues
- Agile Testing
- (Optional) ISTBQ

### Test plans/scenarios/cases

We need to consolidate our testing ideas for specific features and be able to communicate them through a test plan so that everyone knows what the feature is required to do.

Learn how you can do that by reading the following resources:

- [What is Test Scenario? Template with Examples](https://www.guru99.com/test-scenario.html)
- [How to Write Test Cases: Sample Template with Examples](https://www.guru99.com/test-case.html)
- [The One Page Test Plan](https://www.ministryoftesting.com/dojo/series/the-testing-planet-2016/lessons/the-one-page-test-plan)

Examples :

- [Web Application Testing Checklist](https://www.guru99.com/complete-web-application-testing-checklist.html)
- [The Software Testing Planning Checklist](https://www.ministryoftesting.com/dojo/series/the-testing-planet-2019/lessons/the-software-testing-planning-checklist)

### Gherkin

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

### Creating (Bug) issues

Imagine you have your test scenarios (translated into Gherkin or not), and while executing them something went wrong ... you're not seeing what you're supposed to see, the actual behaviour is not as the expected behaviour!

Then you might have caught a bug 🐞! To know what is a bug and what are the kinds of bugs .. watch this:

- [Testing Essentials - What is a bug?](https://www.youtube.com/watch?v=jvBoKXDCvLE)

To communicate a bug to the developers we want to discuss the art of 🐞storytelling.

> Testers are storytellers. Coming from a communications background, one of the striking parallels I have made since working in quality assurance and software testing is that an important part of their role is to tell short stories through immediate product feedback. One powerful storytelling device they use to achieve this is: the bug report. (By Anneliese Herbosa)

- [The Art Of The Bug Report](https://www.ministryoftesting.com/dojo/series/the-testing-planet-2019/lessons/the-art-of-the-bug-report)

### Agile Testing

As part of the team, QA engineers have an important role throughout the whole process of development. Agile Testing is not sequential (in the sense it's executed only after coding phase) but continuous.

Learn more by going through the following course:

- [Agile Testing](https://www.linkedin.com/learning/agile-testing-2/uplevel-with-agile-testing)

### (Optional) ISTQB

From _Wikipedia_

> The International Software Testing Qualifications Board (ISTQB) is a software testing certification board that operates internationally. ISTQB Certified Tester is a standardized qualification for software testers and the certification is offered by the ISTQB.

> ISTQB streams focus on:
>
> - Core – these modules correspond to the “historical” ISTQB certifications
> - Agile – these modules address testing practices specifically for the Agile SDLC
> - Specialist – these modules are new in the ISTQB product portfolio and address specific

ISTQB Foundation Level syllabus stated the principles of software testing, read about them here :

- [7 Principles of Software Testing](https://www.toolsqa.com/software-testing/principles-of-software-testing/)

This site also offers a lot of other information about testing from the standard! So in the next few weeks/months, make sure to keep going back to see what else is out there that is out of scope for our curriculum.

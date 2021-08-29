# Week 1 tasks
You are either in the 'backend' or the 'frontend' team. Although you are only responsible for the deliverables in your team, you will need to communicate between each other. The 'frontend' team may decide on some features that require changes in the schema for example.

We strongly suggest planning daily collaboration meetings, not only within the teams, but also between both teams.

## 'Backend' team
The 'backend' team will be responsible for the following deliverables at the end of the week:
- An Entity Relationship Diagram
- A skeleton code base with the folder structure set up
- Code style/linting rules set up

On Sunday you will be asked to present the diagram and the code base/rules to the whole group, but it is usually better to already share the information before the meeting so others have a chance to look at it beforehand.

### Entity Relationship Diagram
An Entity Relationship Diagram is a visual representation of how the database will be set up and you've learned about them in the database module. By thinking out the database structure and having a diagram that everyone can refer to it will be much easier to communicate with each other. In the project you will be using [mongoose](https://mongoosejs.com/) which will bridge the gap between relational and document-based databases by providing schema's that the documents have to adhere too. By having the diagram, implementing these schema's will also become a lot easier.

### Skeleton code base
When working on the same project with a lot of different people it becomes vital to have a set of rules of how the code is built. If everyone uses their own way of working the code base will become a huge mess which in time will lead to an unmanageable application. Have a discussion with your team about the following questions:

- What CSS solution will you use? (styled-components? react-bootstrap? material ui?)
- What is the frontend folder structure? (Is there a separate folder for the pages / components?)
- What frontend routing solution do you use? (react-router? something else?)
- What is the backend folder structure? Where are the controllers? Where are the models? Where are the routes?
- What type of backend API will you build? (REST? Express? GraphQL? Apollo?)
- Do you want to set up a design system? (Storybook? React-styleguidist?)

To make it easy for the team to stay on the same page concerning these decisions it is generally best to already build a full roundtrip that uses all the things. By doing this, when other team members look at the code base for their first issue next week, it is already clear how the code is structured. As pretty much all applications have users, it is quite safe to already make something that lists users. Create the following:

Backend
- A basic User schema (just id, e-mail and name should be enough)
- A route to get all users. Only return the user's name and id, not the e-mail.
- A route to get the details of a user. This time return everything.

Frontend
- A page that takes the id of the user from the URL and shows the details of that user (name and e-mail)
- A page that gets all the users and lists them on the page with their name. When clicking on a user it goes to the detail page

The goal is to implement the structure, not something that actually will be deployed. This means you should keep it as simple as possible while making sure that all of the decisions made are implemented in some way.

### Code style
The big decisions made to make the skeleton code base will create a general way of working, but code has so many options that all development teams also have a defined code style. These are things like:

- Do we always use arrow functions?
- Do we use `--` to subtract one from a variable or always hard assign?
- Do we use shortcuts for booleans?

This can get very strict, see for example the airbnb rules here: https://github.com/airbnb/javascript. Some rules are there to avoid bugs, some are for readability and others are for consistency. We do not expect a document like this, but do expect the team to set up eslint (https://eslint.org/) in the project and make it run a check on committing so that all code that gets pushed to github adheres to any rules you set up. This will keep the code looking professional by adhering to a shared style.

## 'Frontend' team
The 'frontend' team will be responsible for the following deliverables at the end of the week:
- Wireframes for the full app
- Product board filled with user stories for the [Minimal Viable Product](https://en.wikipedia.org/wiki/Minimum_viable_product)

On Sunday you will be asked to present the wireframes and the user stories to the whole group, but it is usually better to already share the information before the meeting so others have a chance to look at it beforehand.

### Wireframes
All applications start with an idea, but an idea does not get you very far. To work out application ideas we generally start with wireframes. These are a representation of all the pages the application will have without adding any design layers yet. This allows everyone to talk through the application and already figure out the user experience without having to code anything.

To create wireframes we suggest using [figma](https://www.figma.com) as it allows you to easily build and share the wireframes as well as collaborate on them in real time.

The wireframes you make will become the basis for building features in the next 6 weeks, so make sure that they are clear and self explanatory to anyone looking at them for the first time.

### Product board
In github you will find a `Projects` tab that will contain a project board that will be used throughout the upcoming 7 weeks. How the board works will be explained in our first meeting.

After having wireframes set up it is time to decide what features will be part of the MVP (`must-have`) and what can be left out until later (`nice-to-have`). This sounds easier than it actually is. A good way to go about this is write down all the features into [user stories](https://www.mountaingoatsoftware.com/agile/user-stories). Different teams use different templates, the project board will already have an example there for you to help you along. In our project we want every user story to contain:

- A title (`As a user, I want to ..., so that I can ...`) that describes the goal of the feature
- The acceptance criteria (also called `definition of done`) that describes what needs to be implemented for the user story to have been solved

Once you have split up the project into user stories it will be easier to decide on what is absolutely needed and what is not. Giving us a small list of features that the class can build in two weeks.
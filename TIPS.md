# Development team tips
Working on a project with multiple people has a lot of benefits, but it also brings about some challenges. We want to give you some tips of how to transition into the project where you are not studying/learning individually anymore.

Good luck in the project! Make it awesome and your CV will be very happy.

## Keep PRs small and focused!
At the start of the week, make sure you think about the `steps to complete` the feature. You should *not* be doing everything at once, but do everything in small steps. Make it small steps that are functionality on their own so that whenever you finish a step you can already create a PR and have someone review it. The key to keeping a code base clean is to keep the PR's manageable. 

A huge PR is very hard to review and will make it a lot easier for bugs to get through into the production environment, which is about the worst thing that can happen. So keep the steps small and make it easier on everyone!

For example, if you are building a user list that requires the names and avatars of the user to be displayed on the screen you could split this into 4 different steps:
- Create a user model
- Create an endpoint for all users with routers and controllers
- Create a visual component that shows the name and avatar of a single user
- Create a page that grabs the list from the endpoint and shows our component in step 3 for all of the users

Each of these PRs are manageable and reviewable in a short time which make it much easier for your classmates to review. The first 3 do not change the UI/UX in any way so are safe to push to the code base without having the rest implemented yet.

## Do not forget about UX!
We do not have a designer in the team, which means you are responsible for the design of the application. Remember that the [design guidelines repo](https://github.com/HackYourFuture/design_guidelines) gives you loads of tips on how to make an application look good!

## Work as a team
If you are struggling with a bug or are unsure of how to implement something, post it in the class channel! You now have a development team to support you. Sometimes all you need is someone to explain your problem to to get to a solution. This happens all the time in a work environment.

## What to do once finished?
Some features will be done earlier than others, but the sprint is only done when everything is done! So once you are finished, see what other team may need some help! Only if noone else needs help is it fine to pick up a new issue, or possibly use the time to refactor some code! As one of our mentors always said: 'code is never done!'.

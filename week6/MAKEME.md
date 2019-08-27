## Project Week 6 Homework

**Note: This homework assumes you've already done the homework for week 5. If you haven't, please go [here](week5.md) to finish that first.**

## Learning goals

By doing this week's homework you'll learn how to:

- Merge branches
- Resolve merge conflicts
- Make your application production-ready
- Deploy via the Heroku CLI

## Merging branches

So far the every group has worked on different branches. This week you'll merge branches into the `development` branch. When that has happened succesfully, the `development` branch will be merged into `master`.

This doesn't always happen smoothly: **merge conflicts** will arise. What is this? Merge conflicts happen when you merge branches that have competing commits, and GIT needs your help to decide which changes to incorporate in the final merge.

These will always vary. Here are general tips to keep in mind when merging:

- **Keep calm!** Git always allows you to go back to the state before the conflict occurred. With a simple `git merge --abort`, you can always undo the merge and start over again.
- In case you've made a mistake while resolving a conflict and realize this only after completing the merge, you can still easily undo it: just roll back to the commit before the merge happened with `git reset --hard <commit-hash>` and start over again. You can get the commit-hash with `git log --oneline`

## Make the app production-ready

To make the application production-ready requires 2 different changes:

- Rewriting the server to make use of `environmental variables` in production.
-

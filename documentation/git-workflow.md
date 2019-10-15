# Git Project Workflow Guide

There will be 1 remote repository that everyone will work with. Everyone will git clone the repository and make sure to have fetched the most recent commit

### REMOTE

- The remote repository will have a master branch, and a development branch (branched off from master)
- The development branch will contain all the merged feature code
- Each team will create a branch for each feature (so there will be _6_ feature branches in total)
- Each member of the team will use this feature branch to work from

### LOCAL

- The local repository will also have a master and development branch. You will fetch and push code to their respective remote branches
- Each team member will also have a branch for each branch they are working on (so there will be _2_ feature branches for each team member in total)
- Each team member will work on their part of the feature locally, and when they have committed it locally send it to remote (GitHub) for the others to pull it from

## COMMUNICATION GUIDELINES

Communicate as often as possible. At the beginning of each day have a meeting about who’s going to do what for that day. This is the `daily standup`.

Afterwards you can take some time to discuss how to approach each task.

Tips to communicate:

- Write down your tasks using checklists. This creates clarity and provides an overview for you and your teammembers
- Make use of video chat when needed. The “Share screen” option on Slack is useful to help each other to debug code

## GIT WORKFLOW

### Daily workflow:

1. Write some code on local branch [FEATURE_NAME], for example “social-media-login”
2. Add and commit this code locally
3. Push the code to the remote branch with the same name, “social-media-login”
4. Your team member pulls the code from remote branch “social-media-login” to their local branch “social-media-login”
5. Repeat step 1 to 4

### When feature is finished:

1. Make sure every team member has merged their code with the remote branch “social-media-login”
2. Make sure every team member can functionally use the feature in 3. their local project
3. One team member makes a pull request to remote branch development, but doesn’t merge it!

## IMPORTANT!

1. Merging code with development and master will only be done on **remote** (GitHub), through pull requests
2. Each team member will work on a feature while in the branch of that feature. Once you are done for the day, `git push origin [BRANCH_NAME]` the code to the remote branch. At the start of a new day, `git pull origin [BRANCH_NAME]` to get the latest version of the code base
3. Each week you are expected to implement one feature, which you will present to the rest of the class that Sunday
4. We will merge the features into development on the Sunday
5. When in need of help: contact the teachers and assistants who are part of the module

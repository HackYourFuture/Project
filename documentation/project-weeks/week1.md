## Project Week 1 Homework

**Note: This homework assumes you've already setup your basic project folder. If you haven't, please go [here](../guide-newproject.md) to set that up first.**

## Learning goals

By doing this week's homework you'll learn how to:

- Set up [endpoints and routes](https://www.lynda.com/WordPress-tutorials/Understanding-routes-endpoints/572168/596805-4.html) on the backend
- Create, read, update and delete data in the backend
- How to use `React-Router` in the frontend
- Connect a React frontend with a Node backend

### 1. Server-side

1. Create an Express HTTP server which includes the following routes:

- `GET /api/houses`. This route responds with a list of houses. For the moment you can use a JSON array as
- `POST /api/addhouse`. This route creates a new house object with data provided from the client. After, it responds to the client with the freshly created object.
- `GET /api/houses/:id`. This route responds with data from a house with an id specified in the URL.
- `DELETE /api/houses/:id`. This route removes a house object with the id specified in the URL.

Any other request that starts with `/api`, like `/api/jkasdkjas` should result in a `404`.

2. Serve static files.

Write code that will allow your Express server to serve requested static assets from the `/client/build` folder

Any other `GET` request should respond with content of the `/client/build/index.html` file.

### 2. Client-side

1.  The React frontend (client) will communicate to the server via the `/api/` root endpoint. On the client-side, include the following routes using React-Router:

- `/`. This should take the user to the home/index page
- `/houses` should show the user a list of houses
- `/houses/:id` should show the user a single house (with the id provided in url)
- `404` should be shown to the user whenever an unknown route is entered

2.  Whenever you create a parent component, make sure it handles the following states:

- `LOADING`: when the component is still fetching data make sure to show the user feedback. Usually, this would be an animation. For now, just show the message 'Loading...'
- `ERROR`: when the component fails to load data the server responds with an error. Translate this message into a user-friendly feedback
- `EMPTY`: when there is no data to show, for example if there are no houses in the list, give the user feedback. This can be a simple message, like 'Nothing to show yet!'

Note: make sure to put all of the user feedbacks into state and then pass it down to the JSX.

### Stuck?

Watch the following video to get a better sense of what to do:

[Part 1](https://www.youtube.com/watch?v=PH87EnV6CKI)
[Part 2](https://www.youtube.com/watch?v=3fhtOWC-uIY)

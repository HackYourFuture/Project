## Project Week 1 Homework

**Note: This homework assumes you've already setup your basic project folder. If you haven't, please go [here](../guide-newproject.md) to set that up first.**

## Learning goals

By doing this week's homework you'll be learn how to:

- Set up [endpoints and routes](https://www.lynda.com/WordPress-tutorials/Understanding-routes-endpoints/572168/596805-4.html)
- Add, read and delete new data in the backend
- How to use React-Router
- Connect a React frontend with a Node backend

### Server-side

1. Create an Express HTTP server which includes the following routes:

- `GET /api/houses`. This route responds with a list of houses.
- `POST /api/houses`. This route creates a new house object with data provided from the client. After, it responds to the client with the freshly created object.
- `GET /api/houses/1`. This route responds with data from a house with an id specified in the URL.
- `DELETE /api/houses/1`. This route removes a house object with the id specified in the URL.

Any other request that starts with `/api`, like `/api/jkasdkjas` should result in a `404`.

2. Serve static files.

Write code that will allow your Express server to serve requested static assets from the `/client/build` folder

Any other `GET` request should respond with content of the `/client/build/index.html` file.

Any other request should result in `404`.

### Client-side

1.  The React frontend (client) will communicate to the server via the `/api/` root endpoint. On the client-side, include the following routes using React-Router:

- `/api/`. This should take the user to the home/index page
- `/api/houses` should show the user a list of houses
- `/api/houses/:id` should show the user a single house (with the id provided in url)
- `404` should be shown to the user whenever an unknown route is entered

2.  Implement a way to handle the `LOADING`, `ERROR` and `EMPTY` states of the frontend part of the application.

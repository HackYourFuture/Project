## Project Week 1 Homework

**Note: This homework assumes you've already setup your basic project folder. If you haven't, please go [here](../guide-newproject.md) to set that up first.**

## Learning goals

By doing this week's homework you'll be learn how to:

- Set up [endpoints and routes](https://www.lynda.com/WordPress-tutorials/Understanding-routes-endpoints/572168/596805-4.html)
- Add, read and delete new data in the backend
-

### Server-side

1. Create an Express HTTP server which includes the following routes:

- `GET /api/houses`. This route responds with a list of houses.
- `POST /api/houses`. This route creates a new house object with data provided from the client. After, it responds to the client with the freshly created object.
- `GET /api/houses/1`. This route responds with data from a house with an id specified in the URL.
- `DELETE /api/houses/1`. This route removes a house object with the id specified in the URL.

Any other request that starts with `/api`, like `/api/jkasdkjas` should result in a `404`.

2. Serve static files.

Write code that will allow your Express server to serve requested static assets from the `/client/build` folder

Any other `GET` request should respond with content of the `/client/build/index.html` file

Any other request should result in `404`.

### Client-side

client:
base create-react-app with react-router

    client should talk to server via api (don't forget we run backend app on different port)

    supported urls(pages):

        HOME

        LIST of houses - should load and render list of houses using api GET /api/houses

        ONE house by id - should load and renderhouse data with id provided in url

        404

    try to implement LOADING, ERROR and EMPTY states when work with data fetching

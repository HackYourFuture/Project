## Project Week 3 Homework

**Note: This homework assumes you've already done the homework for week 2. If you haven't, please go [here](week2.md) to finish that first.**

## Learning goals

By doing this week's homework you'll be learn how to:

- How to build a `full-stack feature`: a search and filter functionality

## Frontend: filter, order and pagination

Modify the form to have filters (filter by `price`, `location` and `amount of rooms`), order, pagination on frontend

- preserve filter state in url
- read from url on page load and put data in state
- we can do actual filtering on ‘submit’ not on input change as i did
- filtering means you send your search form state to server and wait for new results from it

## Backend:

- change `GET /api/houses` endpoint on backend, it must validate the query params provided by the client. Compose a query that will retrieve only data eligible for search criteria

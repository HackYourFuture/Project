## Project Week 3 Homework

**Note: This homework assumes you've already done the homework for week 2. If you haven't, please go [here](week2.md) to finish that first.**

## Learning goals

By doing this week's homework you'll learn how to:

- Build a `full-stack feature`: a search and filter functionality

## Frontend: filter, order and pagination

1. Modify the form to include extra input fields; these will be filters by which we selectively request data from the database. Make a field for `price`, `location` and `amount of rooms`. Put the input values in state.

2. Add another filter: `order` by price and location. Put the input value in state.

3. Add another filter: `pagination`. Show 5 items on every page. If there are more than 5 houses in the database, split it into a different page. Show a page number at the bottom of the screen. Put the input value in state.

Important to note:

- Put the search criteria in the URL as parameters, like `?price_min=50000&price_max=100000`.
- Make sure to load in items with default search criteria, on page load and when any of the criteria is changed

## Backend:

Inside the route `GET /api/houses`, validate the query parameters provided by the client; make sure the server gets what it expects.

Compose a MySQL query using the query params.

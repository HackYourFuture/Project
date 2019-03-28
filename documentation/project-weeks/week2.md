## Project Week 2 Homework

**Note: This homework assumes you've already done the homework for week 1. If you haven't, please go [here](week1.md) to finish that first.**

## Learning goals

By doing this week's homework you'll be learn how to:

- Setup and `link a MySQL database to your Node.js server`
- How to `validate data` from a database
- `Create a full-stack feature` that allows users to upload data

## Connect a Database to your application

We'll be using an instance of MySQL.

1. Using the CLI or GUI, create a new database called `housesDatabase`
2. Inside the database, create a new table with the following structure:

`id`
primary key
`link`
string
url to original offer
unique key
`market_date`
date
date when offer was added to website or data of adding it to database
required
`location_country`
string
country name
required
`location_city`
string
city name
required
`location_address`
string
house address
`location_coordinates_lat`
float
latitude
`location_coordinates_lng`
float
longitude

- - either address or lat+lng is required
    `size_living_area`
    int
    living area in square meters
    required
    `size_rooms`
    int
    total number of rooms
    required
    `price_value`
    float
    price of property
    float number
    required
    `price_currency`
    string
    currenct code, 3 characters
    required
    `description`
    string
    free text
    `title`
    string
    free text
    `images`
    string
    list of urls to images, separated with comma
    <url1>,<url2>,<url3>
    `sold`
    int
    1/0

## Making a change on the server

1. Change the logic of the POST /api/houses endpoint

- Instead of the `fakeDB` array it should expect a JSON string as input data.
- The data type of this data should be `array`.
- In the response to the client it should generate a small report:
  - valid: N
  - invalid: array
    - errors
    - raw
- All valid data should be inserted into `housesDatabase`, the invalid data can be ignored

2. Validate the data on the server

- Every element in the array should be validated
- All required fields should be included
- Every field in the object should be validated according to its purpose

## Making a change in the client

On the frontend we'll be creating a new feature, that allows a user to **contribute** housing data.

1. Create a frontend route that goes to `/contribute`

2. Create a form that is linked to a `/contribute` endpoint in the backend.

- The form should contain a `textarea` and a `submit button`
- On submit, the backend will send a report as a response
- Take care of error handling

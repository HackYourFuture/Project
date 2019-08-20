## Project Week 2 Homework

**Note: This homework assumes you've already done the homework for week 1. If you haven't, please go [here](week1.md) to finish that first.**

## Learning goals

By doing this week's homework you'll learn how to:

- Setup and link `a MySQL database` to your `Node.js server`
- How to `validate data` from a database
- Creating a feature: user feedback on data upload
- Creating a feature:

### 1. Creating a database

This week we'll be creating a new database, connecting it to the server and making it possible for a user to upload data in the client.

1. Using the command line or GUI ([MySQLWorkbench](https://dev.mysql.com/downloads/workbench/)), create a new database called `housesDatabase`.
2. Inside the database, create a new table called `houses`. Give it the following structure:

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
either address or lat+lng is required

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
`<url1>,<url2>,<url3>`

`sold`

int  
1/0

### 2. Making a change on the server

1. Change the logic of the `POST /api/houses` endpoint

- Instead of the `fakeDB` array it should expect a JSON string as input data.
- The data type of this data should be `array`.
- In the response to the client it should generate a small report:
  - valid: N
  - invalid: `array`
    - errors
    - raw
- All valid data should be inserted into `housesDatabase`, the invalid data can be ignored

2. Validate the data on the server

- Every element in the array should be validated; is the data of the expected type?
- All required fields should be included
- Add error handling: create an error message for each invalid element

3. Send the error report to the client

- Make sure it's an array

### 3. Making a change in the client

On the frontend we'll be creating a new feature, that allows a user to **contribute** data.

1. Create a frontend route that goes to `/contribute`

2. Create a form that is linked to a `/contribute` endpoint in the backend.

- The form should contain a `textarea` and a `submit button`
- On submit, the backend will send a report as a response

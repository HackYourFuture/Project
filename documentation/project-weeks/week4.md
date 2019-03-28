## Project Week 4 Homework

**Note: This homework assumes you've already done the homework for week 3. If you haven't, please go [here](week3.md) to finish that first.**

## Learning goals

By doing this week's homework you'll be learn how to:

- Create your own `scraping` script
- Extract data from any website
- Put the extracted data in your MySQL database

## Web Scraping

The main task is to create a scraper app (separate Node.js script).

It will extract data from other web applications (websites), so that we can use it in our own application (it will be part of the `/contribute` feature).

The result of our scraper should be **housing data** in a specified format: a JSON array of houses. Each key in a house object should align with the data model we have defined: required fields, data types and values.

Ideally, results should be hosted and accessible through a URL.

To build a scraper you can use one of 3 options:

1. [Cheerio](https://cheerio.js.org/)

Cheerio is a Node.js library which will help you to parse html text into a JavaScript structure that is searchable and has handy methods to extract data you need.

Cheerio only works with text (html) that we retrieved by making a request to a corresponding url, which means if data is not in html (initial response, js was not loaded yet, some parts were not rendered) you can not perform search in it.

We still need to put results of scraper in file/url to be able to upload it to our main application.

2. [Puppeteer](https://pptr.dev/)

Puppeteer is a Node.js API for a headless (without a graphical display) Google Chrome browser.

Since it runs an actual browser, you can load your URL in it and have access to the generated DOM, which also means all the searching possibilities you can perform in regular browser console.

The huge advantage of Puppeteer is that it can wait for your page to load and execute JavaScript, which makes dynamically rendered content searchable.

We still need to put results of scraper in file/url to be able to upload it to our main application.

3. [Apify](https://www.apify.com)

Apify is a platform for creating and executing your scrapers.
They have their own way of defining the crawler code, needs some time to understand it.

The huge advantage of Apify is that you can put your crawler on a schedule, and Apify will run it for you, save results and provide a permanent link to it which you can then directly upload to our main application.

> Keep in mind: Don't forget to save html content of requested pages when you are playing with it.

> Keep in mind: Don't send too many requests to any particular website or you will get blocked.

To get you started here are some pointers. The following is pseudocode for your scraper (don't forget, most of it is asynchronous code):

```
var results = [];

generate list of search result pages

for every search result page
    request html content of the page

    extract list of houses urls

    for every house url
        request html content of the house page

        var houseData = {}

        // price looks like "$ 123,321.00"
        // we need to extract value and price according to our database format

        houseData.price_value = extractPriceValue(document.querySelector('.price').innerText);
        houseData.price_currency = extractCurrency(document.querySelector('.price').innerText);
        ...

        results.push(houseData);

write data to file in JSON format
```

# Resources Final Project Week 2

## Agenda

1. Fundamental Web Application concepts I
   - Form validation
   - Error handling
2. What is Agile?
   - Agile philosophy
   - Waterfall vs. Agile

## 1. Fundamental Web Application concepts I

When building web applications, invariably certain challenges come up. How do you make sure users use your application in the right way? And if they're doing it wrongly, how can we help them to do it better?

Some of these challenges have been addressed by developers, and this has led to certain standard practices we need to learn to incorporate in our applications.

### Form validation

Form validation refers to process of checking the `<input>` fields of a `<form>`, to make sure the user has inserted the correct type of information.

If a user fills in a phone number in an email address input field, we don't want our database to accept it. As you can imagine, this might lead to future trouble.

We can add validation rules to **both the backend and the frontend**. Of the two, the backend validation is most important. Why? Mainly because a hacker cannot access the backend of an application as easily as the frontend.

Learn more about form validation in the following resources:

- [Process and Validate User Submitted Data with Express and Node.js](https://www.youtube.com/watch?v=WFHzlExDwrY)
- [JavaScript Form Validation](https://www.youtube.com/watch?v=In0nB0ABaUk)

### Error handling

An `error`, also known as an `exception`, is a mistake that might happen during the execution of our code. Whenever an error happens, we want to be sure that we know about it. The mechanism by which we learn about the occurrence of an error is called `error handling`.

Imagine an application that had no error handling mechanism at all. How would you know where to look if an error did happen?

In order to know where errors happen we have to `throw` them in certain places of our application. This will help you identify where the error originated. Depending on where you insert it, your program will `catch` this error. This is where you can actually "handle" the error, for example by sending back a response to the client that includes an error message for the user.

Learn more about error handling in the following resources:

- [How to Handle Errors - Basics of Error Handling in JavaScript](https://www.youtube.com/watch?v=G8Jux_bsIXU)
- [try, catch, finally, throw - error handling in JavaScript](https://www.youtube.com/watch?v=cFTFtuEQ-10)

## 2. What is Agile?

In this module you'll learn all about Agile software development, because nowadays that's the standard way of working in modern tech companies. But what is it?

### Agile philosophy

The first thing to learn is that Agile is not a technology. In fact, it has little to do with actual progrmaming. 

- [Software Development Methodology: What is Agile?](https://www.youtube.com/watch?v=GzzkpAOxHXs)
- [Agile manifesto](https://www.youtube.com/watch?v=jSayJF0epJs)

### Waterfall vs. Agile

[Waterfall vs. Agile](https://www.youtube.com/watch?v=egF9-FejbsA)

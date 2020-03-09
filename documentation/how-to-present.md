## Individual Presentations

Giving presentations is an essential part of working in teams. But why is this the case? Most likely you've done them in school, and maybe even at some job. In the following we'll discuss several important reasons for **why** it's important to have good presentational skills.

1. Communicate ideas or results

The first reason directly links to the content of the presentation. You want to present ideas or the result of work to members of your team/company. Usually there is no place for discussion innovation, unless at a special meeting or presentation.

2. Show confidence

A business grows through a series of wise decisions. When you present your ideas with confidence, others will take them more seriously and thus think better of your abilities. This will help the business and you as well.

3. Gather feedback

This is important: sure, you're presenting your ideas. But you also want to throw them in the group to see how others look at them. Because maybe you're in some regards incorrect, or need a second opinion.

4. Answer questions

This will allow others to more fully grasp what your ideas are about.

### Presentation guidelines

Here are some guidelines to preparing a quality presentation:

1. Prepare slides (Keynote or Powerpoint)
   - Each slide should contain only a few keywords that help summarise your point
   - Provide code snippets
   - Slide style matters (choose soft colors and fonts)
2. Know the topic by heart. In case it’s helpful you may carry a short note with some keywords to keep your line of thought
3. Prepare at least 1 code snippet that illustrate the concept you’re talking about
4. Make enough contact with the audience: proper eye contact and creating interactivity will increase engagement for both the audience and yourself
5. You have to show your thinking when answering questions (be honest!)
6. You are not allowed to read from a paper or use Google during the presentation

### An Example

The following example has a basic structure:
1. A clear definition, IN YOUR OWN WORDS. Make it as simple as possible.
2. Show an example of the concept in code. Either self-created or found in a project.
3. Be ready for questions!

> Example Topic: “Functions”
>
> 1. A function is a reusable block of code designed to perform a certain task. For example, the task of the map() is to loop over an array to make it possible to modify every array element by calling another function on each item. Required to write a function are the “function” keyword and “return” statement.
> 2. In the following piece of code functions are used to perform the task of transforming the data inside an array from strings to numbers:

```js
const letters = [‘a’,’b’,’c’,’d’];
   function stringsToNumbers(arr) {
   const numbers = arr.map(letter => arr.indexOf(letter));
   return numbers;
   }
   stringsToNumbers(letters);
```

> In the code you can see the definition of the function and the call. This functions takes the “letters” variable, which stores an array of strings, and performs the map function over it to return the index numbers of each ‘letter’.
>
> 3.  Does anybody have any questions?

<!-- You've just finished your project: your own full-stack application! However, so far you've only kept it to yourself. Wouldn't it be more fun to share it with others? That's what this document is about: how to present your project.

You'll be presenting your project to the rest of the HackYourFuture community. These consist of people of different levels of understanding. Some will understand all the fancy technologies you've used, while others will only stare blankly at what you've just said. That's not helpful.

Instead, we'll be presenting things differently: **talk about your own experience**. Something we can all relate to is another person's experience. What have you learned about development, yourself and HackYourFuture, during these past 6 weeks?

Example: _During the process I have learned the value of working together. While it's not easy to communicate, I've found it helpful to ask my team members for help whenever I get stuck. That way I don't feel like I have to do all of this stuff myself._ -->

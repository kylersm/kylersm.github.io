---
layout: essay
type: essay
title: "TypeScript: Finally Introduced for my Class"
date: 2025-08-30
published: true
labels:
  - Course Pedagogy
  - TypeScript
---

At long last, one of my college classes has introduced the language I have used as a daily driver for a while now: TypeScript!

## Type(d)Script - What is it?

<img class="img-fluid float-start pe-4" width="250" src="../img/typescript.svg">

For those that don’t know, TypeScript is essentially JavaScript but less forgiving with what you can get away with writing and running. It’s the same syntax, just with additions for type safety. For example, you can’t reassign the type of a variable in TypeScript; but you can do this in JavaScript. You may think this sort of behavior is limiting at first, but ask yourself: “Why would you need to do that in the first place?”. After all, it makes the code harder to read. While other tools like ESLint can (and should also) be used to check your code for clarity, TypeScript enforces type safety. “Type safety” as in making sure you don’t access a property that may not exist on an object, or call a function with the wrong amount or wrong types of arguments. Think of JavaScript, but less with guesswork on what properties and types an unknown object might have.

In fact, all that happens to the TypeScript code is that it gets compiled to JavaScript for actually running. When it comes to which one I like better, I prefer JavaScript when it comes to testing quick snippets of code. I don’t need to mess around with compiling and I can write quick n' dirty code that doesn’t have to obey the rules of TypeScript. I use it for Tampermonkey scripts, inside the node.js terminal, and in DevTools’ console. If I’m writing something complex, say more than 20 lines of code, then I will switch to TypeScript to notify me of mistakes I might make. When compared to the other languages I know that are “strongly typed” (C, C++, Java), I consider TypeScript to be the easiest to use out of all of them.

## LearnedScript - ES6

Even though I consider TypeScript/JavaScript to be one of my main languages, the ES6 module on freeCodeCamp taught me something else I didn’t know I could do in JavaScript. 

In ES6, we can selectively pick out certain properties from an object using this syntax:

```js
const object = { a: 5, b: 6 };
const { a, b } = object;
```

I already knew this, but I didn’t know this can be applied for nested objects. However, I never really found a situation where I needed to do this:

```js
const people = { john: { hobby: "drawing" }, cris: { hobby: "soccer" } };
const { john: { hobby } } = people;
console.log(hobby); // “drawing”
```

If I hadn’t known this, I probably would have written it like this:

```js
const people = { john: { hobby: "drawing" }, cris: { hobby: "soccer" } };
const { hobby } = people.john;
console.log(hobby); // “drawing”
```

It’s not that different from the previous example, and actually shorter than it. Though, I can see it being useful if I wanted the hobby for `cris` in addition to `john`’s. 

## What are we doing with TypeScript?

For ICS 314, we have had two timed coding assignments called workouts of the day (WODs for short). For context, our course’s pedagogy is based on “[athletic software engineering](https://philipmjohnson.org/essays/ase-2017.html)”, where every week we are given a timed programming assignment to finish in class and receive a grade based on accuracy. You can think of it as a timed Leetcode question. So far, these two assignments were practices that could be done in the comfort of your own space with unlimited retries. 

*What do I think?*

I’m not sold. (yet)

The practice WODs we were given can be rewritten into the following prompts:
- Write a program in JavaScript that sums up all the numbers [1, 1000) that are multiples of 3 or 5.
- Write a function named `isUnique` in TypeScript that checks if every character in the string only appears once (that is, there are no duplicate characters).

### WOD Predictions

First, the difficulty of these assignments were very easy. My concern is that the real WODs won’t hold back on the difficulty at all. These WODs feel like they are for getting us used to the process of doing a WOD, not on what to expect in terms of difficulty. Although, the course assumes we have just learned JavaScript on freeCodeCamp and TypeScript on W3Schools, so there is a case where this level of difficulty is reasonable.

However, In order for me to be able to form a good opinion, I need to be in the classroom doing a “real” WOD. “Real” meaning the instructor might tell us it’s real, then come out at the end and say it won’t be graded to induce genuine anxiety; or, "real" as in it will actually be graded. Regardless of grades, sitting in the comfort of my room while doing these WODs won’t exactly induce the same panic and anxiety.

Nevertheless, I shall keep an open mind, and see how these WODs make or break my ICS journey.
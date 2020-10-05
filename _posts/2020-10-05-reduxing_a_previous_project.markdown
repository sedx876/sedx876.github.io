---
layout: post
title:      "Reduxing a Previous Project"
date:       2020-10-05 12:06:36 +0000
permalink:  reduxing_a_previous_project
---



I have finally arrived...Final Project for Flatiron. It feels like it took forever..yet not, all at the same time. It was everything they promised, scary...exciting...stress inducing with a satisfying after taste.

**D3 Playr Companion** is a small app the help players of the game, Diablo 3 keep track of character builds and item drops they need in game. As a avid player of the game I always found myself writing on the back of junk mail envelopes to keep track of what I was doing in game. This was perfect opportunity to fix this problem with my new found skills.

![D3 Playr Companion](https://i.ibb.co/jz1pX5b/d3about.png)

When hearing from previous Flatiron graduates you get a little feeling of what is to come. One of the things I kept hearing was how challenging Redux can be. I braced myself for this roadblock and tried to prepare myself.

Redux: is a small library with a simple, limited API designed to be a predictable container for application state. It operates in a similar fashion to a reducing function, a functional programming concept. It is influenced by the functional programming language Elm.

So what does that actually mean to devs that actually have to work with it? Basically it is a more elegant way to manage state in an app.

With vanilla React you may have to drill through layers and components to access props and state which can get a bit messy as your app grows in size and can cause errors and unwanted behaviors. This is known as prop-drilling.

With Redux we take the state and move it to the side so we can access what we want, when we want without disturbing components and layers that may have nothing to do with what we are currently needing.

Basically there are two main parts to Redux which are actions and reducers. Actions tell us what we are going to do. Reducers tell us how we are going to do it.

**Actions**  are payloads of information that send data from your application to your store. They are the _only_  source of information for the store. Actions are plain JavaScript objects. Actions must have a `type` property that indicates the type of action being performed. Types should typically be defined as string constants. Action creators are the functions that encapsulate the process of creation of an action object. These functions simply return a plain JS object which is an action. It promotes writing clean code and helps to achieve reusability.

**Reducers** are a function  that determines changes  to an application’s state.  It uses the action  it receives to determine this change. It helps manage an application’s state changes in a single store so that they behave consistently.

**State** changes are based on what the user does. So if the state changes it will happen inside the reducer function.

Ultimately when a user trips an event it is sent to the action(The “what we are going to do”) then it is sent to the reducer(The “how are we going to do it”).

I will admit at first the Redux was confusing and intimidating. Then I had the cliché light bulb moment during a Redux lecture. It was explained simply and expertly(Thanks Aysan!!!). Honestly I would prefer using React and Redux in tandem from now on. It does make your app simpler in cleaner.

All in all I am happy with the result. I still have a long way to go with making the code cleaner but as always it is a work in progress.

---
layout: post
title:      "All The Small Things"
date:       2020-01-08 14:21:02 -0500
permalink:  all_the_small_things
---


My second project for Flat Iron School was to build an app using the Sinatra framework. As stated on the Sinatra Homepage…. **”Sinatra is a DSL (Domain Specific Language) for quickly creating web applications in Ruby with minimal effort.”** 

Think of Sinatra as Rails’ little brother…….

Our main objective was to build a `CRUD` (Create-Read-Update-Delete) app with a `MVC`(Model-View-Controller) architecture that could show relationships between models.

Sinatra is a great way to get a simple app built and running. But that is not to say there are a few small things that may trip you up in production if you are new to Sinatra.

`Bcrypt` is a `Ruby Gem` that will encrypt a password within your databse. The main point you have to remember is to use `password_digest` in your tables when performing migrations.

`Rack::MethodOverride` is basically a hack to get patch requests through. If you forget to add this line to your `config.ru` then you may be into some frustrating debugging.

One gem that could make your build a lot easier is the `Corneal` gem. This gem will generate a file structure for you automatically with a few simple commands.

One of the best things I did was to plan out my project on paper. It took a lot of guess work out and things definitely went a lot smoother. Organization must become my new BFF.

For me personally I felt a bit less stress with this project then with the first project. Sinatra takes care of a lot of the logic behind the scenes so one can concentrate on how the app will work and look.

Overall it was a positive growth experience and I look forward to building even more with Sinatra.

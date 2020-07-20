---
layout: post
title:      "Out of time"
date:       2020-07-20 19:22:52 +0000
permalink:  out_of_time
---

My time working through the Flatiron Software Engineering self-paced program is coming to an end. The MVP of my final project is complete: an app with a React.js frontend and a Ruby on Rails backend. 

In picking my project, I thought about the way I like to study or complete tasks I don't want to do. For both, I use timers! I pick a certain length of work time (usually 20minutes for a chore, 30-40 minutes for studying) and then a certain break length (usually 10minutes for a chore, 5 minutes for studying...with longer ones thrown in after a few cycles). This is similar to the popular "pomodoro method," but what actually inspired me was seeing a 20/10 work/break cycle touted on a home organization blog. Both methods are built from the same science that shows improved performance with frequent breaks! So, what I came up with was a project that allows a user to save timer cycles for various activities. Let's say you want a cycle of 20min work/10min break. You can save a timer that will go off at 20 minutes and then 10 minutes. You can also pause at any time, reset a cycle at any time, and skip to a break at any time.

This project was a lot of work, in part because there is so much to learn in React.js. It is such a popular framework that is expanding and receiving updates all the time, so I had to decide if I wanted to take some extra time to learn the latest best practices (React hooks), or if I wanted to stick to what I learned in the Flatiron lessons to build it. In the end, I went with the latter, because it will give me a chance to solidify what I learned through Flatiron before I move on, and I have plenty of time to build a new project using React hooks after graduation.

A big lesson I learned from this project was to always split up a large task, function, or React component into smaller pieces that are easier to work with. I had a lot of trouble working out my timer logic, because state needed to change when they were in work and break mode, and I was doing WAY too much logic in my Timer component. Finally, I extracted all of the logic and state out into a new parent component, and immediately was able to solve all problems. 


---
layout: post
title:      "A sinatra project that sings"
date:       2020-04-16 19:31:10 +0000
permalink:  a_sinatra_project_that_sings
---

Deciding what to build is always the hardest part of any project for me. I knew I needed to pick something I was passionate about, and something that I would genuinely want to use.  Opera singing is the career path I am moving from, and as this is a quite niche interest, there is not a lot online built for us. I wanted to create a site where opera singers could keep track of the roles they are working on, track progress, and share notes with others. 

The most difficult part of the planning stage was keeping it simple. I thought of many, many ways I could create the site I wanted, all with various pitfalls and difficulties. I settled on sticking with the simplest version that would allow me the features I wanted. This was a User class, which had many Roles, and a Roles class that belongs to a User. The Roles class has a whole lot of attributes, including six boolean attributes that I thought of as "tasks", to be checked off on a form as each is completed. 

Figuring out how to make my boolean attributes work how I wanted was the biggest hurdle of my project. The tricky part with using booleans in a checkbox feature is making sure boolean attributes are either true or false - avoiding the dreaded third state of "nil". I did so by adding "default: false, null: false" to each boolean attribute, and this worked like a dream! When a form is submitted with checkboxes, unchecked items are not included in the params hash at all. By making sure they defaulted to nil, when using mass assignment with the params hash in create(params) or update(params), boolean attributes that were not in the params hash were set to "false", while those checked off were set to "true". This made coding the show pages work like a dream. Ruby lets you check if a boolean attribute of an instance is true or false simply by using: instance.attribute?. 

I learned SO much from this project. It clarified a lot of topics that were still muddy to me, like the sessions hash and how mass assignment works with Active Record. I am so thankful to flatiron school for giving us such interesting projects, and for the helpful video library on the subject!

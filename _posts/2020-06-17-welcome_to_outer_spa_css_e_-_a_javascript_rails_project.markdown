---
layout: post
title:      "Welcome to outer spa(css)e - a javascript+rails project"
date:       2020-06-17 18:45:09 +0000
permalink:  welcome_to_outer_spa_css_e_-_a_javascript_rails_project
---


I had an extremely hard time deciding what I wanted to do for my rails+js project. I was a bit bored of the blog-like style of project I had done for Sinatra and Rails, where a user submits some information which you can then view on their user page, formatted but still parroting back information a user had submitted. I wanted to make something more like a game, where the user interacts with the site in a fun way. I came up with many ideas that were just too complicated for this style of project. Thinking through topics I liked, I decided I wanted to make something space-related. I realized that using pure CSS and html, a solar system could be drawn. Since this was true, a solar system could be altered by changing aspects of the CSS, and thus users could submit information about the solar system they wanted, and a personalized solar system could be rendered.

Doing this was a challenge with my beginner CSS knowledge, but I really like how it turned out. A user picks the sun's spectral type, and this determines the size and color of the sun. Then, they decide the number of planets they'd like. Finally, they create each planet, setting attributes like name, composition (which determines color), size, and whether or not the planet has rings. I have three models: a solar system, sun, and planet model. The solar system has one sun and many planets.

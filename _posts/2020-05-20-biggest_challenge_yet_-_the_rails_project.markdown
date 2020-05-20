---
layout: post
title:      "Biggest Challenge yet - The Rails Project"
date:       2020-05-20 16:31:23 +0000
permalink:  biggest_challenge_yet_-_the_rails_project
---

​
When I decide what topic I want to use for a project, I tend to think about real people. This project was inspired by a friend who pulled out a list of all the anime he'd seen, written messily in the notes app of his phone. I wanted to make a site that would let people essentially make lists of all the anime, tv shows, books, etc. that they had experienced. There were many ways I could have set up this project, and if I had a full month to work on it, I would have maybe done seperate models for each media type. Instead, I settled on four models: User, Experience, Medium, and Category. Medium was to be my join table between User and Medium, similar to how a post or review would be in various example projects. The Category model was to help me sort between medium types and keep them mostly seperate in the views.
​
To keep this from getting extremely long, here is a bulleted list of the things I learned doing this project:
* **Figure out what you want your user flow to be BEFORE coding your views.** I naively thought that just fleshing out my models before writing any code would be enough, but it ended up being extremely hard to figure out how to make all my view pages come together in a neat way, and I'm still not fully happy with the result. I will definitely use something like Figma before my next project, and spend as long as I need in the planning phase.
* **Don't be afraid to use yield in your partials.** The way I ended up using my Category model was a strange sort partial that I called "category_organizer." In it, I iterated through my Category instances and passed them through to a different view throgh yield(category_instance). I then used this category instance in two different ways - one to sort a user's media by category, and one to take advantage of the has_many relationship to make a media index page sorted by category. While I may in the future find a cleaner, faster way to code this, it was a great learning experience to make it work and DRY up my code!
* **The console is your friend when figuring out scope methods.** I cannot count the number of times I typed "rails c" during this project. What a useful tool! It was especially necessary when figuring out my scope methods, as I wanted to relate my User with my Medium - and as they are joined by a join table, I had to include that too, joining THREE tables together. Luckily, because they are associated, rails documentation gives an easy way to do this. Here's a link if you'd like to read more on this: [https://guides.rubyonrails.org/v5.0/active_record_querying.html#joining-tables]
* **Writing custom CSS is HARD as a beginner.** Enough said. I will be looking into Bootstrap or similar libraries for next time ;)

Overall, I had a lot of fun building this project, and though it is not perfect, I enjoyed it immensely and cannot wait to continue making improvements.

---
layout: post
title:      "Baby steps to CLI magic"
date:       2020-03-02 01:43:46 +0000
permalink:  baby_steps_to_cli_magic
---


The CLI Data Gem Portfolio Project was some of the most fun I've had so far during this course! Before I picked my topic, I was TERRIFIED. I had no idea where to start and I struggled through the extra hard labs leading up to it. After browsing through the code of other submitted projects and watching some video walkthroughs, I felt slightly more ready. However, it was picking my topic and practicing scraping that really made me excited.

After some thought, I decided my project was going to center around a French cartoon that I've been watching for years called *Miraculous: Tales of Ladybug & Cat Noir.* As this show gets released in multiple countries, episodes are often released in a bizarre order. I decided to make an application that would let a user select a season and see a list of episodes in that season. I gave an option to receive the episode list in order of release date or by production code (in my opinion the superior watch order). Additionally, the user can enter a production code or episode title to get the details of the episode formatted with production code, title, and release date.

The key to making this project go smoothly was taking baby steps, focusing on one thing at a time. I am the kind of person who tends to jump from topic to topic and start too many things at once, so this was a great exercise for me. The very first thing I did is something that is often the last in these types of projects, and that was the scraping itself. I was nervous that I'd do the entire project and end up stuck at the end unable to scrape the website I chose, so I made sure it was possible from the beginning. Unfortunately, all of the data I wanted was nested inside of tables in the website so it took some trial and error to get the data pieces I wanted. I ended up picking some class selectors that would give me ALL of the table text line by line, and from there I could split the data how I needed and grab it by index. Instead of iterating through scraped data with each, I used each_with_index so I could specify index ranges for the tables I wanted. I had to account for a range for each season, so three index ranges total. While it looks a bit weird, it worked exactly how I wanted it to in the end.

Once I had my scraping down, I followed along with the famous DailyDeals CLI walkthrough video. I went slow and steady and stubbed all the methods I wanted as the video went along. It really helped me stay organized and on track. I would pause the video, make a stub method that made sense for my program, and continue. I inserted puts statements into my method stubs to make sure I was able to call methods from the correct class and all my require_relatives were working. Once the skeleton was created, I found it so refreshingly easy to add real data and code into my program! Taking it slow and steady and focusing on making small parts work one by one was so much easier than trying to get the whole thing working at once. 

One thing I was nervous about in this project was not feeling the joys of making a test pass like I was so used to doing in labs. What I wasn't expecting was how satisfying it was to make something work functionally! Adding functionality bit by bit to my program was even more satisfying than making tests pass. It has inspired me in future labs to think not just about how to pass the tests, but about why the tests were written in the first place and what functionality it could add to a program. 



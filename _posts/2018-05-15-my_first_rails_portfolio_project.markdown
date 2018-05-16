---
layout: post
title:      "My First Rails Portfolio Project"
date:       2018-05-16 01:48:57 +0000
permalink:  my_first_rails_portfolio_project
---


I started this project thinking about the different possibilities on how I could display relationships between multiple objects. As an avid movie fan I naturally decided to make a simple IMDb style website. With this website I wanted to be able to have lists of movies and when I clicked on them I could see the actors who appeared in those movies. If I was to click on an actor, it would then show me the movies the actor has been in. A simple concept but it was a bit tricky for a newer programmer.

I started out strong by setting up the models and databases to make sure the base functionality for the website was there. I knew I would need a join table considering that movies "have many" actors and actors "have many" movies. I then began to make the base controllers. Just the stuff I knew I would need like index, new, and show methods. I then added the corresponding views and routes to be able to start testing things.

I made a simple index to list all of the movies in my database. Same for actors. I then made it so that I could link back and forth between movies and actors. I added show pages with detailed information for everything. Everything was going smoothly until I started to implement nested forms.

Nested forms are tricky at first. What I learned a lot doing this project is you have to really think about what information is available to you, and HOW you're getting that information. Whether it's coming from your controller or the URL or some other rails magic. By playing with the website, you really start to understand the rails magic that is happening. After some effort the nested form became a little easier to understand. Do I fully understand it now? No, probably not. But I'm confident that I could do it again in the future now.

With forms and all of the dynamic view pages taken care of, it felt like I was almost done. Then I went on to implementing users and sessions. I probably spent the most time on this. I think I could have gotten it done quicker, but I really wanted to make sure I understood everything that was happening when a user was considered "logged in". I constantly played with what kind of information I could save in a session and how I could access that information and what I could do with it. It made me really understand how it all works under the hood.

The next big hurdle was implementing OmniAuth. This took me out of my comfort zone a little bit because I'm perfectly comfortable using my own code to do things but once this authentication forced me to communicate with github's code, I got nervous. I had a little trouble because I was trying to verify it based on the email saved to a person's github account. Little did I know that your email doesn't show up unless you have "public email" checked in your github account. So instead I decided to use the github id to verify since I knew that would always exist.

After all of that it was just a bunch of quality of life tweaks. Like links to different things so you dont have to hit the back button all the time and so you don't have to physically type in the whole address for everything. It was fun, I learned a lot, and I definitely feel more confident with the back-end of web development now.

---
layout: post
title:      "Sinatra Portfolio Project"
date:       2019-08-23 18:30:17 +0000
permalink:  sinatra_portfolio_project
---


For my Sinatra Portfolio Project I decided to create a simple recipe web app. Sinatra is a simple framework that is ideal for such a task. 

I like good food and to have good food you need to either go to restaurants or be a good cook. Since going to restaurants isn't always an option (nor cheap) I had to become a good cook. Just like programming, you get better with learning, sometimes through trial and error, sometimes through experimenting or through reading/watching what others did or are doing.

Frequently I look up recipes online. On the web there is a lot of blog-based recipe sites. One thing most of them have in common is that they start with a long article that explains how they came up with that idea or what makes it special. That's fine. It's normal to do. Sometimes I read those articles, but most of them I do not. I usually skim past them and get to the recipe and instructions. The problem I have with this approach is when I'm cooking I forget what I need to do next. I open the recipe on my phone browser. It usually takes a long time to load. You can't scroll fast enough to the recipe. And it interrupts you with pop ups. By the time I get to the necessary step that I forgot, my food burnt in the pan and I had a negative user experience. 

The web app I created focuses only on the recipe. Users can create an account, they can create new recipes, list them, update or delete them. Creating an MVC structure in Sinatra is a concept. First I had to create migrations to the database that uses Active record. After creating migrations for users and recipes next step was creating models and designing the relations between the models. After the model part it was time to create the controllers and views. I separated the controllers into Users and Recipes. Same was done to the views. I used the bcrypt gem to create safe storing of passwords and to validate the user login input. Another frequently used gem during development was shotgun. When used properly it can streamline the creation of views and make it easy to implement minor as well as major changes. The base structure of my project was created with the corneal gem. It is very useful for this. 

At first my plan was to separate recipe ingredients and instructions into their own models but after reaching the point how to implement it into the forms I realized I don't have that knowledge. I wanted to create auto generated fields for them. After some research I realized I would need a better understanding of JavaScript. At that point I decided to not worry about that and stay with the plan and learn JavaScript with the curriculum. It was a humbling experience. Also, that felt like a great opportunity to play with branches in GitHub. I already had created migrations, set up models, made controllers and started working on views for Instructions and ingredients respectively. It felt like a lot to delete all those files and just make a small comit. I wasn’t sure if nothing will break. After cleaning out the structure and implementing ingredients and instructions into recipes I merged the two branches and continued to finish my project. 

Working on this was a pleasure. It felt great to sit down and navigate in browser to the differnet pages I made. There were moments where I would take a break and I would only think how to make the next step.  I'm looking forward to see what Rails will bring. 

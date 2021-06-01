---
layout: post
title:      "Rails React & Redux Project"
date:       2021-06-01 14:41:49 +0000
permalink:  rails_react_and_redux_project
---



### Game Cave

The idea was to create a web app were I can put in different game publishers and their games in one site and keep an eye on my thoughts and if I have finished the game. Nowadays, there are too many gaming stores (Origin, Steam, UPlay...). That's it. Just a one stop to check on my game library. 

### Backend

I used Rails to create a backend API to save my data in. I used the Serializer gem to send the JSON data. My DB consist of 2 tables, publishers and games, where games belong to publishers. The controllers have the ability to Create, Read and Delete. 

### Frontend

##### React & React-Router
The frontend is made with React and Redux, minimal styling is done with React-Bootstrap. I used the create-react-app generator to start it off which made a lot of things easy. My two container components are GamesContainer and PublisherContainer. For my stateless components I chose Games, Game, NavBar, Publishers and Publisher. There are two more components that handle the inputs, PublisherInput and GameInput. Both of these components have received styling by React-Bootstrap. 

All the routes are handled inside publisherContainer with a Switch component. There are 4 routes. 

###### Redux & Thunk

The redux store and Thunk are imported into Index.js. The reducer I am using I called publisherReducer since all the data is being fetch through the publishers. I was debating about fetching games directly, but after carefull consideration there was no benefit of fetching data that was already available inside publishers. The reducer handles actions for both publishers and games. I have 4 actions: fetchPublishers, to get the data from the backend. addPublisher and addGame, to persist new publishers and games to the DB that users created. Delete game, which allows users to delete a game for whatever reason they want to do it.

### Future Add-ons

It would be nice to update the publishers. The published datetime is not properly utilized, I planned to make that as a sort function. Adding users would be nice. Providing pictures for the games as well. 


### My Flatiron Journey is coming to an end. 

I'll never forget the words my dad said to me after I got my drivers license: "Congratulations, now that you have a DL you oficially don't know how to drive!"
At that moment I didn't fully understand what he meant. I was caught off guard. I just received papers that I do know. It was evident I didn't know how to drive the first time I found myself in a big city. 
With my Flatiron Journey coming to an end I see many similarities. The feeling of success and the posiblity to call myself a Full Stack Web Developer. I know how to create Web Apps now.
On the other side, there is still so much to learn. Different languages and their frameworks for backend and different JS frameworks. Deploying web apps, maintaining sites and optimizing them. But, all of these things I am looking forward. Eventually they will become part of my repertoar just like writing an IF statement is. 



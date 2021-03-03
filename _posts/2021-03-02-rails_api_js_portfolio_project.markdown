---
layout: post
title:      "Rails API + JS Portfolio Project"
date:       2021-03-03 01:47:06 +0000
permalink:  rails_api_js_portfolio_project
---


## World National Parks
A one stop website to place to display all the national parks. 
#### What I made
I used Rails to create a backend API, that stores National Parks from different countries.

First I had to come up with this idea. I love hiking, and visiting national parks. I feel that the the US National Parks have a good representation online. Nation Park Services(NPS) has an open source Park API and they keep creating new apps and features constantly, just recently they deployed their new app called NPS. The other countries parks are a bit hard to find information about. 

The goal is to create a website where all the parks on our beautiful world are listed. 
#### Backend
The backend is supported by a Rails API that I have made. I have connected it to PosgreSQL, I might deploy it down the road on Heroku. I also separated the Backend and Frontend into different repositories. The Project requirements are to have a one-to-many relationship DB. My models are Parks and Countries (a country has many parks.....). The controllers render data to JSON. I also utilized the Serializer gem. 
#### Frontend
I wanted to keep this as clean as possible. The only framework I am using is Bulma.css for the styling. I chose Bulma because it is lightweight, clean syntax and no JS frameworks required. The index.html page is all written by me with classes from Bulma added here and there. I mainly used IDs when I needed to connect something to JS. JS is made with OO functionality. I have a park.js and country.js that have same named classes. Inside index.js I have made 4 fetch calls, get and post parks, countries. I have a function to handle form submision for a newly created park. 

I wanted to have countries inside a dropdown field, which was dynamically filled in, plus it auto updates when you create a new country. This was the biggest challenge of my project, some due to my inexperience with JavaScript some due to the lack of understanding how does JavaScript work inside the browser. I have spent a good amount of hours inside the debugger and was chasing some wild errors. Sometimes I would fix them, sometimes I would realize it isn't possible because I am calling on the function before the fetch got executed (quite painfull when you get undefined from console.log in your code and inside the browser it returns you the object you are looking for).

#### Conclusion
I have had fun building this project, some things I would like to add in the future is to edit park information and add more pictures, leave ratings and comments on it. 
I have learnt a new framework that I believe I will use in the near future again because of how modular it was and how much pleasurable it was. 
It felt great going back to Rails after learning all the quirks JavaScript has, it was nice, even if it was only for a small application. 
JavaScript and I will be butting heads more and more in the near future. I feel like we are at the beggining of a lasting love-hate relationship. 
I am excited to start learning React. 


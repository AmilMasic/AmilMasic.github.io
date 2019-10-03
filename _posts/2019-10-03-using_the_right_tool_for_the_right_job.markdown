---
layout: post
title:      "Using the right tool for the right job"
date:       2019-10-03 21:23:11 +0000
permalink:  using_the_right_tool_for_the_right_job
---

What does that mean for us flatiron students? 

For me personally, it means knowing how to approach that current test in my lab that isn’t passing. Am I going to google and use StackOverflow or am I going to read the documentations? Am I going to reach to my bookshelf and grab one of those books I have? My goal of this blog post is to explain how I approach now problem solving. 

I wasn’t always like that. My approach to solve a lab when I was stuck was copy paste the error message and hope for the best. I’ll find any article, more than often it would be from StackOverflow. Copy/paste the highest up voted solution into Atom. Try to adapt it to fit my objects. Run learn. Red. Check the code to see if I deleted any quotation marks, check commas, run learn again. Red.

Go back to searching for a different solution. Find it. Again changing it to fit the objects. Red again. There usually are some solutions that fit the problem but are written in a different language, a few times I thought to myself to decode those but I never went down that path because it will probably take too long and there is no guarantee it would work. It would be madness. At this point I would either keep trying or take a break, come back later to the problem with a fresh mind. Fresh ideas for searching. Often times I would find the solution and it would be green! What a relief, but sadly, no dopamine kick. 

Another valuable approach is to ask a question on a lab. The technical coaches do a fantastic job explaining and brining me to a conclusion. If things got tangled up badly there is always someone ready to jump into a screen share. Most of the times, the solution that comes from this approach is usually simple. (Thank you TCs, I really appreciate all of yours help.)   

On the other side, there are moments where I think I know what I’m doing, but I can’t remember the exact boilerplate or I have the “what was that .method again?” moment. The usual way I try to solve this is to either check one of the older labs to find the answer or I go to the documentations to search for the answer. I find what I need. I apply it to my problem. Run learn. Red. I forgot a comma. Run learn again. Green! Dopamine kicks in. 
I don’t know about you but the dopamine kick I get from problem solving is one the things I love about coding. It’s a great experience and provides a stronger desire to keep on pushing and do more work. 

Thankfully, things have changed when it comes to my approach to solve errors.
I had the pleasure of attending Dwayne Harmon’s study group called “Googling for web developers”.  Dwayne explained how to make google work for you, using features like the “+” symbol. 
This one helps define that you are specific about something. Example, the programming language and/or framework that you are working in; a search could look like this: “ruby + rails + random error message.” 
Another example would be putting a sentence in quotations so google looks for articles with that actual sentence in it. 

Apart from that, Dwayne shared a story that he worked with a seasoned programmer on one of the WeWork locations. He mentioned that this person doesn’t like to google for errors. Instead he reads the documentations. He is slow and very careful when reading them.  Most of the times, it felt faster than searching on google. 

Why? Because the answers on SO are usually to a specific edge case that might not be the best for the problem. The documentation gives a relatable solution. The questions and answers on SO could be from the late 2000’s which has the possibility to be outdated. The documentations are usually up to date. 

I thought about it. I decided to implement a lot of the things that Dwayne suggested. Oh what a great success it was. In my most recent lab I had to set appointment to have a date and time, but also be human readable. I decided to go with the subclass of DateTime, which worked great. However, the human readable part was a bit tricky. By default, DateTime gives the following output “11 23 2011 20:20 UTC”. 
The lab requirement is to get the result to be “November 23 2011 at 20:20”. First approach was with split and join. Got a ton of code that was messy and didn’t give the desired output. Second approach was to go to ruby docs and search for DateTime and read the documentation to see if there might be a method available. 
I found the method .strftime. The options in that method are intimidating. After reading through it I found the things I need, I wrote it into my custom method and boom! It worked! It was one line of code and I achieved it thanks to the documentations.
For the curios ones, here is the method: 

```
  def formated_datetime
	   self.appointment_datetime.strftime("%B %d, %Y at %H:%M")
	end
```

It felt great to figure that one out without searching the forums for a hopefull answer. All it took was reading the documentation. Writing a one-line method and the reward was a good amount of dopamine. 

I’m not trying to say that going with the documentation is the only right way or that googling SO and other places is a bad practice. There are situations where it makes sense to read the forums, I couldn’t have set up my environment properly if it wasn’t for googling on SO and askUbuntu and all the help provided by technical coaches. 

Using the right tool for the right job requires a good amount of knowledge how to approach the problem. 
Dwayne’s study group definitely helped me in the decision making for the right tool. I first think now what part of my error message is obsolete for searching. How can I rephrase so it makes more sense? Is this an edge case or a more common problem? 
Should I google it or should I go to the documentations.  I highly recommend attending Dwayne’s study group if he decides to do it again. I only wrote about few things he mentioned, there was way more that he taught in his study group.


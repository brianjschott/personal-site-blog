---
title: Mind Meld
Description: A mind meld app
Author: Brian Schott
Date: 11-17-2018 6:31 PM
Robots: 
Tags: ruby, sinatra, app
Template: blog-post
---
Sometimes it's tough to make time for coding projects, but it really is beneficial to my teaching. You have to be making things and practicing your craft in order to get better at it! I wanted to revisit a project I had done during my Upperline teacher bootcamp, so I deployed one of my Sinatra apps, [Mind Meld](https://mind-meld-sinatra.herokuapp.com/), to Heroku.

Offline, it's a great icebreaker game: Pairs of individuals have to shout the same word simultaneously; if they fail, you try to find a word "between" the two you guessed, until you land on the correct one. So a typical car might go like this:

Car!	Table!

hmmm... (each player thinks of a word between the two)

Pickup truck!	Metal!

hmmm....

Bumper!	Tailgate!

hmmmm....

License plate!	License plate!

**commence high-fives**

[This version](https://mind-meld-sinatra.herokuapp.com/) uses an API called [DataMuse](https://www.datamuse.com/api/) that looks for relations between pairs of words. The computer starts by picking a random word from a dozen seed words, using their random word endpoint. It then uses its "trigger words" API, with two inputs, to find a word that matches both the user and the computer. If no luck, it just attempts to match against the computer's guess. If still no luck, it guesses a random word again (thankfully, this doesn't happen unless the user doesn't pick a well-known word or misspells it).

It was a fun project to see if it was possible!  I managed to pull it off in about 5 hours last June with a little bit of help from my co-teachers, who handled the frontend and brainstormed backend structure. 

Yesterday I ironed out a few bugs and deployed it to Heroku. It was a great feeling getting to publish a fun app after so long!


---
layout: post
title: "Graphics Sets Project"
date: 2014-09-21 13:24:00
categories: programming projectlog
---

## Sets Project

![Sets Project]({{}}/images/sets.jpg)

For our first homework assignment we were asked to implement a graphical front end for the card game sets. This was a 2D Graphics programming assignment in C using OpenGL.

I decided to use Microsoft Visual Studio 2013 as the development environment. I had not used that IDE before, but after spending some time with it I found it to be very useful.

Since the assignment was in 2D there were many different ways one could approach it. I decided that I would focus on code re-use as much as possible in implementing this project.

Extra Credit implementaion

![Mini Cards]({{}}/images/sets_ec.jpg)

After I had finished with the main project, I decided to tackle the extra credit portion. One of the options was to draw mini squares indicating progress in a game. This was a task simple enough. The other was to implement miniature cards to represent sets that had already been found. My earlier decision to focus on code reusability really shone here, becuase all I had to do was to use a glScale call prior to entering my existing draw methods, and the cards were drawn without issue.

I also incorporated logic to draw a second row of cards after 6 cards had been found to prevent overflow. According to reading I did about the sets game, a maximum of 12 sets can be found in a legal draw of of a sets hand. This would be very unlikely, like i-should-have-bought-a-lottery-ticket unlikely, but I decided to implement it nevertheless.
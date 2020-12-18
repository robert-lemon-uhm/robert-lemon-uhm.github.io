---
layout: project
type: project
image: images/LogoJava.png
title: "2048"
permalink: projects/2048
date: 2019-12-06
labels:
  - Java
  - Eclipse
summary: I coded the game 2048 in Java for my final project in ICS 111.
---

<img class="ui medium right floated rounded image" src="/images/2048UI.png">

This project was meant to demonstrate a fundamental understanding of the basics of Java.  Title images were created for the introduction screen, as well as the winning and losing screens.  The game itself was created using a 2D array that stored tiles, a class that was created for this project.  Each tile had an associated coordinate, value, and color, and moved based on user input.  This basic functionality incorporated continuous while-loops to gather user input, maintenance and storage of objects within a matrix, and organization of graphics drawn on the screen.  Collision needed to be detected, and the combination of tiles needed to occur in a certain order, as corresponding to the original game.  In order to win the game, a tile of 2048 must be produced, so this was checked when each tile updated.  In order to lose, there can be no more valid moves left.  To achieve this, the entire matrix had to be iterated over whenever the board was full, checking if there were valid moves left.  As the only programmer for this project, I had to figure out how to implement all of the methods.

You can view the whole code in the [GitHub repository](https://github.com/robert-lemon-uhm/2048Java) for this project.

___

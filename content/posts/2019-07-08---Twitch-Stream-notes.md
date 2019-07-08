---
title: Twitch Stream Notes - July 8, 2019
date: "2019-07-08T12:46:37.121Z"
template: "post"
draft: false
slug: "/posts/twitch-stream-07-08-2019/"
category: "Twitch Streams"
tags:
  - "Twitch"
  - "Stream Notes"
  - "Python"
  - "TDD"
  - "Game of Life"
description: "Weekly stream for July 8th, 2019. Building Conway's Game of Life in Python, TDD Style."
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/i6vrIdpbPCo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## What we did

### Show and Tell

- [My NDC Oslo Talk is up on YouTube](https://www.youtube.com/watch?v=5SYjR2D4p0c&list=PL03Lrmd9CiGe9QtFC8LRRqknzpKgcrWpe&index=134)
- [breakingthings.io](https://breakingthings.io)

### Conway's Game of Life in Python! 

- What is [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life)?
- Create a new project, [`py-conway`](https://github.com/bsatrom/py-conway)
- Find a good Python TDD Framework
- Using a TDD Approach, start building out the game
  - Create a `Game` class that takes a `numpy` array as a seed
  - Create a beacon to represent the initial state of every cell
  - Display the initial state using `matplotlib` (We did this in a separate `run.py` script to keep the game management separate from display concerns)
  - Add functionality to check for the number of neighbors to a single cell

### Next Time...

  - Run the game with a single cell on
  - Run the game with two cells on
  - Run the game with three cells in a linear orientation
  - Animate steps
  - Check for invalid types (thanks @DontCallMeLatrForDinner)

## What we learned

- [Python has a Unit Testing FW built-in to the standard lib](https://docs.python.org/3/library/unittest.html), thanks @roberttables

## Thanks!

- @roberttables for the 4-mo resub!
- @visualstudio for the host!
- @SurlyDev and @strick0 for the live coding help!
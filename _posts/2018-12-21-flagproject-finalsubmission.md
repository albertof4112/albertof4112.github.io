---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## Flag of Pakistan by Alberto Fernandez

## Describe your program

The country I designed my program for was Pakistan.With my creation of the Pakistan flag on pyret, I expect a professional grade on it due to having dimensions, simple parts, and combinations of simple parts.

## Current output

* * *
![Pakistan.Flag](/images/bestpakistanflag(epic).png)
* * *

## Describe your process.

Firstly, questions I asked to help improve my Pakistan flag were "How do I calculate the exact angle of the star if websites don't mention it?, How do I create a crescent in pyret if there are no crescent shape funcitons?, and How do I make my flag so that I can change one number and the entire size changes?" These questions helped me developed strategies that turned my flag into a professional level like searching for star geometery, using two overlapping circles to make a crescent and by using dimensions in my code. Most of this help I got from the teacher but I did create all of the dimensions code by myself with my own thinking.

## Explain your code.

-   Choose a significant part of your program (15 lines max) and paste it below. Do not insert your entire program here. _then delete this instruction_
```
# Dimensions

height = 200

width = height * 3/2

stripe-height = height / 1

stripe-width = width / 4

star-radius = 1/10 * height

crescentwhite-radius = 3/10 * height

crescentdarkgreen-radius = 11/40 * height

rectangledarkgreen-height = height * 1

rectangledakrgreen-width = width - stripe-width
```

This section was my "dimensions"part of my code. The first two lines are the height and width of the flag, with the height being the most important part as it is the one where I can change one number and change the entire size of the flag program. After this, I have my white stripe heigh which is the same as my flag height and the width that is 1/4 of the entire flag width. I then have the radius or size of my star which is 1/10 of the flag height. After this there is the radius of the white circle that makes the crescent and the dark green circle that makes the crescent, 3/10 and 11/40 respectively. Following, there is the height of the main green dark rectangle which is the same as the normal flag height, and then the width which is 3/4 of the flag width or the flag width - stripe width.

These dimensions control all of the sizes of the program as my simple parts, a.k.a. shapes use these for their size and for their positional placement in combinations of simple parts.
* * *

## Program code

```
include image

# Pakistan Flag


# Dimensions

height = 200

width = height * 3/2

stripe-height = height / 1

stripe-width = width / 4

star-radius = 1/10 * height

crescentwhite-radius = 3/10 * height

crescentdarkgreen-radius = 11/40 * height

rectangledarkgreen-height = height * 1

rectangledakrgreen-width = width - stripe-width

# Simple Parts/ Pieces

DGR = rectangle(width, height, "solid", "dark-green")

WR = rectangle(stripe-width, stripe-height, "solid", "white")

WC = circle(crescentwhite-radius, "solid", "white")

DGC = circle(crescentdarkgreen-radius, "solid", "dark-green")

WS = star(star-radius, "solid", "white")

RWS = rotate(18, WS)

# Combinations of Simple Parts

WR-DGR = place-image(WR, width / 8, height / 2, DGR)

WC-WR-DGR = place-image(WC, width / 1.60, height / 1.95, WR-DGR)

DGC-WC-WR-DGR = place-image(DGC, width - (width * 0.31666), height - (height * 0.5625), WC-WR-DGR)

Pakistan = place-image(RWS, width - (width * 0.28333), height - (height * 0.625), DGC-WC-WR-DGR)

```

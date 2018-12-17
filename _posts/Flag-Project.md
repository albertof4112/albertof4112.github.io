---
layout: post
title: "Flag Project-In Process"
date: 2018-12-14
---

# Pakistan Flag Project Week

We had four days this week to work on out flag project (mine was Pakistan) and since I am the most prepared human being in the world, I started off my project earlier the previous week to get a heads up. Here is the code and flag I have so far:
```
include image

# Pakistan Flag

# Dimensions

height = 400

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

RWS = rotate(28.5, WS)

# Combinations of Simple Parts

WR-DGR = place-image(WR, 75, height, DGR)

WC-WR-DGR = place-image(WC, width - (width * 0.38333), height - (height * 2), WR-DGR)

DGC-WC-WR-DGR = place-image(DGC, width - (width * 0.31666), height - (height * 0.5625), WC-WR-DGR)

Pakistan = place-image(RWS, width - (width * 0.28333), height - (height * 0.625), DGC-WC-WR-DGR)

```
![Pakistan.Flag](/images/flagV2.png)

As you can see, the flag is a very rough draft. You might also be thinking that this is a pretty bad flag for working on it for 4+ day but I can explain. You see I had the flag done, everything to proportion, but then I found out that I needed to use the dimensions of the flag so that one number would change the entire size of my flag. This meant I basically had to change everything and am still in the process of editing through it. Two questions I have are how could I change my star rotation so that it matches the one of the actual flag? and is there any way I could work with other people with the pakistan flag to share ideas? A challenge overall is knowing how to put the dimensions where they need to be precisely, and an oppurtunity is all of next week. I still have at least 2-3 class periods (due to wednesday trip) to continue to work on the flag and am confident I can get it done.

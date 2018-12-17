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

As you can see, the flag is a rough draft

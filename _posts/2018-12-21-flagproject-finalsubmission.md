---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## Flag of _insert your country_ by _insert your name_

## Describe your program

-   What country did you design for? _then delete this instruction_
-   What grade do you expect? _then delete this instruction_

<!--- Delete this comment and add your writing -->

## Current output

-   Insert an image that your program currently produces. _then delete this instruction_

* * *
![Flag](/images/final-flag.png)
* * *

## Describe your process.

-   What questions, strategies, help from peers or teacher, or thinking got you to this point? _then delete this instruction_

<!--- Delete this comment and add your writing -->


## Explain your code.

-   Choose a significant part of your program (15 lines max) and paste it below. Do not insert your entire program here. _then delete this instruction_
-   Explain each argument in the code section. _then delete this instruction_
-   Tell us how it functions independently and within the whole program _then delete this instruction_

* * *

```
Insert 10-15 line code section here _then delete this instruction_
```

* * *

-   Explain the code you posted by telling us about each argument.
-   Then tell us how your code section fits into the whole.
 
<!--- Delete this comment and add your writing -->


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

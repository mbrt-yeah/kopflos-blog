+++
slug = "software-development-methodology"
author = "mbrt"
title = "Software development methodology"
date = "2022-07-17"
description = ""
tags = ["Planing", "Methodology"]
+++

## Scrumban

In order to plan and keep track of the development process I will use the [Scrumban methodology](https://en.wikipedia.org/wiki/Scrumban).

This methodology gives me a lot of freedom regarding the conception of the individual features of »kopflos«. Instead of having to plan the entire features-set in advance, this method allows me to do so on-the-fly.

Also, this method is not so strict regarding the timing of the implementation of the individual features. All I have to do is to plan iterations in which I commit to the implementation of a certain set of features.

Last but not least, I like the fact that the work process is visualized by means of a [Kanban board](https://en.wikipedia.org/wiki/Kanban_board). I already used such a visualization-technique successfully for other projects at my day-to-day job.

## Kanban board structure

- **Backlog**: All features that await to be implemented during an iteration.
- **In progress**: All features that are currently beeing implemented.
- **Code review**: All features that are currently beeing reviewed.
- **Implemented**: All features that have been implemented.

The actual Kanban board on which I will keep track of the work process can be found here: https://trello.com/b/Qv0s2ROG/kopflos-work-progress

## Ground rules

- An iteration cannot last longer than two weeks.
- A feature is considered as implemented if, in addition to the source code, successfully passed tests have been created, a sufficient code documentation is available and a code review has been performed.
- A feature implementation that did not pass code review will be moved back to the "In progress" category.
- Every iteration ends with a short evaluation. If not all features have been implemented, they will be earmarked for the next iteration.
- No new features will be planned until the backlog is empty.

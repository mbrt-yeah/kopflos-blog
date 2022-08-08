+++
slug = "source-code-management"
author = "mbrt"
title = "Source code management"
date = "2022-07-31"
description = ""
tags = [
    "Git",
    "Github",
    "Management",
    "Methodology",
    "Planing",
    "Source code"
]
+++

## Overview

In order to manage the source code of »kopflos« I will use a Github repository which is publicly available via https://github.com/mbrt-yeah/kopflos.

Since I'm going to use Scrumban which is an iteration-based development process (see [Software development methodology](/blog/posts/software-development-methodology), I will create a development branch for every iteration before it starts.

This means, that at the beginning of each iteration, at least the following branches will be available in the repository:

- `master`: holds the current working version of »kopflos«
- `iteration\[1|2|...|n]`: holds all the code added to »kopflos« during the current iteration

Once I have established that the code added to the iteration branch during an iteration represents a new current working version of »kopflos«, I will merge it to the master branch and delete it. Furthermore, I will create a new version of »kopflos« after a successful merge of the iteration branch.

## Iteration branches in detail

Every iteration will have it's own branch. The naming of the iteration has the following syntax: `iteration\{numberOfIteration}`.

New code that is produced during an iteration is not directly committed to the iteration branch, but to feature, fix, chore etc. branches stemming from the iteration branch which will be merged with the iteration branch after completing the feature, fix, chore etc.

The naming of these new feature, fix, chore etc. branches will have the following syntax: `iteration\{numberOfIteration}\{typeOfWork}\{titleOfWork}`.

Regarding the `typeOfWork` classification I will follow the [@commitlint/config-conventional](https://github.com/conventional-changelog/commitlint/tree/master/%40commitlint/config-conventional) standard which lists the following types:

- `build`
- `chore`
- `ci`
- `docs`
- `feat`
- `fix`
- `perf`
- `refactor`
- `revert`
- `style`
- `test`

This means that during an iteration, besides the `master` and `itertation\numberOfIteration` branches an arbitrary number of `typeOfWork` branches might be present in the repository.

### Iteration branch example

Let's imagine that during the 2nd iteration a new feature which will add a REST API endpoint to »kopflos« is to be implemented. 

Instead of commiting the code of this feature directly to the branch of the 2nd iteration named `iteration\2`, I will create a new type-of-work branch stemming from the iteration branch called `iteration\2\feat\rest-api-endpoint`.

On implementation of the REST API endpoint feature, I will merge this branch into the iteration branch.
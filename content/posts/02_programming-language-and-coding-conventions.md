+++
slug = "programming-language-and-coding-conventions"
author = "mbrt"
title = "Programming language and coding conventions"
date = "2022-07-28"
description = ""
tags = ["Language", "Planing", "Principles"]
+++

## The language

The core of »kopflos« will be a `Node.js` application. This means that either `Javascript` or `Typescript` will be the programming language of choice.

To be honest, I don't have to think long about this. The choice falls on `Typescript` for the following two reasons: 

- I have been programming a lot with this language lately and am therefore more used to it than `Javascript`.
- The optional static typing and the resulting features at language and IDE level make me more productive.

## The conventions

I will try to follow as closely as possible the [coding conventions by basarat](https://github.com/basarat/typescript-book/blob/master/docs/styleguide/styleguide.md) with the following exceptions:

- I will use double quotes (`"`) instead of single quotes (`'`) for the simple reason that I find them more beautiful. ;)
- I will not use `camelCase` as my file naming strategy. Instead my file names will be all lowercase. Should a file name contain two or more parts, I will use a hyphen (`-`) to separate them (e.g. `remove-file.ts`).
- I will prefix abstract classes and interfaces with a lowercase `a` or `i` respectively (e.g. `a-file-reader.ts`, `i-file-reader`) since it helps me to find my way around in the folder structure of the project.











---
title: 5 Patterns I wish I knew Before Starting my 50k line Go Project
description: How to structure your Golang projects so that they can grow safely
slug: how-to-structure-new-go-projects
date: 2026-06-19 00:00:00+0000
image: head.png
draft: true
# categories:
#     - Projects
tags:
    - Software Development
---

[Digital Carrot](/p/digital-carrot) was my first major Go project. I only knew the basics of Go when I first started and had no idea that the project would grow to a sprawling 50k line codebase. Here are some of the most important lessons about structuring Go projects that I learned along the way.

First a little about my background. I spent the majority of my career from 2013 to 2025 working on Django apps in Python. A lot of people like to lump Python in with Golang purely because they are both ostensibly "simple" languages. This characterization is very misleading. Python is seen as simple because of it's clean beginner friendly syntax. In reality, Python will let you do just about anything, which lets you design clean looking code that works by magic and is absolutely impossible for a newbie to reverse engineer or build a mental modal of. 

## Create a Single Root Context
## Proactively Set Up Mutexes
## Logging
## Settings
## Plan for Concurrency from Day 1

## Error handling

Your ultimate goal when an error is returned is to do one of the following:
- If the error is expected and known, handle it and keep going
- If the error is not critical, surface it to the user and let them figure out how to handle it
- As a last resort, if the error prevents the code from functioning either panic or exit with an error

## Safer Go Routines

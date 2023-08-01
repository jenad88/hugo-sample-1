# hugo-sample-1

Checking out Hugo

Pre-requisites:
Git installed
Github account established
Install Powershell 7+ (not sure if necessary)

Install Hugo: (on windows)
Run on terminal window: winget install Hugo.Hugo.Extended

Create a new repository on Github and create a develop branch.
Clone repository to your computer.

Run in a terminal window:
hugo new site quickstart

then copy everything (all the folders and files) from quickstart folder into your cloned repository

Run in a terminal window:
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke

OR

git submodule add https://github.com/manid2/hugo-xterm.git themes/xterm

Add the following at the end of the hugo.toml file:
theme = 'ananke'

Run in a terminal window:
hugo server

Start browser and type http://localhost:1313/

Press Ctrl+C to stop server

To add a new page to the site run in a terminal window:
hugo new posts/my-first-post.md

## Add some markdown to the file:

title: "My First Post"
date: 2022-11-20T09:03:20-08:00
draft: true

---

## Introduction

This is **bold** text, and this is _emphasized_ text.

Visit the [Hugo](https://gohugo.io) website!

Run hugo server (allow drafts to be visible)

- hugo server --buildDrafts OR
- hugo server -D

Follow instructions here:

https://gohugo.io/hosting-and-deployment/hosting-on-github/

# ComputerCraft-WebSockets
A basic but efficient tutorial to start using WebSockets in order to communicate with turtles from a terminal.

![Alt text](./2021-02-15_03.15.03.png?raw=true "Hades welcomes you, mortal")

## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)

## General info

Hi, welcome on this tutorial to learn how to basicly use WebSockets for CC: Tweaked. This tutorial won't cover the very basic of WebSockets. If you do not know how they operate and you can't make it to the end of this tutorial, I won't be able to help you. But don't worry, there is a plenty of web pages about it on the Internet.

I'm making this tutorial because I wasn't able to find a single good one that explains everything. So I spent a few hours looking for documentation, testing and running my scripts to provide you this. If it helped you, you can star the repo, it will be a huge compensation for me!

## Technologies

In this tutorial, we are going to use the following:

* [NodeJS](https://nodejs.org/en/ "NodeJS Official Website")
* [WS](https://www.npmjs.com/package/ws "WS npm page") - NPM Package for WebSockets

## Setup

### Prerequisite

You'll need a couple of things before starting. This is a tutorial but it seems obvious that I can't do everything for you.
I hope you know what is CC: Tweaked (otherwise, why are you even here?) but I'll explain briefly to you why we use this mod and not Computer Craft.
In fact, it is very simple: ComputerCraft does not handle WebSockets. So make sure you install CC: Tweaked on your Minecraft.
Here is a list of everything you need:

* A modded Minecraft with [Forge Mod Loader](http://files.minecraftforge.net/ "Forge Website")
* [CC: Tweaked](https://www.curseforge.com/minecraft/mc-mods/cc-tweaked "CC: Tweaked CurseForge page") installed in the */mods* directory
* Basic knowledge in **NodeJS**, **NPM** (Node Package Manager), **LUA** and obviously **Computer Craft**
* (optional but recommended) An IDE like VS Code
* A terminal
* ~~Tom Cruise~~
* A brain. It may sound like a joke but it isn't totally. Seriously, think by yourself. Even if this is a tutorial, some steps can fail for you for a reason or another. If you keep this in mind, you shouldn't have any difficulty in solving your problems. Otherwise, you can create an issue and i'll try to help you as much as I can.
* [WS](https://www.npmjs.com/package/ws, "WS NPM link")
* [ngrok](https://ngrok.com/, "Ngrok Official Website") Create an account and download it or if you're on linux, type "sudo snap install ngrok".

### Let's Get Started !

Ok so now, you should have your modded Minecraft working.
Let's open our terminal and type :

```
$ mkdir your_project_name
$ cd your_project_name
$ npm init -y
```

Those commands will create a new directory and initialize the repository so we can use NPM by creating a new "package.json" file.
Ok, so now, we'll need two things. The first is a starting script in your newly created "package.json".
Open it and just above the "test" line in the scripts part, add this:

```
"start": "node index.js",
```

You can close it for now.
Place in this directory the *index.js* file provided [here](https://pastebin.com/bnSCj9fy).
Type in your terminal:

```
$ npm start
```

You should see on the terminal that the server is initialized.
Good job, your server is now up and running!
But let's try to make the whole thing connect.


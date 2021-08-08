---
title: "Homie"
date: 2021-06-08T23:06:40+02:00
draft: false
---

# Introduction 

Homie is an angular application I am working on. It helps you keep track of all your home chores and is **your best friend around the house** ! 

It is simple, the list of tasks you have to do is available on the website, per machine, and once a task is done, it is marked as completed until it is time to do it again, say, in two weeks ! 

Not only is Homie a **great visual representation of your day to day chores**, but also a great reminder, **sending you a notification each time a task needs to be done.**

# Coding and design

The application is coded in Angular. My goal is to make it so simple and effective that it can be used everyday by people who know nothing about code but want to reap the benefits of a digital companion which can keep track of everything for them ! 

Thus, the application is separated into different parts, which I will explain one by one in what follows: 

## First, the home screen 

The **home screen** (well named XD) is an introductory screen to, first, give a glimpse of the aplication and its use cases, but also show notifications and to dos once sign in functionality is added and user is signed in ! 

For now it looks like this, but I have plans for it:

![Home screen](/blog/homie/homeScreen.png)

## Second, the appliances screen


This part of the application shows the appliances the person logged in has in their house. If one of the icons is red, then work has to be done for this particular appliance, else all of its tasks have been done. Once you do a task, you press the done button which changes the icon's color to green. Magic ! 

Once the task is ready to be done again, the icon will be automatically be reshown in red. No need to carry it inside your head ! 

Lastly, *time left* shows how much time is left until the task has to be done again, which lets you plan if you want to. But don't worry, once the time is up, you will be automatically notified !

For reference, please have a look at the photos below: 

Task is not done:
![Task Not Done](/blog/homie/taskNotDone.png)

Task is done:
![Task Done](/blog/homie/taskDone.png)

## Last but not least, the appliance page 

Every appliance in the future will have its own page. To enter the page specific to the machine you want to look at, just click on the icon of the machine in the appliances screen !

Once there will be more than one task for each appliance, the done button, and timer for each task, will move into this page, and the icon on the appliances page will turn green if and only if all the tasks for the appliance have been done ! 

For now, it does not look like much ;)

### Sneak peek  
![Machine Page](/blog/homie/machinePage.png)

# Future work and progress

In the following weeks, I will be working on this application so it reaches the best version I have to offer you. 

All future progress and features will be posted on my blog, so stay tuned for future fixes and releases ! 

# Link to the git repository 

Click on this [link !](https://github.com/hadi-el-hajj/homie)

# Test the application

To test, you can click [here](https://hadi-el-hajj.github.io/homie/)

# News 

[Part two](/blog/posts/homie_2) is here, check it out !




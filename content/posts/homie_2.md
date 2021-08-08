---
title: "Homie - 2"
date: 2021-08-08T13:55:01+02:00
draft: false
---

# Introduction

This is the second part of my blog series on Homie, an application I am building. For the first part, go to [part one](/blog/posts/homie) !

In this post, I intend to give you a glimpse of the progress I was able to make on the application, style-wise, but also feature-wise. 

Alike the first part, I will go through the different parts of the application, and display them one by one while explaining what upgrades were made to them. 

## Home screen

First of all, as you may recall, the Home screen was not that stylish and had only one button, which said "Start now". 

This made for a rather basic screen which did its work, but had to be upgraded ! 

For this, I eventually added two buttons, one which leads you to the notifications page, which I will talk more about later on, as well as a reset application button, which cleans the application's history and sets you up with a clean canvas ! All your old notifications, gone. Everything is reset ! 

On the other hand, the style of the page changed, for you can now see a navigation bar on top to ease the switching between the different components of the app, and give it a greater feel ! Also, the page is now centered so it feels symmetrical and well put together. 

So, without further due, here is your new home screen ! 
![home screen](/blog/Homie_2/home_screen.png)

## The appliances screen 

No big modifications were made on this component, except for the centering of visual elements, similar to what has been done for the Home Screen, but also the addition of **new appliances** as promised: you now have a dish-washing machine and a fridge. 

The machines have different running times (You can test that by clicking on done for each one and comparing) and different things to do once the time is done, as you will see on the new notifications panel, which I will talk about in a minute.

You may realize the timers vanished from the page, but don't worry, they are coming back in future versions ! 

The new appliances screen ! 
![appliances screen](/blog/Homie_2/appliances_screen.png) 

## The appliance page 

The appliance page has not changed, but later updates are coming, as you will read in the future work section of this post ! 

For now, it looks like this: 
![appliance page](/blog/Homie_2/appliance_page.png)

## Last but not least, the new notifications page !!! 

This component is absolutely new and enables a new feature in the application, which is to receive notifications once a task is done ! 

I am very excited about it, as it makes it possible to work with the application without having to look at the times or the status of the machine on the appliances screen, thus, getting us closer to a fully working **digital nagging mother**, that follows you everywhere !

The notifications are sent sequentially, in the order they were emitted, and they each denote a task to do, as well as the time they were emitted at ! 

For now, they are only sent on the notifications page, but later versions may send the notification to your phone or your email. Mom is coming after you !! 

**Sneak peek**
![notifications panel](/blog/Homie_2/notifications_screen.png)

# Functional upgrade 

This part discusses not a visual upgradde, nor a componenet addition, bu rather a functionality upgrade. 

In the first version of the application, its state was not saved upon quitting, which caused the timers of the tasks, the machines' running status as well as the notifications, to be reset when the user comes back, succesfully losing all his past usage of the application and progress. 

In this version, I made use of the local storage to save the state of each component upon quitting, which would be loaded again when the users comes back. 
Typically, if you have notifications upon quitting, you will still have them upon coming back, but you may also have new ones if you've left a machine running, and the task was done running while you were away. 

**This is a very important upgrade, since the application is not usable if it resets each time the user quits.**

Finally, this explains the presence of the reset button on the Home screen, which is thus used to erase the local storage and reset the state of the application. Notifications are erased, and all the machines are stopped and reset ! 

**For example :**

Before reset: 
![notifications panel](/blog/Homie_2/notifications_screen.png)

After reset:
![notifications panel](/blog/Homie_2/notifications_screen_empty.png)

# Future work and progress

In the upcoming weeks, some upgrades will be coming:
- A sneak peek of your notifications on the Home Screen, else if you have none, a welcoming text with a small tutorial, to make for a more welcoming screen.
- The possibility to choose from a list of appliances the ones you have at home so the application can adapt and show only what is necessary.
- New appliances and tasks, with a richer and more stylish appliances screen ! 
- Bring back the timer on the appliances screen. 
- In the appliance page, a list of the tasks for this specific appliance. 
- Send notifications by email or to your phone ! 
- Work on the mobile render of the application 

These upgrades may not come at once, but sequentially. Stay tuned for future posts !! 

# Link to the git repository 

Click on this [link !](https://github.com/hadi-el-hajj/homie)

# Test the application

To test, you can click [here](https://hadi-el-hajj.github.io/homie/)









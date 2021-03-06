---
title: "Unity Roll a Ball Implementation"
date: 2021-03-06T01:03:10+01:00
draft: false
---

This post describes briefly how I implemented Roll a Ball in Unity, what difficulties I faced as a beginner and how I overcame them. Additionally in the end you can find some captures I took of the Unity screen and the game screen. 

## What is Rall a Ball ? 
Roll a Ball is a minigame where the player controls a small ball and has to roll it to collect the most *collectibles* possible (which can take any form possible), hence the name. The player is, of course, bound in a space so he could not roll the ball outside the playing field. The player can move in any direction he wishes to.

![Roll a Ball](/blog/rollaBall.jpg)

That's it, it is simple game, but is a great way to start learning about the Unity environment (as a developer). By going through the process of implementing the game, I learned a lot about how objects, assets, etc. were coordinated in the Unity environment ! **It is a great way to start that I recommend.** 

## References that helped me with the implementation
- My classe's Tutorial Slide Deck 
- Unity's tutorial available at **https://learn.unity.com/tutorial/setting-up-the-game?uv=2019.4&projectId=5f158f1bedbc2a0020e51f0d** 
- Unity's YouTube Channel

Following through with the tutorials in these references, it was fairly easy to implement the game, but I ran nonetheless into some challenges I will describe next. 

## Difficulties 
All steps were easy until when I had to duplicate the collectibles. It was not hard creating the collectibles, but rather 
moving them around the scene to place them right (my choice was to place them in a circle). There was a little catch. I had to change the Toggle Tool - Gizmo - Handle Rotation to Global (from local), so the
object moves as I wish (parallel to the ground) when looking at it through the Y-Axis. I found this catch through Unity's 
tutorial videos on youtube, specifically: https://www.youtube.com/watch?v=HlDGSStxuHI

No problems afterwards for scene reproduction. 

Then came the time to build, run and test the game. 
The game built fine but I observed no movement when keys were pressed, as if the key press events were not taken into account.
To resolve the problem, I had to recreate a new input actions file after writing the scripts, so the play button would appear on its icon (which was not apparent before for one reason or another) (see figure below). 
<img src="/blog/inputAction.png" alt="Input Action File" height="100" width="20" />

All worked fine after this last step and I was able to run and play the game ! 

## Screen Captures
![Capture 1](/blog/rollaballcaptures/Unity1.png)
![Capture 2](/blog/rollaballcaptures/Unity2.png)
![Capture 3](/blog/rollaballcaptures/Unity3.png)
![Capture 4](/blog/rollaballcaptures/Unity4.png)
![Capture 5](/blog/rollaballcaptures/Unity5.png)
![Capture 6](/blog/rollaballcaptures/Unity6.png)







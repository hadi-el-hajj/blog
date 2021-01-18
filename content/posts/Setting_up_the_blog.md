---
title: "Setting up my Blog"
date: 2021-01-18T15:32:37+01:00
draft: false
---

## Installing Hugo ! 

Installing Hugo was not hard since I was using Linux. This said, I did encounter some difficulties with version updates. I wanted at first to use **Introduction**, but the theme needed higher versions of HUgo. After figuring out how to upgrade the distribution I had (see images below of the problem as mentioned on Stack Overflow) (a simple sudo apt... did not work, installing hugo through Ubuntu Software neither) and getting *Introduction* to build, I had another issue which is cited on the theme's Github page, but I was already a bit off the theme and just wanted to choose a new one at this stage. Finally, I chose **Console**, which was showcased during the Lab session. 

![HUgo update problem](/blog/Problem.png)

After choosing the Theme, came the time to create a GitHub account and learn to use Git (I knew a little at the time but learned much more throughout my Pages webpage setup). 

## Deploying 

**Setting up Pages** took me a while. In fact, I had to reorganize my blog's directories well and redo the commits, since I had duplicate docs folders at times and the *Pages* build failed many times because of that. BUt once my docs folder was well set up, it worked. 

## Adding Images

After this, all wemt smooth until I had to add **Images** to my posts. In fact, they would never show up and instead were always replaced by the alternate text. After detailed inspection of what was going on, it became clear to me that since my base URL was **https://hadi-el-hajj.github.io/blog**, my images' path had to be **/blog/image.jpg** instead of **/image.jpeg** only (pictures were stored in the static folder). 

After this was fixed, all went well ! 







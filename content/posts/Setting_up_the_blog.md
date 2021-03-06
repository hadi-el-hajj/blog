---
title: "Setting up my Blog"
date: 2021-01-18T15:32:37+01:00
draft: false
---

## Installing Hugo ! 

Installing Hugo was not hard since I was using Linux. This said, I did encounter some difficulties with version updates. I wanted at first to use **Introduction**, but the theme needed higher versions of HUgo. After figuring out how to upgrade the distribution I had (see images below of the problem as mentioned on Stack Overflow) (a simple sudo apt... did not work, installing hugo through Ubuntu Software neither) and getting *Introduction* to build, I had another issue which is cited on the theme's Github page, but I was already a bit off the theme and just wanted to choose a new one at this stage. Finally, I chose **Console**, which was showcased during the Lab session. 

![HUgo update problem](/blog/Problem.png)

After choosing the Theme, came the time to create a GitHub account and learn to use Git (I knew a little at the time but learned much more throughout my GitHub Pages webpage setup). 

## Deploying 

**Setting up Pages** took me a while. In fact, I had to reorganize my blog's directories well and redo the commits, since I had duplicate docs folders at times and the *Pages* build failed many times because of that. (The GitHub Pages builder needs to fetch your page's data through a ell defined **docs** directory, so having duplicates was not great). But once my docs folder was well set up, it worked. 

## Adding Images

After this, all wemt smooth until I had to add **Images** to my posts. In fact, they would never show up and instead were always replaced by the alternate text. After detailed inspection of what was going on, it became clear to me that since my base URL was **https://hadi-el-hajj.github.io/blog**, my images' path had to be **/blog/image.jpg** instead of **/image.jpeg** only (pictures were stored in the static folder). 

## Navigation Buttons
Following the addition of images to my posts, it was now time to see if my blog was fully operational, i.e. that all my posts can be accessed and reviewed. Clicking on the posts button on the top right of my blog, I quickly realized it did not work the way I thought it did, and that further investigation was due. 

Looking into the example site provided with the theme, it turns out a modification to the config.toml file had to be done (see picture below). The whole params section had to be added in order for the navigation buttons to be configered (navigation buttons being the buttons on the top right of your page - for the console theme).

![Configuration file](/blog/configToml.png)

**This out the way, a very important notice I would have to someone setting up a Hugo website is DO REALLY CHECK HOW THE EXAMPLE SITE IS CONFIGURED AND PUT TOGETHER, AND FOLLOW WHAT HAS BEEN DONE THERE FROM THE GET GO. The example site's purpose is guiding you to easily follow the lead. Look well into the structure of the folder before starting. I resolved many issues by doing this, like showing the images in the images panel, resolving navigation buttons issues, etc** 

After this was fixed, all went well ! 







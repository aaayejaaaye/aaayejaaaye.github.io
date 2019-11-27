---
layout: post
title: "How I Created My Blog For Free Using Jekyll and GitHub"
categories:
author: "AJ"
image: \pictures\
excerpt_separator:  <!--more-->
---
---

<img src="\pictures\how I Created My Blog\HowFreeBanner.png" style="margin-left:auto; margin-right:auto; display:block;">

Hi Techies, So I've been playing around with Jekyll for about a month trying to get this blog running. This tutorial is for those with basic understanding of HTML, CSS, CMD, IDE's, etc. Of course I will not discourage someone without any experience to not try this. If you want this to be easy and seamless then head over to WordPress, Wix, or whatever and give them your money. No shade, seriously. If you have the basic skills, and time, you can create a blog on the cheap! I'm not big into web design or development, but that just kind of is the way things are going and being able to create a website is a useful skill set for anybody trying to put themselves out there.
<!--more-->

If you are here for the first time, Hi, I'm AJ. I am a CS Major at CU Boulder and I have interest in AR/VR/Game Dev subjects. This Blog is dedicated to highlighting things I've Learned, tutorials and other cool stuff I like.

What are We going to Learn Today!
We are going to use [Jekyll](https://jekyllrb.com/), a static site creator, and [GitHub](https://github.com/), a software hosting platform.
I am also using a Jekyll Theme: [Minima](https://github.com/jekyll/minima), which is the default theme, but I have altered it to make it my own. If you would like to see more about how I designed this blog click [here](How-Designed-My-Jekyll-Blog.html).


**What will you Need:**

GitHub Account

Command Line Prompt

Domain Name (Optional)

W3 schools

JEKYLL documentation

Atom (or any text editor/IDE of your choice)


**Installation of Jekyll:**

There is a lot of great Documentation on how to install Jekyll on your device. Head on over to the [Jekyll Docs](https://jekyllrb.com/docs/installation/) and that should get you squared away. Since I am on Windows I followed the instructions [here](https://jekyllrb.com/docs/installation/windows/).

Next, we are going to head over to GitHub page for the [Minima Theme](https://github.com/jekyll/minima)
Make sure you are logged in and click the 'Fork' button on the top right of the page.

<img src="\pictures\how I Created My Blog\installjekyll2.png">

This will create this repo under your name. Go to your profile and click on this repo.
There are several ways to go about this but rename your repository to username.github.io in order for git to recognize this repository as your hosted website. For instance, mine is [aaayejaaaye.github.io](https://aaayejaaaye.github.io/) @https://aaayejaaaye.github.io/.
I recommend going to the documentation for [GitHub Pages](https://pages.github.com/) and checking that out to see more on how this works, including documentation on Jekyll implementation.
Now we are going to open this new repo folder in Atom.
Go to file > open Folder and select the 'minima' folder.
Make note of the file structure:

<img src="\pictures\how I Created My Blog\installjekyll3.png">

Save the project and go to your cmd prompt and navigate to the minima folder. See how atom and cmd match:

<img src="\pictures\how I Created My Blog\installjekyll4.png">

Again, this took me a month. Don't feel like you have to do this all at once, in fact DON'T! Follow these simple tricks, learn some more through hours of tutorials, and keep doing Google searches. In the meantime, save your work and don't forget to push to GitHub.

***Push to GitHub***

Here are the basic git commands to update your site:

```
git add .
```

adds all your changes in all your files

```
git commit -m "Some message about the changes you made"
```
```
git push
```
or
```
git push origin master
```
alright so now if you go to the https://username.github.io site you should see the default Jekyll theme on your site! Congrats!

Save often, google often. Thanks for hanging out with me!

If you want to see more about how I adjusted the design, check out my post [How I Designed My Jekyll Blog From Minima](How-Designed-My-Jekyll-Blog.html)

**BONUS ROUND: Domain Name for $12**

You may have noticed my URL is not the standard .io extension. That is because I got a custom domain name. I purchased/registered my domain name aaayejaaaye.com for $12 at [google domains](https://domains.google/). It just adds that extra touch of validity.

***Adding your Google domain to Jekyll***

So now that we are feeling valid, it's time to make sure that whoever comes across this site is seeing a real nice, custom domain. In the root of your Project in Atom, create a file called 'CNAME'. no extension needed. and inside that file put the url you have registered with google. push these changes up into to repository.
Back in your GitHub repository go to Settings and make sure under Custom domain you see your url.

Check "Enforce HTTPS".

<img src="\pictures\how I Created My Blog\installjekyll014.png">

Now we are going to go to look at [this page](https://help.github.com/en/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain)

Did you look? Good.
Head over to Google Domains and click the DNS tab.
(note: if you have forwarding or another URL occupying this URL it wont work)
Go down to custom resource records and put in the IP addresses from the above pages. for me these were:

<img src="\pictures\how I Created My Blog\installjekyll015.png">

Then you are all set!
It may take a day for the site to appear at this URL, but for me it took about an hour! Your are now not only hosting a website but also using a custom domain name. Can you feel the validation! Now go get posting!

---


 **Alrighty!**

 So there is the quick and dirty basics of how I hosted my customized my blog for free!

 Thank you for checking it out! Here is my cool moto Jacket:

 <img src="\pictures\busme.jpg" width="241" height="224">

 Deuces

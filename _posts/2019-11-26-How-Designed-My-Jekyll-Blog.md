---
layout: post
title: "How I Designed My Jekyll Blog From the Minima Theme"
categories:
author: "AJ"
image: \pictures\
excerpt_separator:  <!--more-->
---
---

<img src="\pictures\how I Created My Blog\How I Easily Edited My Jekyll Minima Theme.png" style="margin-left:auto; margin-right:auto; display:block;">

Hello welcome to the Design portion of my blogging adventure! I want to use this blog to get my projects and ideas out there. I am not trying to be a web designer or full stack developer, so spending a lot of time getting this perfect wasn't a priority. Yet, I still found the default Minima theme to be... not my style. I initially was over ambitious with my design, too many ideas. I had a eureka moment working on the design. I thought, 'Keep It Simple Stupid'. I needed to just stick to the basics and work my way up. <!--more-->

<img src="\pictures\how I Created My Blog\tenor.gif" style="margin-left:auto; margin-right:auto; display:block;">

This tutorial is for those with Basic understanding of HTML, CSS, CMD, IDE's, etc. It is also a continuation of my post [How to create a Jekyll Blog](How-I-Created-My-Blog-For-Free-Using-Jekyll-and-Github.html). Of course I will not discourage someone with out any experience to not try this, I'm just gonna say, If you want this to be easy and seamless then head over to WordPress, Wix, or whatever and give them your money. No shade, seriously. If you have the basic skills, and time, you can create a blog on the cheap!

Make sure you have your Jekyll minima theme installed and have the project open in your text editor.

**Design Stuff:**
So you've opened your project in your text editor and have a batch going on localhost:4000, now what?
On The [Minima Theme Page](https://github.com/jekyll/minima) and the [Jekyll Site](https://jekyllrb.com/docs/step-by-step/01-setup/) they explain really well just what all you are looking at. There are also some great [YouTube Tutorials](https://www.youtube.com/watch?v=iWowJBRMtpc&t=442s). I'm going to focus more on the extras like MD formatting CSS, HTML, and creating custom files.
First thing edit your \_config.yml file.
You will see a lot of presets, go ahead and fill those in. Here are my relevant Presets:

 <img src="\pictures\how I Created My Blog\installjekyll7.png">

 Save the changes and go back to your cmd prompt to reset the batch:
 ```
jekyll serve
 ```
Go to local host you should see that the changes to the title of the page have been made! FUN!

Next we are Going to Edit the About Me Page

In the root of your directory you should see a about.html. This is what we are going to edit. By default it includes a lot of helpful links, so I recommend checking them out before deleting them. You will see some elements in between \--- lines. This is called [front matter](https://jekyllrb.com/docs/front-matter/) which we will get into later. I updated, saved and gone to localhost:4000/about/

<img src="\pictures\how I Created My Blog\installjekyll8.png">

If you want to add a picture you can use the HTML \<img> tag.

I first in root created a directory named \_pictures and the "\_" lets Jekyll know that this folder is included in the \_site

Now I am going to show you the about.html page for aaayejaaaye blog.

<img src="\pictures\how I Created My Blog\installjekyll9.png">

Basically this is my current file structure and if you navigate to my About page [this](/About) is what the md file for the page looks like. I've inserted my image using an HTML tag and the rest is writing in pretty plane English.

***Front matter***

You can see above in the front matter you can see I have a layout variable If you go to the \_layouts folder you will see post.html. I like to think of the layout variable as a wrapper for how everything assigned to this variable, in this instance "post".
Next you see the title variable. I feel like this is pretty self explanatory.
Then you have the permalink variable, this lets Jekyll know what page to navigate to inside the directory.

***CSS***

Now we wanna edit some CSS styles of the blog. The first thing I did was change colors of the text. I navigated to the localhost:4000, once there I right clicked and chose inspect.
This will help guide you too the CSS elements you want to change.
<img src="\pictures\how I Created My Blog\installjekyll010.png">

As you scroll over the element it will highlight which section is covers. I'm going to get specific enough so that I only have the site tile highlighted. This is what I see:

<img src="\pictures\how I Created My Blog\installjekyll011.png">

Under the styles tab to the right in the .site-title, .site-vistied box we see the file and the line we need to go to. Change that element. In this case in the css file: layout.css:26. Back in Atom I will go to \sass > minima > \_layout.css > line 26 aka .site-title{} and insert color: #99ff33; like so:

  ```
  .site-title {
    @include relative-font-size(1.625);
    font-weight: 300;
    letter-spacing: -1px;
    margin-bottom: 0;
    float: left;
    color: #99ff33;
    @include media-query($on-palm) {
      padding-right: 45px;
    }

  &,
  &:visited {
    color: #99ff33;
  }
}
  ```
Now the title is lime green.
I Continued to do this for my site-nav, post-headings, and post-links.


***Creating a Banner***

You also may have seen the \_includes folder, read up on it [here](https://jekyllrb.com/docs/includes/). I wanted to have my own logo up instead of just my default name. Head to header.html. Using simple 'a' and 'img' tags I included my banner which I saved to my \_picture folder.


<img src="\pictures\how I Created My Blog\installjekyll012.png">

My custom code is the \<a> tag to create the link and in between that I have the \<img> that is the link to my Logo. I also did I similar thing to footer.html to include my logo in there.
BTW, I created all my Logos with [Canva](https://www.canva.com/), I love it!

Now I have my logo in my header and footer:

<img src="\pictures\how I Created My Blog\installjekyll016.png"><img src="\pictures\how I Created My Blog\installjekyll017.png">


***Preivew Blog on Main Page***

You may have noticed that I have a little exceprt on the main page for each blog post, this is by design. I use a excerpt_separator variable and the  \<!--more-->
lets it no where the excerpt ends, observe:

<img src="\pictures\how I Created My Blog\installjekyll013.png">

Once you have previewed your changes enough and feel happy. Go ahead and commit them to the remote repository.

***Push to GitHub***

Again, this took me a month. Dont feel like you have to do this all at once, in fact DON'T! Follow these simple tricks learn, some more through hours of tutorials and google searches. in the mean time save your work and dont forget to push to git GitHub. here are the basic git commands to update your site:
```
git add .
```

Adds all your changes in all your files

```
git commit -m "Some message about the changes you made"
```
```
git push
```
Or
```
git push origin master
```
Save often, google often. Thanks for hanging out with me! Time to get posting!

---

Peace,

<img src="\pictures\Annotation 2019-11-16 224810.png" width="222" height="434">

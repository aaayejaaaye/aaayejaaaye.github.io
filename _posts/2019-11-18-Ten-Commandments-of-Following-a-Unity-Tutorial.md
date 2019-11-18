---
layout: post
title: "Ten Commandments For Following a Unity Tutorial"
categories:
author: "AJ"
image: \pictures\scroll.jpg
excerpt_separator:  <!--more-->
---
---
Follow these tips or

<img src="\pictures\tencommandments\badtime (2).jpg" style="margin-left:auto; margin-right:auto; display:block;">

Ah Yes, Unity, Throughout the years of being an aspiring game developer/CS graduate /billionaire /philanthropist(ehehe) I have followed hundreds of Unity tutorials. I would consider myself an intermediate beginner as a Unity user. I find that I can still find some real quality intro Unity tutorials that I can benefit from(usually not free tho). If you look up Unity 3D/Game Development or any other popular keywords for aspiring game makers in an analytics tool you will see that the results are both highly sought after and also... highly saturated (I'm a small fish in a big pond).<!--more--> So mulling through these results and finding the right tutorial that wont waste your time is essential in the beginning stages of you game making journey. Having said that, I have learned a few things about the DO’s and DONT’S of trying to follow along. If you are looking for some basic Unity tutorials check out my [Best Unity Tutorials for Beginners in 2019]({% post_url _post/2019-11-14-Best-Unity-Tutorials-For-Beginners-2019 %})  So without further ado, Here are the 10 Commandments for beginners following a Unity tutorial online:

<!--<img src="\pictures\scroll.jpg" width="400" height="350" style="margin-left:auto; margin-right:auto; display:block;">-->

1. Thou Shalt Break Everything
2. Thou Shalt Observe the Unity version Number
3. Thou Shalt name the scripts to match the project and in the IDE
4. Thou Shalt Learn the Editor Before Learning the Scripting
5. Thou Shalt google endless until a fix is found to a console Error
6. Thou Shalt utilize forums and documentation
7. Thou Shalt Use the Search API feature in VS
8. Thou Shalt Align Empty Game objects with origin
9. Thou Shalt Always double check the configurations and the player settings
10. Thou Shalt have Patience


**1. Thou Shalt Break Everything**

You have to accept when following an online tutorial that it is not going to go perfectly. this may be redundant from the intro but if you didn't read it then you are getting it here. It is a rare occasion that I follow a tutorial online and it works perfectly according to plan. This is so rare. you have to accept that if you try a tutorial there are going to be inconsistencies. You will inevitably need to google a work around to be able to get through a tutorial. It is also almost as likely, if you are following a video, that you will miss a step and that may cause problems. Just be consistent and work through those problems and you will learn more than you would have if you just followed the tutorial as is.  

**2. Thou Shalt Observe the Unity version Number**
As a beginner you may not realize that Unity Projects are not backwards compatible and that the layout/configurations and capabilities of Unity projects vary greatly between major version releases. If you are opening a Unity project that was created and save as a different version, a notification will appear and warn you that this could be troublesome. I would say for official Unity tutorials this may not be a problem but there are a lot of tutorials out there that are extremely dated and will be hard to follow if you don't already understand Unity essentials.

In these two pictures you can see that I am currently using Unity 2019.2.0f1.
Major releases are a new year ex. 2017.x.x or 2018.x.x


There are two ways to check which Unity version you own(and you may own several) one way is in the Unity Hub under Installs:
<img src="\pictures\tencommandments\unityversion.png">


The other is once you have opened a Unity Project in the top left corner:
<img src="\pictures\tencommandments\inituversion2.png">

*tip: if you don't see and explicit 20xx.x.x version than the tutorial is in a much older version(usually unity 5>) as  a newbie it might be best to avoid these older ones)*

Its the tutorials the have a major release differences from your own version that you want to avoid.


*tip (Import the Project as assets or as a unity package)*


**3. Thou Shalt name the scripts to match the project and in the IDE**

<img src="\pictures\tencommandments\cantaddscript.png">
One sort of trivial mistake I made when I was first starting with scripting in Unity was learning to understand the relationship between Unity and Visual Studio. I very Common mistake is Remnaming a class in visual studio only to realize back in the editor the console is throwing an error about my scripts.

<img src="\pictures\tencommandments\Inkedsampleerror_LI.jpg">

Observe. In the upper left the name of the class does not match the class name in the actual script. Thy have to match or your going to have a bad time.

**4. Thou Shalt Learn the Editor Before Learning the Scripting**

Have you checked out my [Best Unity Tutorials for Beginners in 2019]({% post_url _post/2019-11-14-Best-Unity-Tutorials-For-Beginners-2019 %}) if you have right after your read this go that that. I mention in that post the importance of understanding the Unity Editor before trying to get to involved in other aspects of working in Unity. You can do it the easier way, or you can do it the hard way.


**5. Thou Shalt google endless until a fix is found to a console Error**

Those console errors suck. Fortunately a lot of them are common and easy to find answers too. The fastest easiest way to research an error is to copy the exact error output from the console and search it verbatim on the web. Stack Overflow and Unity forum usually the results needed to resolve most issues.


**6. Thou Shalt utilize forums and documentation**

<img src="\pictures\tencommandments\documentation_matrix.jpg" style="margin-left:auto; margin-right:auto; display:block;">

SO! SO! SO! Important, I keep hearing that as a stereotype programmers hate documentation, idk maybe, but this is so important to utilize forums and documentation so that not only do you get things working the way you want, but that also, when it inevitably breaks, you can understand enough of what going on to be able to fix it.



**7. Thou Shalt Use the Search API feature in VS**

This blew my mind. In visual studio if you are looking over some code and you see a method that you cant quite remember what it does you can highlight the reference below I have 'List' as an example. Go to Help > Unity API Reference.

<img src="\pictures\tencommandments\unityapiVS.png">

and I will open up the Unity Scripting API web page in your IDE(it even has a hot key combo!!!)

<img src="\pictures\tencommandments\unityapiVS2.png">


**8. Thou Shalt Align Empty Game objects with origin**

When creating a empty game object, in the inspector window you will see the transforms. Unless their is a specific reason to have the transform be anything other than (0,0,0) then I say make sure to always reset the transform to make sure that their are no issues in the future with any children of the game object.


<img src="\pictures\tencommandments\transfrom.png">

**9. Thou Shalt Utilize the Asset Store**

If you haven't checked it out, the Unity Asset store is a great resource for all things you would need in your Unity Journey. there are tons of options for free assets as well as many options for paid! you can access the access store through your unity editor, or go to <a href="https://assetstore.unity.com/">The Asset Store Here</a>


**10. Thou shalt have Patience**

Unity takes a long time to master and with perseverance and patience you will learn. It's important to try not to get to ambitious, and if you do then break down what you want to accomplish piece by piece and build up from there. It's important to not be too idealistic and try to understand when something you are trying to do is too hard. If you find a goal is too much keep reorganizing and putting each goal into smaller more realistic task. You'll get there I promise!

---

WOW! you made it this far!
Thanks for checking out my posts and sticking it out for the long haul.

<img src="\pictures\tencommandments\cheers-congratulations-meme.jpg" style="margin-left:auto; margin-right:auto; display:block;">


**-AJ**

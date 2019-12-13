---
layout: post
title: "Beginner Mistakes in Unity"
categories:
author: "AJ"


image: \pictures\
excerpt_separator:  <!--more-->
---
---
<img src="\pictures\unitymistakes\Common Mistakes Beginners Make In Unity.png" height="50%" width="50%" style="margin-left:auto; margin-right:auto; display:block;">

<h3>It is so very funny, starting in Unity is exciting and there is much to learn. After doing a tutorial or two it might be time to venture out into the wild and start working on a project you have been dreaming about all this time. I am so so soooooo happy for you. However, read this first and learn from my mistakes.
</h3> <!--more-->

<h3>Here are some mistakes I made starting out in Unity:</h3>


<h2> 1. Diving in head first</h2>

At this point this might be cliché advice. It is so important to take baby steps when learning Unity. I have tons of projects where I focus on learning just one aspect of a game. Breaking topics down into categories; ex. player movement, animation, game physics; can really prevent a project from getting overwhelming which can eventually then lead to not finishing.

<h2> 2. Improper Project Planning</h2>

I am SOOOOO guilty of this. It is really important to understand what you want to do with your project and how you plan to do it before actually starting the project( It is important to at some point actually start). Doing proper research and knowing which tools can help with streamlining a lot of work and can save you time! which bring me to my next point...

<h2> 3. Not utilizing the tools/features in the editor</h2>

Do you know the difference between using pure c# and extended monobehavior? Can you create your own prefabs? Have you utilized scriptable objects? do you know anything about animation? If you don't know what any of these things are. Then you might be overcomplicating your workflow. It might be fun to reinvent the wheel and sure you will learn a lot from doing that but for the actual implementation of your game, it best to utilize features that already exist if you can.

<h2> 4. Not using version control</h2>

If you are not using version control with your project, you are making a huge mistake. I will admit, using VC with Unity is incredibly annoying at first. Once you get the hang of it, it is very helpful. For example, say you have started a new feature on you project. It gets messy and confusing and your not sure how to sort it out so you opt to start over. If you use version control it is very easy to do that. I will be writing a tutorial on this in the future so be on the look out and be sure to sign up to my email list to be informed.

<h2> 5. Relying heavily on someone else code </h2>

I am all for copy/paste/modify as long as  you understand what is happening, like really truly understand. You will save yourself a lot of time in the long run if you do. Chances are the code will eventually break and when it does you will have to understand in order to fix it.

<h2> 6. Not comparing script name with class name</h2>

This is a very simple very common beginner mistake. Basically, when you create a script in the Unity editor you will usually give it a name. If you have opened the script in Visual Studio and then decide to rename the scripts from VS then once you return to Unity it will throw and error. So you will also need to rename the class in Unity. You would think Unity would be able to pick up on those changes but it doesn't. Simple mistake, simple solution.


<h2> 7. Terrible project inconsistencies/organization</h2>

Here is another one I am deeply guilty of. PLEASE KEEP YOUR HIERARCHY AND PROJECT FOLDERS NEAT! That means everything is properly organized and labeled accordingly. Keep your Prefabs and a Prefab folder, you scripts in a scripts folder etc. Your Hierarchy should have empty game objects with appropriate names and if you can turn and object into an instantiated prefab? please do! Obviously if none of this specific advice applies to you project the message is the same. Pick a structure, stick with it, keep it clean, readable, and organized. If you really want to be the over achiever, include a Read file that explains your structure organization choices etcetera.


<h2> 8. Taking advantage of Garbage Collections/ not utilizing efficient performance</h2>

Garbage collection, when a program runs it cleans out all the unnecessary code and clears memory space. C# does this, Java does this, most languages do. But garbage collection also takes a toll on memory usage. Just like keeping your project structure clean, you want to keep you code clean. It is also important to understand that efficient performance doesn't just apply to the code. It is also closely related to the third point of not utilizing tools and features of the Unity editor.

<h2> 9. Not understanding Meta files</h2>

Meta files, I had a huge issue with meta files for my NASA project. It was a huge lesson, I wont get into details but I will tell you what to avoid. If you are looking at a Unity project via your file explorer, you will usually see two similarly named files. ex. 'Enemies.cs' and right after 'Enemies.cs.meta' These are very important. I do not recommend deleting files in your file explorer unless you also delete the meta files. If you have done this wrong, the next time you open your project it will load improperly and essentially break. The way to fix this mistake is to touch nothing! go to your file explorer, delete Everything except the Assets folder. This should fix your problem.

<h2> 10. Not saving often enough</h2>

This one is kind of a give away but yeah... save your project, like every 10-30 mins. You really don't know what could happen especially as a beginner.

<h3>Once again, Thank you so much for reading this article I hope it is super helpful to you and best of luck!</h3>

---

I cut my hair and I love it!

<img src="\pictures\hiarcut.jpg" width="50%" height="50%">

Peace,
AJ

---
layout: post
title: "I Tried Spark AR: Beginner Friendly"
categories:
author: "AJ"
image: \pictures\basic color switcing\sparkar.png
excerpt_separator:  <!--more-->
---
---
**Spark AR Studio v75**


![Image of Me](\pictures\basic color switcing\sparkar.png)


How long has this been a thing!?(August) It's fantastic, super easy, and fun!

I was recently googling and found Spark AR show up in several of my results. At first I was reluctant because I personally don’t currently use Instagram or Facebook filters (but have been considering it). <!--more-->I thought <em>It seems simple, so let’s give it a go!</em> and I made this simple lil filter that make it look like you have a cool RGB bulb in your space that changes color whenever you tap the screen.

 <img src="\pictures\basic color switcing\giphy.gif" width="800" height="400" style="margin-left:auto; margin-right:auto; display:block;">
*it's a bit blurry because my phone camera is broken... but we cant let that stop progress!*

**First Impression**

I wanted to do some investigation. First, I looked up the documentation on the Spark AR Website. It's fabulous, thorough, and my favorite, provides sample projects with video tutorials! Next I went to YouTube and looked for content created on there: again, plenty to work with.

So I took the next step and downloaded the application and booted her up. Installation was super simple and I was able to log in with my Facebook account info, I was prompted that if I wanted to create and AR application for iPhone I would have to create an iTunes account. This is just for fun, so I'm not going to. 

**First Boot**

I opened up a sample project, Boombox with Audio, and the interface was very natural and easy to understand. Perhaps it is my experience with Photoshop and Blender, but it felt akin to those types of programs. I followed along to a few of the sample tutorials/assets and mulled over the documentation, and I felt ready to create my own Masterpieces!

<em>AJ! What Are We Going to Create Today???</em> Glad you asked!

Ok, how many of you love RGB!? ME TOO! Well, I sadly only own one cool RGB light bulb, it sits near my desk and I use it when the sun is down (any darkness lovers?) I love the purply, pinky, blue tones best but would love to experiment with what it would look like if I had more RGB, like a whole apartment of RGB *(twinkling eyes)* LET'S GO! So this is pretty basic. We will get more into it in a later post, but for now we will make this very non-intimidating and simple. 

**What you’ll need**

Smartphone

USB Connector 

Spark AR player app

Spark AR Studio

Webcam

**Setting the Scene**

* Go ahead and create a new project. I named mine SparkRGB.
* First we are going to create a canvas and a rectangle in the scene view. It needs to be a child of the focal Distance so that it is in view of the camera. 
* Right click Focal Distance > Canvas
* Right click Canvas > Rectangle
* Rename the rectangle to rgb_env

![Image of scene](\pictures\basic color switcing\basic final_scene.png)

* Now in the rgb_env inspector you should see the Materials drop down menu. Hit the + symbol to create a new material. 

![Image of rgb_env](\pictures\basic color switcing\basic final_rgb_env.png)

* Under the Assets menu you should see a new material0 appear. Rename it to background_mat.
* We want to add a texture to our new material. Click on the camera object in the scene view and hit the + under Texture Extraction this will create a texture from what the camera is capturing. You should see cameraTexture0 appear in the textures folder under Assets.

![Image of Camera](\pictures\basic color switcing\basic final_camera.png)

* Click back on our background_mat and under Shader Properties > Diffuse. Click the arrow next to Texture.

![Image of background_mat](\pictures\basic color switcing\basic final_backgroundmat.png)

* The Patch Editor should open, and now we are ready for some simple logic.

**The Patch Editor**

* The Patch Editor is a tool Spark AR is implementing to make Spark AR more accessible to non-programmer types. You should see a background_mat box in our patch editor view.
* So in order for the scene to change color, we are going to create a screen tap event. Right click in the patch editor and search for Screen Tap and insert it into the editor. Screen tap registers when the user touches anywhere on the screen.
* We want our tap event to circle through a series of colors, so for that we want to use a counter patch. Right click and search for counter and add it to the editor. 
* We need some values for our counter to loop through so we are going to create and Option Picker. This patch is nice because you can choose a value that is being picked. It can be colors, vectors, animations etc. We are going to add then select our option picker and make sure that data type is color. You can choose whichever colors you like. Combined with counter you can increase or decrease the number of color options.
* Finally, we are going to connect all the patches. I have the final connectivity here:

![Image of final Scene](\pictures\basic color switcing\basic final_patch.png)


**Preview**

To View in App:

So now we are going to select the camera icon and choose the integrated camera option. You should now see yourself in the preview. On the camera preview box select the drop down and hit simulate touch, and begin selecting the screen. You should see the colors changing each time! YAY!

To View on Phone:

Download the Spark AR Player app and then connect your device to your computer via USB. In the bottom left there is a phone icon. Select it and you should see your device listed. Hit send and the app will appear on your phone! Voila! You now have an RGB Room!

Final Project in App:

I really look forward to digging in deeper with this in the future! Anywho... See you next time!

---

-AJ


![](\pictures\basic color switcing\giphy (1).gif)

silly faces not necessary...

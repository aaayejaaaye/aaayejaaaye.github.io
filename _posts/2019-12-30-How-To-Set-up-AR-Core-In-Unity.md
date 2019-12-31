---
layout: post
title: "How to Setup AR Core in Unity"
categories:
author: "AJ"
image: \pictures\
excerpt_separator:  <!--more-->
---
---

<img src="\pictures\arCore\ARCore-logo-_3_.jpg" style="margin-left:auto; margin-right:auto; display:block;">
**Hello Hello,**

If you are on the internet looking for a tutorial on ARCore or AR Foundation you might be receiving mixed information on the configurations. Never fear, I am here to hold your hand. Don't worry I wont casually gloss over critical details. This tutorial assumes this your first time building an Android application. If you want to try the [ARCore official Instructions](https://developers.google.com/ar/develop/unity/quickstart-android) please do. I find that a combination of these plus my own knowledge of unity works best. If you plan on using the ARFoundation package for Unity you will also need to view these instructions [Quickstart for ARCore Extensions for Android.](https://developers.google.com/ar/develop/unity-arf/quickstart-android)

<!--more-->
**What You'll Need:**

Android Studio

Unity 2019.LTS with Android Build Support(we will cover this)

optional:

Google ARCore Unity Package

A compatible device with developer mode enabled and an USB cord to connect it with your computer.

Java 8 (For the AR Foundation Users)

**First Steps: Get the Android SDK**

Download [Android Studio](https://developer.android.com/studio).

<img src="\pictures\arCore\androidstudio.png" style="margin-left:auto; margin-right:auto; display:block;">

You can download all the defaults. We are really just using android studio to get the SDK.

Start up Android Studio and hit the drop down Configure > SDK Manager

<img src="\pictures\arCore\androidstudio0.png" style="margin-left:auto; margin-right:auto; display:block;">



<img src="\pictures\arCore\androidstudio1.png" style="margin-left:auto; margin-right:auto; display:block;">

The minimum required API level is Android 7.0 or level 24 so if you just want to only install that you can. I have installed 7.0 - 10.0.

Go ahead and hit 'Apply' and It will download the API's. After that has downloaded hit ok and you are done with Android Studio.

**Unity Modules and Packages**

Open Unity Hub. Under the Installs tab, hit the three dot drop down next to the version of unity you want to Install Android support for. Hit 'Add Modules'.

<img src="\pictures\arCore\unity0.png" style="margin-left:auto; margin-right:auto; display:block;">


Check the Android Build Support and make sure the SDK and NDK and OpenJDK are checked as well. This will take a while to install.

<img src="\pictures\arCore\unity1.png" style="margin-left:auto; margin-right:auto; display:block;">







**Package Manager**

Once Unity has installed the new module you are going to want to create a new 3D project. Now we are going to download some packages.
Under Window > Package Manager. It should be on the 'All' tab by default but if not, click it now.

<img src="\pictures\arCore\unity2.png" style="margin-left:auto; margin-right:auto; display:block;">

**Under Package Manager search for and install the following:**

1. Multiplayer HLAPI
2. XR Legacy Input Helper

For the ARCore SDK you have two options. [click here](https://github.com/google-ar/arcore-unity-sdk/releases) and download the google ARCore Unity package or download the ARCore XR Plugin Package from the Unity Package Manager.**Note** if your plan is to use ARFoundation stop and follow these directions aswell. [ARCore Extensions for Android.](https://developers.google.com/ar/develop/unity-arf/quickstart-android)

They are slightly different so you will have to decide which version is right for you.

If you have downloaded the Google ARCore Package. Navigate to the location of the download and click on the package with Unity open. A window will appear asking which assets you wish to install. I have all them checked. hit 'Install'.


**Configure Project Settings**

Go to File > Build Settings to open the Build Settings window.

Select Android and click Switch Platform.

In the Build Settings window, click Player Settings.

**In the Settings window, configure the following:**


Player Settings > Other Settings > Rendering	Uncheck Auto Graphics API

If Vulkan is listed under Graphics APIs, remove it.

Player Settings > Other Settings > Package Name	Create a unique app ID using a Java package name format.

For example, use com.example.helloAR

Player Settings > Other Settings > Minimum API Level	Android 7.0 'Nougat' (API Level 24) or higher

(For AR Optional apps, the Minimum API level is 14.)

Player Settings > XR Settings > ARCore Supported	Enable

In your project window you should now see ARCore, Multiplayer HLAPI, and XR Legacy Input Helper.

You should be good to go!

I highly recommend looking over the documentation they have on the [Google ARCore Page.](https://developers.google.com/ar/develop/unity)

**Deploy to Android Phone:**

In order to deploy an app live to your phone you will need an ARCore device put into developer mode with USB debugging on. Connect the device to your computer via USB.
In the Build Setting make sure you have a scene added to 'Add Open Scenes'. You can use one of the sample scenes that comes with the ARCore packages. Under 'Run Device' select your phone from the drop down. Mine is the Google Pixel.

<img src="\pictures\arCore\unity3.png" style="margin-left:auto; margin-right:auto; display:block;">

Select 'Build and Run'. A window will pop up asking where to save the build file. I always create a new folder called 'Builds' for my builds. lol.
The app should deploy to your phone and your good to go!


---
---
Thanks so much for checking out this tutorial, if you have any problems send me a message on IG and ill be sure to get back to you!
Peace,

AJ

# Destroy-on-Collision-Tutorial
tutorial one how to Destry a game object on collision

# Prerequisites
Before approaching this tutorial, you will need a current version of Unity and a code editor (such as Microsoft Visual Studio Community) installed and ready to use.

This tutorial was created with Unity 2022.3 LTS and Microsoft Visual Studio Community 2022 versions. It should work with earlier or later versions. But you should check the release notes for other versions as the Editor controls or Scripting API functions may have changed.

To proceed with this tutorial you must already have a unity project in which you should have a Player that moves Left & Right, if you do not have this i have a tutorial explainig how to make 2D Left & Right Movement from the begining, please follow that tutorial first and come back to this. 

# Objectives
In this tutorial, i will show you how to destry a gameobject on collision in unity.

# Getting Started
The first thing to do is in the hierarchy go to sprites and create a circle and name it coin, this will be the object we will be destrying, in the inspector change the color of the coin to whatever you want. Give it a `Circle Collider 2D` and set `Is Trigger` to enable by ticking it, lastly go to the top of the inspector and create a new tag called `Coin`, set your coin to this tag. Your inspector should look like this. 

<img width="453" alt="Screenshot 2025-01-05 at 02 45 19" src="https://github.com/user-attachments/assets/9bffe370-18e2-4339-8957-8c1ea1f20614" />

# Scripting 
In your scripts folder create a new script and call it `Pickup` doble click on the script and now we can start to code.

In your script editor go all the way to the bottom and start to write an on trigger enter 2d into our script and as the name suggest what this code will do is when both colliders from our player and our coin collide the following will happen, the code would check for the tag of coin and destroy any object we have overlaped with. [`OnTriggerEnter2D`](https://docs.unity3d.com/6000.0/Documentation/ScriptReference/MonoBehaviour.OnTriggerEnter2D.html) The following code should look like this.

<img width="643" alt="Screenshot 2025-01-05 at 02 55 19" src="https://github.com/user-attachments/assets/0a352f25-92bd-4b5b-9092-6c18fbc53887" />

# Finishing
Back in Unity just drag our `Pickup` script and add it to the player and we are done, press play and the coin will destroy on collision.

I got reference for this tutorial from https://www.youtube.com/shorts/r7H1hmiCdWU

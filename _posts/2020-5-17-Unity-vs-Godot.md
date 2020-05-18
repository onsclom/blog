---
layout: post
title: Unity vs Godot
---

## Quick Update

I am done with finals and have free time again! I have been using that time to learn how to use Godot. This blog post will be different than my previous ones in that it will be dedicated to comparing the two game engines. I will break down many aspects of the two engines and explain why Godot seems to be better in every category.

## Overview

Unity is earning roughly $300 million per year and while it has a basic free tier, to get all the features and to sell your games you must buy a subscription. Godot is a totally free and open source engine which runs off donations and contributors. The things discussed below are simply observations and opinions from using both engine. Some things may be inaccurate as I am not an expert, but I tried to gather the main differences between these engines.

## Languages

Godot supports C#, C++, VisualScript, and my favorite, their own language GDScript which is very similar to python. Unity supports JavaScript and C#. Python is one of my favorite languages because it is so easy and fast to transform logic into code. Because of that, GDScript has been great for me.  Most people dislike python because the lack of static typing does not allow for things like like linting, autocompletion, and type checking errors, but GDScript actually allows for optional typing that supports all of these features. GDScript can easily be picked up by any programmer and it is a great first language to learn for nonprogrammers, but its greatest strength is how it is configured for game development. Files are automatically class declarations where you start by inheriting from another class, then defin fields, and finish with defining methods. This makes code so clean and easy to read compared to C# as there is so much syntax simply starting the declaration of the class. GDScript and its integration with the editor is probably my favorite part of Godot.

## Organization

It is so easy to get lost in a sphagetti organization mess with Unity. There are gameobjects, components, scenes, and prefabs and they can all be combined in ways that make things really messy. When navigating and referencing things in your game there seems to be an endless amount of methods to consider like GameObject.GetCompont() or GameObject.Find() or Transform.Find() and it takes a nontrivial amount of time to learn it all. Godot uses a very simple organization system which is called scenes. Everything that could be a gameobject or component in Unity is a node in Godot. Scenes are just a tree of nodes. Godot’s organization system is much more concise and intuitive, yet it supports all the workflows that people in use in Unity.

## UI

Unity’s UI can be very intimidating, and even after using it for months I still was not sure what half the things on the screen did. By most standards, the UI is outdated looking. Dark theme is only available for those who buy a membership. Godot opts for a very simple and clean UI where rarely used features are tucked away until manually expanded. The game preview and other important aspects are given more screen real estate because of this. Godot allows users to customize many aspects of the editor including the colors and the whole UI is built from its own UI tools. This allows people who are proficient at using Godot to easily contribute to the open source project.

## Lightweight and Fast

With all the export packages, Unity is roughly a 10x bigger file than Godot. Since Godot is only around 1GB it can easily be stored on any flash drive or downloaded quickly. Games made with Godot tend to be much smaller and export faster. While html5 exports on Unity could take me 2-3 minutes, Godot is more like 2-3 seconds! Lastly, as a Linux user, the Unity editor runs very slow on my computer. Godot on the other hand is optimized very well for linux since that is what the main developers use. 

## Intuitiveness

While intuitiveness is hard to quantify, I can give a couple of examples. In unity, the process to use 2d lights is the following: import the LWRP package to your project, configure your project to use the new render pipeline, change all the textures in your projects to be unlit textures, and finally, 2d light gameobjects can be used in your project. In Godot, instantiate a 2d light node and it just works. In unity, the input system needs specific names for specific keys and it focuses around an unintuitive axis system. Godot has a very modern and concise input manager with input listening. Someone with no previous experience can quickly and easily set up bindings in Godot.

## Conclusion

With everything I have seen from both engines so far, Godot seems to be the better option. Switching over to Godot has been exciting and I have really enjoyed everything about it so far. This is my first technical post and I hope to do more technical posts in the future. 

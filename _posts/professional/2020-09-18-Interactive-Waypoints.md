---
layout: post
title: Interactive Waypoints
subtitle: List of interactive waypoints
tags: [Professional]
thumbnail-img: /assets/img/posts/professional/interactive_waypoints/iw.gif
comments: false
---

At some point while working for Ross Robotics I was tasked with coming up with a solution for navigating the robot along predescribed waypoints. The idea was that someone using RR robots coudl define a path for them to follow many times. While, move_base provides a nice pose-to-pose functionality, such waypoint following was not supported by default at this time.

Looking around online I've foind the [follow waypoints](http://wiki.ros.org/follow_waypoints) repository. However it had a few major shortcomings. There was no easy way to edit, save and loard the paths. And so, I've made my own [interactive waypoints](https://github.com/JuliusSustarevas/interactive_waypoints) package that actually alows the user to play with the waypoints prior to exectution. Using interactive markers, the waypoints can be moved around, their order can be changed and a move_base command send out just from a rick-click menu.

<iframe width="640" height="480" src="https://www.youtube.com/embed/TEhuI_YelVc" frameborder="0" allowfullscreen></iframe>
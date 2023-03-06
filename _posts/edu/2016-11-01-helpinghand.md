---
layout: post
title: Helping Hand
subtitle: Coursework on haptic teleoperaiton
thumbnail-img: /assets/img/helping_hand_2.jpg
cover-img: /assets/img/helping_hand_2.jpg
tags: [Edu]
comments: false
---

During my time @UCL one of the courseworks we were tasked with was to develop a rudimentary teleoperated system. The parameters of the assignment was very open ended and our only other brief was to write up a mock paper. I chose to develop a low-cost teleoperated robot arm designed to allow wheelchair users to manueuver and retrieve objects indoors.

The robot arm was modified from the "Maplin Robotic arm with USB and PC interface". The four servo motors were replaced and interfaced with a raspberry pi micrcomputer via custom built motor drivers as commercial alternative were not available. Each motor was controlled by force sensors connected to a MCP3008 ADC and interfaced with a seperate raspberry pi. Wireless communication between the raspberry pi's was set up by establising a VPN and creating a TCP/IP socket that continuously stream infromation between the pis. Additionally, a faster connection was made by creating a network via the home wireless network and establish a static IP address for each device.


<img src="/assets/img/posts/HelpingHand/15871013_10157955922495517_2042112932_n.jpg" alt="">
 
<img src="/assets/img/posts/HelpingHand/motordriver1.jpg" alt="">

A rudimentary wheeled platform was made for the robotic arm and controlled via the same four force sensors. The assignment between control of the robotic arm motors and the motors on the wheeled platform was controlled via a switch.



<iframe width="640" height="480" src="https://www.youtube.com/embed/zI3apLY_KhM" title="Helping Hand" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/zI3apLY_KhM" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

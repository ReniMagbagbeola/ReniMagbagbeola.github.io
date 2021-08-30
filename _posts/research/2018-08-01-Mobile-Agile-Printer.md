---
layout: post
title: Mobile Agile Printer
subtitle: Robot for on-site Construction
tags: [Research]
cover-img: /assets/img/posts/research/map/map1.png
thumbnail-img: /assets/img/posts/research/map/map.gif
share-img: /assets/img/posts/research/map/map1.png
comments: false
---
[Mobile Agile Printer](https://ieeexplore.ieee.org/document/8593815) was my very first paper. It is a systems intergration work  that merges my own and [Daniel Butters'](https://www.linkedin.com/in/danielbutters/) MSc projects together. The paper covers two main topics - the omni-directionality of this custom mobile base and the (lack of) deterioration of arm end-effector trajectory during base motion. The central learning here is that printing-in-motion should be feasibile as the base motion is not drastically effecting the end-effector. Here is the video acompanying the paper:

<iframe width="640" height="480" src="https://www.youtube.com/embed/ZDWArH0ajdg" title="Mobile Agile Printer" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

My side of this project mostly focussed on the development of the mobile base itself, wheel/leg/robot-level controllers and the overall robot behaviour. One of my favourite parts of the project were the number of cute control bits throughout the base-arm hierarchy. The legs would sometimes rotated in different directions based on the shorter angle difference or the robot velocity gain was made to be a function of the allignment of the four legs. 

<video autoplay="autoplay" loop="loop" width="768" height="512">  
  <source src="/assets/img/posts/research/map/map_leg_response.webm" type="video/webm">
</video>

<!-- <img src="/assets/img/posts/research/map/map1.png" alt=""> -->

The AML lab, which I was part of at the time, had future plans for the MAP robot. And so, one year later another Msc student,[Pedro Javier Rodríguez](https://www.linkedin.com/in/pedro-javier-rodr%C3%ADguez-26a287140/), under my supervision began works in implementing planned design improvements. These included changing to hoverboard-style hub motors, introducing a second mounding frame and shifting construction to aluminium extrusion. And another two years later a third MSc student, [Andras Nagy](https://www.linkedin.com/in/andras-nagy-13473b208/), finished the work.
<img src="/assets/img/posts/research/map/pedro.jpg" alt="">
<img src="/assets/img/posts/research/map/adreas.jpg" alt="">
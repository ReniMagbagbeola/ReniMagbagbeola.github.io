---
layout: post
title: ros_msgdict
subtitle: ROS messages as app parameters
tags: [Professional, Ross Robotics, ROS]
comments: false
---

I don't like large blocks of code that are often neccessary to fill a ROS message. For me, blocks like these look horrible:

```
pose_goal = geometry_msgs.msg.Pose()
pose_goal.orientation.w = 1.0
pose_goal.position.x = 0.4
pose_goal.position.y = 0.1
pose_goal.position.z = 0.4
group.set_pose_target(pose_goal)
```

Especially if all I want is a quaternion representing a zero or standard 90 degree rotation. Complex messages like moveit service requests can look even worse. So I wrote a small package that can help.

[ros_msgdict](https://github.com/JuliusSustarevas/ros_msgdict) exploits how similar dictionaries are to ros messages and helps save/load complex ros messages to/from yaml files. The block above could thus somewhere in a yaml file like this:

```
pose_goal:
dict:
    position: {x: 0.4, y: 0.1, z: 0.4}
    orientation: {x: 0., y: 0., z: 0., w: 1.}
type: geometry_msgs/Pose
```


Thus, for example, if you are writing visual marker publisher, you can parameterise more easily:

```
arrow_scale:
dict: {x: 0.3, y: 0.02, z: 0.02}
type: geometry_msgs/Vector3
control_scale:
dict: {data: 0.35}
type: std_msgs/Float32
default_mesh:
dict: {data: 'package://interactive_waypoints/res/generic_flag.stl'}
type: std_msgs/String
marker_color:
dict: {a: 0.6, b: 0.8, g: 0.8, r: 0.8}
type: std_msgs/ColorRGBA
```

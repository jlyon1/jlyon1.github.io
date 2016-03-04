---
layout: post
title: Why use computer vision in FIRST?
---

Computer vision has been an element of FRC games for many years, however, it always ends up not being utilized on our team, and many FIRST teams. This is usually due to a variety of factors, however, It should be noted, that computer vision often provides a huge advantage to teams who decide to use it. In shooting games, it allows team's to guide their shots, depending on robot design, allowing them to shoot without pausing in motion. Many teams use these vision solutions in order to guide their robots to making most of the shots they take, often times over 90% accuracy. In non shooting games, computer vision often allows teams to track non moving elements of the game, notably the yellow totes and green containers in Recycle Rush (2014-2015).

![Example of Vision Targets]({{ site.baseurl }}/images/stronghold_vision.png)

The advantages of computer vision seem fairly obvious, and often times the implementation of code to gain these advantages can be simple, however, many teams do not take advantage of the possibility of using a Vision system. FIRST clearly intends to encourage vision systems, by providing cameras, LED rings, and retro reflective tape, however, the spread notion that vision code is slow, hard to write, and often challenging for teams prevent many from even attempting to gain the benefits of computer vision. With the release of GRIP this year, teams have found it easier to apply computer vision solutions, however, many people have reported issues with the system, and by writing your own vision software, not only do you gain the experience of doing so, but you have much more control over what processing goes into the information before it is sent to the robot.

Vision code, however, does not need to be difficult, our team has struggled with this perception for a few years, fears of slowed robot computation cycles, fears of latancy over the network, and issues with robot functionality caused our team to decide to not use a functioning vision system in previous years.

This year our vision system is written in Java, using [OpenCV 3.0.0](http://opencv.org/downloads.html), an [Axis M1011 camera](http://www.axis.com/us/en/products/axis-m1011), and two green LED rings. The [system](https://github.com/jlyon1/StrongholdVision) looks at only the green channel of the image, and minimal processing has to be done in order to track the targets, giving us information about the angle to the target, as well as the distance away. 

An example of some shots taken by our robot using this system can be seen here: (www.youtube.com)

In order to help remove the barrier to a vision system, I will be posting a full writeup and tutorial of this vision system and posting it here in the coming weeks. 

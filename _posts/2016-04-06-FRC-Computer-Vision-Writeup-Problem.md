---
layout: post
title: Team 3044 Stronghold Vision Part 1
---

In our analysis of the game FIRST Stronghold, our team decided that vision tracking of the targets was not only a "Nice to have" Feature, but was a design requirement. Once this was decided, I took on the task of developing a reliable system which we could use in this year's game. We decided on three requirements for our system, which had to do the following in real time: 

* Reliably Locate the position of the targets
* interpret the information
* send the results to the robot.

Our vision software was written in Java, using the Opencv libary, and ran on our driverstation laptop. The software used the following basic procedure: 

1. Aquire the image from the axis camera
2. Convert the image to HSV
3. Threshold the image
4. Draw contours around all areas that met the threshold
5. Use other information to determine what "Blobs" were likley targets
6. Use the smart dashboard libary to communicate the most probable target to the robot.

## Configure OpenCV 3.0.0

## Aquire Images from Axis Camera
Our team used an [Axis M1011 camera](http://www.axis.com/us/en/products/axis-m1011) with two LED rings around the lens for image aquisition. The camera was directly plugged into the radio using the ethernet port on the camera. This setup gave us some illumination on our targets, however, there was still a significant amount of noice and extra light in the image. 




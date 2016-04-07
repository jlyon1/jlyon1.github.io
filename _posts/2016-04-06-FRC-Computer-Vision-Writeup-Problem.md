---
layout: post
title: Team 3044 Stronghold Vision Part 1: The Problem 
---

In our analysis of the game FIRST Stronghold, our team decided that vision tracking of the targets was not only a "Nice to have" Feature, but was a design requirement. Once this was decided, I took on the task of developing a reliable system which we could use in this year's game. We decided that the software must be able to Reliably Locate the position of the targets, interpret the information, and send the results to the robot. Our system used an [Axis M1011 camera](http://www.axis.com/us/en/products/axis-m1011) with modified camera settings, which we plugged directly into our radio for image acquisition, and two green LED rings. The green LED rings illuminated the reflective tape around the target. The result of this setup were images, with a 320px by 240px resolution that had the targets illuminated in the image. 

This article assumes you are already familiar with the game as presented [here](http://www.firstinspires.org/resource-library/frc/competition-manual-qa-system) Although it is not necessary that you know the game to understand this. 

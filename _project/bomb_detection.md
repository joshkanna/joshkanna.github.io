---
title: "Autonomous Bomb Detection Robot"
position: "Engineering Computing Project"
location: "Notre Dame, IN"
date: 2025-04-10
collection: project
permalink: /project/bomb_detection
---

I worked with a 4-person team to build an autonomous robot using a BBC Micro:bit and Python that could navigate complex mazes, hunt for magnetic targets, and wirelessly communicate between two microcontrollers. It was a really fun challenge that combined hardware integration with programming!

We packed the robot with multiple sensors - ultrasonic for obstacle detection, magnetometer for finding targets, line-following sensors, and motor encoders for precise movement. The coolest part was implementing an advanced maze navigation algorithm that could dynamically record its path and then autonomously navigate back to the start once it found all the targets.

One of the bigger challenges was optimizing the embedded system performance since the Micro:bit has pretty limited resources. We focused on memory management and efficient task scheduling to handle all the sensor readings, motor control, and wireless communication smoothly. We also removed redundant code - like cutting out unnecessary wall checks on the exit path since we already knew the route. Getting everything to run efficiently on such a constrained system was definitely a learning experience!

Here's a link to the final presentation: [Final Presentation](https://docs.google.com/presentation/d/1A3qlRVDPjJGXVBZbrajlDvEv31_qV2AapJPDLz2MkKI/edit?usp=sharing)
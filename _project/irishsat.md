---
title: "IrishSAT"
position: "Power and Electronics Project Member"
location: "Notre Dame, IN"
date: 2025-04-15
collection: project
permalink: /project/irishsat
---

I've been working as part of the Power and Electronics team on IrishSat, Notre Dame's CubeSat project! One of my main contributions has been designing a custom Battery Management System using the BQ28Z chip to handle our 2S2P lithium-ion battery pack. I designed the [PCB](BMS.png) in KiCad with an I2C fuel gauge interface so the main Power Control Board can monitor the battery's health.

When we brought up the first board, we ran into some interesting challenges - the BQ28Z chip got stuck in secondary mode, which locked the I2C communication at 1.8V instead of the 3.3V we needed. We also realized that due to some uncertainty with CSLI funding from NASA, we needed to reformat the project approach. Now I'm serving as the responsible engineer for the BMS board, which means I'm leading a small team through chip selection (we're moving away from the BQ28Z) and keeping the larger team updated on our progress.

I also worked on the satellite's attitude control system, implementing a custom magnetorquer wrapping setup using an Arduino and stepper motor control. This lets us precisely control the satellite's orientation in space! Here's a video of it in action: [Magnetorquer Wrapping video](magnetorquer_wrapping.mp4)

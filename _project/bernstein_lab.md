---
title: "Bernstein Lab"
position: "Undergraduate Research Assistant"
location: "Notre Dame, IN"
date: 2025-12-18
collection: project
permalink: /project/bernstein_lab
---

I’ve been working as a research assistant in the Bernstein Lab at Notre Dame, where I spent the semester automating the characterization process for a specialized infrared detector called a TECNA (Thermoelectrically Coupled Nanoantenna).

Before this project, the lab had to manually sync a rotational motor with a lock-in amplifier, which was slow and prone to timing errors. I developed a unified software suite in Python using the QCoDeS framework to bridge the gap between the hardware and the data. I modernized the driver for a Newport SMC100 controller, implementing custom error-handling and translating raw motor counts into precise angular degrees.

To validate the code, I ran polarization sweeps that successfully captured the expected cos²(θ) response of the nanoantennas, proving the system was accurate. We’re now ready to use this for live imaging as soon as our new focusing lenses are ready!

I also expanded the project to include a 2D "snaking" raster scan using Thorlabs Kinesis motors, which allows us to create spatial thermal maps of the devices.

Here's a link to the final report: [Fall 2025 Research Report](Fall2025ResearchReport.pdf)

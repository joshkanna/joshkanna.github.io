---
layout: default
title: Projects
---

<section id="projects">
        <div class="container">
            <div class="section-header">
                <h2>Projects</h2>
            </div>
            
            <div class="projects-grid">
                <!-- Project 1: CubeSat BMS -->
                <div class="project-card">
                    <div class="project-header">
                        <h3>Battery Management System for IrishSat's CubeSat</h3>
                        
                        <p>
                        The Battery Management System (BMS) is a custom-designed board built to manage and protect IrishSat's 2S2P lithium-ion battery pack. It monitors cell health in real time and communicates state-of-health data to the Power Hub Board over SMBus, ensuring the satellite's power subsystem stays informed and protected throughout operation.
                        </p><br>

                        
                        <p>
                        At the heart of the design is the Texas Instruments BQ40Z50-R2, a fuel gauge IC with built-in overcurrent and overvoltage protection and active cell balancing — all communicated over a 3.3V SMBus interface. The board interfaces with a network of peripherals including the Power Hub via a 6-pin I2C/power connector, four NTC thermistors for temperature sensing across the pack, a PTC thermistor for safety cutoff, and an additional NTC routed out to the Power Hub for external monitoring.
                        </p><br>

                        <p>
                        The board is a 4-layer design with a dedicated ground plane on the bottom layer. High-current paths on the top layer use copper pours to reduce resistance and thermal stress, with the pack negative stitched to ground through a sense resistor and a net tie connecting 1N to GND. Layout decisions prioritized modularity, crosstalk minimization, and trace width scaled to each current path — from milliamp signal lines to the full pack discharge current.
                        </p><br>

                    </div>

                    <div class="project-links">
                        <a href="/assets/BMS_3D_Model.png" class="btn btn-outline" target="_blank">
                            <i class="bi bi-cpu"></i> PCB 3D Model
                        </a>
                        <a href="/assets/System Diagram.png" class="btn btn-outline" target="_blank">
                            <i class="bi bi-layers"></i> CubeSat System Architecture
                        </a>
                    </div>
                    
                    
                </div>

            
                <!-- Project 2: MIDI Synthesizer -->
                <div class="project-card">
                    <div class="project-header">
                        <h3>MIDI Synthesizer</h3>
                        <p>
                        This project involves the development of a polyphonic MIDI synthesizer utilizing an ESP32 microcontroller and a USB Host Shield to interface with digital pianos. The system is designed to perform real-time waveform generation (sine, square, triangle, sawtooth) with audio output delivered through dual 40mm speakers.
                        </p><br>

                        <p>
                        To transition the design from a prototype to a finished product, a custom PCB was developed in KiCad. This board integrates the ESP32, a Digital-to-Analog Converter (DAC), an amplifier, and necessary peripheral components into a compact footprint. The system firmware is written in C++, managing both MIDI protocol processing and software-defined audio synthesis.
                        </p><br>

                        <p>
                        The hardware was manufactured by JLCPCB and assembled using pick-and-place equipment at the Engineering Innovation Hub at the University of Notre Dame. This integrated approach replaces the initial breadboard circuit with a more robust and professional hardware solution.
                        </p><br>
                    </div>

                    <div class="project-links">
                        <a href="/assets/midi_synth_system.jpeg" class="btn btn-outline" target="_blank">
                            <i class="bi bi-cpu"></i> Full System
                        </a>
                        <a href="/assets/midi_PCB.png" class="btn btn-outline" target="_blank">
                            <i class="bi bi-layers"></i> PCB 3D Model
                        </a>
                        <a href="/assets/midi_synth_video.mp4" class="btn btn-outline" target="_blank">
                            <i class="bi bi-play-circle"></i> Video Demo
                        </a>
                    </div>
                </div>


                <!-- Project 3: Motion Control -->
                <div class="project-card">
                    <div class="project-header">
                        <h3>Automated Measurement Control for TECNA Characterization</h3>
                        <p>
                        Before this project, the lab had to manually sync a rotational motor with a lock-in amplifier, which was slow and prone to timing errors. I developed a unified software suite in Python using the QCoDeS framework to bridge the gap between the hardware and the data. I modernized the driver for a Newport SMC100 controller, implementing custom error-handling and translating raw motor counts into precise angular degrees.
                        </p><br>

                        <p>
                        To validate the code, I ran polarization sweeps that successfully captured the expected cos²(θ) response of the nanoantennas, proving the system was accurate. We’re now ready to use this for live imaging as soon as our new focusing lenses are ready. I also expanded the project to include a 2D “snaking” raster scan using Thorlabs Kinesis motors, which allows us to create spatial thermal maps of the devices.
                        </p><br>
                    </div>
                    <div class="project-links">
                        <a href="/assets/Fall 2025 Research Report.pdf" class="btn btn-outline" target="_blank">
                            <i class="bi bi-cpu"></i> Research Report
                        </a>
                    </div>
                    
                
                </div>

                <!-- Project 4: Autonomous Bomb Detection Robot -->
                <div class="project-card">
                    <div class="project-header">
                        <h3>Autonomous Bomb Detection Robot</h3>
                        <p>
                        I worked with a 4-person team to build an autonomous robot using a BBC Micro:bit and Python that could navigate complex mazes, hunt for magnetic targets, and wirelessly communicate between two microcontrollers. It was a really fun challenge that combined hardware integration with programming!
                        </p><br>

                        <p>
                        We packed the robot with multiple sensors - ultrasonic for obstacle detection, magnetometer for finding targets, line-following sensors, and motor encoders for precise movement. The coolest part was implementing an advanced maze navigation algorithm that could dynamically record its path and then autonomously navigate back to the start once it found all the targets.
                        </p><br>

                        <p>
                        One of the bigger challenges was optimizing the embedded system performance since the Micro:bit has pretty limited resources. We focused on memory management and efficient task scheduling to handle all the sensor readings, motor control, and wireless communication smoothly. We also removed redundant code - like cutting out unnecessary wall checks on the exit path since we already knew the route. Getting everything to run efficiently on such a constrained system was definitely a learning experience!
                        </p><br>
                        
                        <div class="project-links">
                        <a href="https://docs.google.com/presentation/d/1A3qlRVDPjJGXVBZbrajlDvEv31_qV2AapJPDLz2MkKI/edit?slide=id.p#slide=id.p" class="btn btn-outline" target="_blank">
                            <i class="bi bi-cpu"></i> Final Presentation
                        </a>
                    </div>
                    </div>

                    
                </div>
            </div>
        </div>
    </section>
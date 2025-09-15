---
title: "Midi Synthesizer"
position: "Individual Project"
location: "Dublin, IE"
date: 2025-08-20
collection: project
permalink: /project/midi
---

I've been working on this MIDI synthesizer project that I'm really excited about! It uses an ESP32 with a USB Host Shield to connect to digital pianos, and I designed it to generate different waveforms (sine, square, triangle, sawtooth) with real-time polyphonic playback through dual 40mm speakers.

I designed a custom [PCB](midi_PCB.png) in KiCad to integrate the ESP32, DAC, amplifier, and all the supporting components into a compact form factor. The firmware handles all the MIDI processing and software-defined waveform generation in C++.

Right now I have it working on a breadboard circuit, but I've ordered the custom PCB from JLCPCB and will be assembling all the components using the pick and place machine at Notre Dame's Engineering Innovation Hub with Professor Snider's help. Can't wait to swap out the breadboard for the PCB - should be way more compact and give cleaner audio with less static from better connections!

Here's a video of the synth in action: [Midi Synth Breadboard](midi_synth_breadboard.mp4)

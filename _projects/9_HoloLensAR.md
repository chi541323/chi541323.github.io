---
layout: page
title: Designing AR HMI Controls for Robotic Systems
description: This project explored a new human-machine interaction paradigm for industrial environments. I designed a proof-of-concept using an Augmented Reality (AR) interface to enable intuitive and seamless gestural control of a robotic system.
img: assets/img/HololensAR/3.png
importance: 7
category: UI/UX
paper: Work at AUO
---

<b class="font-weight-bold">Note: Due to a Non-Disclosure Agreement (NDA), specific details and visuals of this project have been omitted. Further insights can be shared during the interview.</b>

<!-- Project Overview -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Project Overview</h2>
    <ul>
        <li class="mt-3"><b class="font-weight-bold my-color-b">Project Name</b></li>
            Designing AR HMI Controls for Robotic Systems
        <li><b class="font-weight-bold my-color-b">My Role</b></li>
            Interaction Designer & Interface Developer
        <li><b class="font-weight-bold my-color-b">Core Technologies</b></li>
            Unity3D (C#), AR Interface Design, Spatial Gestural Interaction, Haptic Feedback (Arduino, C++)
    </ul>
</div>

<!-- Problem & Challenge -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Problem & Challenge</h2>
    <p class="mt-3">The rise of smart manufacturing presents a need for more intuitive machine control interfaces. Traditional methods, such as control panels, can be cumbersome and inefficient. To address this challenge, our goal was to develop a proof-of-concept that explores how Augmented Reality (AR) could create a new paradigm for industrial human-machine interaction.</p>
    <p>Our team faced three key challenges:</p>
    <ul>
        <li><b class="font-weight-bold my-color-b">Spatial Interaction</b></li>
            How to design a gestural interface that allows users to intuitively and precisely control a real-world object like a robotic arm within a 3D space.
        <li><b class="font-weight-bold my-color-b">Information Overlay</b></li>
            How to present critical real-time data (e.g., temperature, component angles) in the user's field of view without obstructing their perception of the physical environment.
        <li><b class="font-weight-bold my-color-b">The Haptic Gap</b></li>
            Without physical buttons, users lose the tactile feedback that confirms an action has been triggered, leading to a disconnect and potential for errors.
    </ul>
</div>

<!-- My Process & Contributions -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">My Process & Contributions</h2>
    <p class="mt-3"> 
    I led the interaction design and development for this project's short-term goal: to <b class="font-weight-bold my-color-b">create an AR interface on HoloLens 2 to control a robotic arm.</b>
    </p>
    <p>
    My primary contribution was to bridge the gap between virtual commands and physical actions. I developed a gestural interface that utilizes HoloLens 2's hand-tracking capabilities to manipulate a virtual control panel. This interface then transmits commands via Bluetooth to control the physical robotic arm.
    </p>
    <p>
    During the development process, I collaborated closely with our team's designer to create a <b class="font-weight-bold my-color-b">user-friendly interface for both control and data visualization</b>. We also proactively addressed the issue of missing tactile feedback. We explored solutions for haptic feedback by utilizing an <b class="font-weight-bold my-color-b">UltraHaptics device for ultrasonic feedback</b> and building a prototype based on the <b class="font-weight-bold my-color-b">'Touch&Fold' paper for vibrational feedback</b>, enhancing user confidence and precision during control.
    </p>
    <!-- image -->
    <div class="row justify-content-sm-center mt-5">
        <div class="col-sm-6 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/HololensAR/1.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-6 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/HololensAR/2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<!-- Outcome & Impact -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Outcome & Impact</h2>
    <p>
        The outcome was a successful proof-of-concept that demonstrated the viability of a gestural AR interface for controlling complex machinery. The fully functional prototype, capable of manipulating a robotic arm, validated our core hypothesis that AR interaction can create a more intuitive and seamless control experience. This project laid the foundational work for our team, providing a tangible sector concept that guided the future development of AR solutions for the manufacturing. It highlighted the potential to improve operational efficiency and reduce cognitive load through a new paradigm of human-machine interaction.
    </p>
</div>

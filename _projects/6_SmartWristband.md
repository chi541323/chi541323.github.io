---
layout: page
title: Rehabilitation and Fitness Wristband
description: A smart wristband solution that empowers users in both rehabilitation and fitness. It provides real-time motion tracking and Bluetooth feedback to ensure safe and effective exercise, transforming a traditional workout into a data-driven, guided experience.
img: assets/img/Wristband/1.png
importance: 6
category: Embedded System
paper: Course Project 2014
---

<!-- Motivation -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Motivation</h2>
        <p>Our project was born from two key observations. First, we identified a critical gap in rehabilitation, where a single therapist often struggles to provide continuous, one-on-one guidance to multiple patients. This led us to envision a system that could automate progress tracking, form monitoring, and provide timely, tactile feedback to patients.</p>

        <p>Simultaneously, we recognized the increasing popularity of smart wristbands, yet noted a lack of features for tracking specific activities like weightlifting repetitions. We understood that proper form is crucial in strength training to prevent injury. By combining these insights, we were motivated to create a wearable wristband with integrated rehabilitation functions. This device would serve a dual purpose: providing essential monitoring for patients during therapy and empowering everyday users to exercise safely and effectively with real-time feedback.</p>
</div>

<!-- image -->
<div class="row">
    <div class="col-sm mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Wristband/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<!-- Prototype -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Prototype</h2>
        <p>To monitor and track exercise performance, we developed an embedded system using an Arduino board and a complementary mobile application. The system utilizes a three-axis accelerometer and a gyroscope to collect motion data, such as joint angles and velocity, which are then transmitted to the mobile app via Bluetooth.</p>
        <div class="row">
            <div class="col-sm-9 mt-md-0">
                {% include figure.liquid loading="eager" path="assets/img/Wristband/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class="col-sm-3 mt-md-2">
                {% include figure.liquid loading="eager" path="assets/img/Wristband/7.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
        <p>We collaborated with a physical therapist to establish specific criteria for correct exercise form, including target angles and speeds. The system analyzes the real-time motion data and only registers a repetition when the patient's movement meets these criteria. This ensures that the tracked count not only reflects the number of repetitions but also confirms the accuracy of each movement, providing users with information on both their progress and the correctness of their form.</p>
</div>

<div class="row">
    <div class="col-sm mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Wristband/4.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row">
    <div class="col-sm mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Wristband/5.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<!-- Our Award Moment -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Our Award Moment</h2>
        <div class="row">
            <div class="col-sm mt-md-0">
                {% include figure.liquid loading="eager" path="assets/img/Wristband/6.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
</div>
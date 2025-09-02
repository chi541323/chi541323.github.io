---
layout: page
title: Bridging Unity and Arduino
description: Bridges the physical and virtual worlds. The Arduino-based embedded system collects real-time data (e.g., from a three-axis accelerometer or gyroscope) and transmits it to our Unity application via a physical connection (such as USB) or Bluetooth for real-time visualization and feedback. Conversely, our Unity interface can also send messages back to the Arduino to control components like a motor.
img: assets/img/BridgingUnityArduino/1.png
importance: 6
category: Fun
---

Bridges the physical and virtual worlds. The Arduino-based embedded system collects real-time data (e.g., from a three-axis accelerometer or gyroscope) and transmits it to our Unity application via a physical connection (such as USB) or Bluetooth for real-time visualization and feedback. Conversely, our Unity interface can also send messages back to the Arduino to control components like a motor.

<div>
    <p>After writing and uploading a program to the Arduino, you can establish a communication link with it via the Arduino Serial Monitor, Processing, or Unity. This allows you to send commands to control components like motors or receive data from sensors such as pressure sensors.</p>
    <!-- image -->
    <div class="row">
        <div class="col-sm-6 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/BridgingUnityArduino/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-6 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/BridgingUnityArduino/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<div>
    <p>We can use devices like the HTC Vive or Leap Motion to control actions within Unity3D. If we establish communication between Unity3D and Arduino, this means you can use an action in VR (e.g., a hand gesture with Leap Motion or a movement with the HTC Vive controller) to trigger the Arduino to control a motor. Conversely, data from sensors on the Arduino, like a pressure sensor, can trigger events or activities within the Unity3D application.</p>
     <!-- image -->
    <div class="row">
        <div class="col-sm">
            {% include figure.liquid loading="eager" path="assets/img/BridgingUnityArduino/4.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<div>
    <p>To create a simple Unity3D interface that communicates with an Arduino to control a servo motor, you first need to understand the hardware. The Arduino board has both analog and digital pins. For motor control, you'll need to use a digital pin that supports PWM (Pulse Width Modulation), a technique that controls analog components by rapidly switching the digital output on and off.</p>
    <p>You also need to know how to properly connect the motor to the Arduino, which involves connecting its power, ground, and signal wires. Once the hardware is set up, you can write the code on both the Arduino and in Unity3D to establish communication and send the necessary signals.</p>
    <!-- image -->
    <div class="row">
        <div class="col-sm-6 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/BridgingUnityArduino/5.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-6 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/BridgingUnityArduino/6.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Example</h2>
    <div>
        <p>You can download Arduino and Unity3D example to control motor here
            <a href="/assets/BridgingUnityArduino/Controller-Arduino-and-Unity.zip" class="btn-no-shadow btn btn-sm btn-outline-primary ml-1 ml-md-4 mt-1" target="_blank">
            <i class="fa-solid fa-file-pdf"></i> Download
            </a>
        </p>
    </div>
</div>

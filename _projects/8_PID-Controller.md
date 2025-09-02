---
layout: page
title: PID Controller
description: Using a PID Controller to Control a Motor. A PID controller is highly effective for motor control. Its primary application is to ensure a motor's output—such as speed, position, or torque—precisely reaches and maintains a set target value.
img: assets/img/PIDController/1.png
importance: 7
category: Fun
---

<!-- Motivation -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Motivation</h2>
        <p>Learn how to use a PID controller for precise motor control. This skill is essential for future projects involving applications like robotic arms or any system requiring accurate motor movement. I knew that simply adjusting a motor's voltage (an open-loop control) would lead to unstable speeds due to factors like friction or changing loads. My goal for this project was to solve this issue by implementing PID closed-loop control, allowing the motor to consistently and accurately maintain a target speed.</p>
</div>
<!-- image -->
<div class="row justify-content-sm-center mt-5">
    <div class="col-sm-6 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/PIDController/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Introduce</h2>
    <p><b class="font-weight-bold">What is a PID Controller?</b></p>
    <p>A PID (Proportional–Integral–Derivative) controller is a widely used control algorithm in industrial and engineering fields. Its primary goal is to make a system's output (e.g., motor speed, temperature) as close as possible to a desired setpoint (target value).</p>

    <p>Imagine you're driving a car and your goal is to maintain a speed of 100 km/h.</p>
    <ul>
        <li>If your speed is only 90 km/h, you press the gas pedal to accelerate.</li>
        <li>If your speed is 110 km/h, you ease off the gas pedal to slow down.</li>
    </ul>
    <p>This process of adjusting the gas pedal is what a PID controller does, but with much greater precision.</p>
</div>

<div>
    <ul>
        <li><b class="font-weight-bold my-color-b">Proportional (P):</b> This component provides an immediate response to the current error. A large P value leads to a quick reaction but can also cause the motor to overshoot its target speed.</li>
        <li><b class="font-weight-bold my-color-b">Integral (I):</b> This part helps eliminate any persistent, small errors (steady-state error) that the P component might miss. It accumulates these past errors over time, ensuring the motor eventually reaches the exact target speed. However, an overly high I value can increase the system's response time.</li>
        <li><b class="font-weight-bold my-color-b">Derivative (D):</b> This component anticipates future error by reacting to the rate of change. It is crucial for damping the system, preventing overshoots and oscillations, and making the motor's movement smoother and more stable.</li>
    </ul>
</div>

<!-- image -->
<div class="row justify-content-sm-center mt-5">
    <div class="col-sm-6 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/PIDController/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


<!-- Technical -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Technical</h2>
        <p class="mt-3"><b class="font-weight-bold my-color-b">Hardware</b></p>
        <ul>
            <li>The core of this project's hardware consists of an Arduino as the embedded system.</li>
            <li>For the motor, I used the Pololu 12 HPCB gear motor with a 298:1 gearhead. </li>
            <li>To control the motor's power and direction, I used a motor driver (TB6612FNG).</li>
            <li>To measure the motor's rotational speed, I incorporated an encoder.</li>
        </ul>
        <p class="mt-3"><b class="font-weight-bold my-color-b">Software</b></p>
        <ul>
            <li>Set all gains to zero.</li>
            <li>Increase the P gain until the response to a disturbance is steady oscillation.</li>
            <li>Increase the D gain until the the oscillations go away (i.e. it's critically damped).</li>
            <li>Repeat steps 2 and 3 until increasing the D gain does not stop the oscillations.</li>
            <li>Set P and D to the last stable values.</li>
            <li>Increase the I gain until it brings you to the setpoint with the number of oscillations desired (normally zero but a quicker response can be had if you don't mind a couple oscillations of overshoot)</li>
        </ul>
</div>

<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Example</h2>
        <p>You can download example here
            <a href="/assets/PIDController/PID-Controller.zip" class="btn-no-shadow btn btn-sm btn-outline-primary ml-1 ml-md-4 mt-1" target="_blank">
            <i class="fa-solid fa-file-pdf"></i> Download
            </a>
        </p>
</div>
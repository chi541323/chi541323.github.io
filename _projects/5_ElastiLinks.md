---
layout: page
title: ElastiLinks - Force Feedback between VR Controllers with Dynamic Points of Application of Force
description: Handheld VR controllers that provide force feedback with dynamic points of application (PAFs) using rotatable tracks. Conducted perception studies on resistive and impact forces, as well as PAF offsets and rotations. Results show that dynamic PAFs enhance realism and user experience in VR.
img: assets/img/elastilinks/elastilink_30.gif
importance: 5
category: Human-Computer Interactions
paper: ACM UIST 20
author: Tzu-Yun Wei, Hsin-Ruey Tsai, Yu-So Liao, Chieh Tsai, Yi-Shan Chen, <span style='font-weight:900;'>Chi Wang</span>, Bing-Yu Chen
---

Handheld VR controllers that provide force feedback with dynamic points of application (PAFs) using rotatable tracks. Conducted perception studies on resistive and impact forces, as well as PAF offsets and rotations. Results show that dynamic PAFs enhance realism and user experience in VR.

<div class="embed-responsive embed-responsive-16by9 mb-3">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/subl15vGq7Y?si=RxkMmf_r23z9wYXv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

<!-- Motivation -->
<div class="row">
    <div class="col-md-7">
        <h2 class="mt-5 font-weight-bold">Motivation</h2>
            <!-- 左邊文字 -->
                <p style="text-align: justify;">Conventional VR controllers mostly rely on vibration motors, which provide only limited tactile cues and lack realistic kinesthetic feedback. This restricts how well users can perceive forces, object resistance, and two-handed interactions (e.g., stretching, pulling, or bending objects). To address this gap, ElastiLinks was proposed to provide dynamic and reconfigurable force feedback between two VR controllers, enabling more immersive and natural interactions.</p>
    </div>
    <!-- 右邊圖片 -->
    <div class="col-md-5 mt-5">
        {% include figure.liquid path="assets/img/elastilinks/1.png" title="example image" class="img-fluid rounded z-depth-1 w-100"%}
    </div>
</div>

<!-- Design -->
<div>
    <h2 class="mt-5 font-weight-bold">Design</h2>
        <p>ElastiLinks are handheld VR controllers designed to enhance realism by providing dynamic points of application of force (PAFs), allowing them to simulate not only the magnitude of a force but also the torque a user would feel in their hands.</p>
        <ul>
            <li><b style="font-weight:900;">Considerations</b></li>
                <ul>
                    <li class="font-weight-bold">Realism</li> 
                    The primary goal is to provide realistic force feedback with accurate PAFs to simulate both force and torque for various applications.
                    <li class="font-weight-bold">Versatility</li> 
                    The device is designed to be versatile, capable of generating two common types of force feedback—resistive force and impact—with multiple levels of intensity.
                    <li class="font-weight-bold">Comfort and Safety</li> 
                    The force output is carefully limited to a safe and comfortable range to prevent user injury or discomfort.
                    <li class="font-weight-bold">Mobility</li> 
                    The controllers are designed to be lightweight (750g total) and compact to avoid hindering user movement or causing fatigue.
                </ul>
                <li class="mt-2"><b style="font-weight:900;">Hardware</b></li>
                    <ul>
                        <div class="row">
                            <div class="col-md-7">
                            <li class="font-weight-bold">Main Components</li> 
                            ElastiLinks consists of two controllers, tracks, connectors, and force links. The connectors on the tracks act as the dynamic PAFs.
                            <li class="font-weight-bold">Force Links</li> 
                                <ul>
                                    <li class="font-weight-bold">Resistive Link</li> 
                                    A motor adjusts the length of a rubber band by winding it, which changes its tension and provides a variable resistive force when the controllers are pulled apart.
                                    <li class="font-weight-bold">Impact Link</li> 
                                    A motor stretches a rubber band to store energy, which is then suddenly released by a mechanical brake to create a sharp, pulling impact.
                                </ul>
                            </div>
                            <div class="col-md-5">
                                {% include figure.liquid path="assets/img/elastilinks/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
                            </div>
                        </div>
                        <li class="font-weight-bold">Dynamic PAF Mechanism</li> 
                            Dynamic PAFs are achieved using two DC motors on each controller: a rotation motor that rotates the track and an offset motor that moves the connector along the track.                     
                        <li class="font-weight-bold">Features</li> 
                            <ul>
                                <li class="font-weight-bold">Wire Brakes</li> 
                                Each force link has a wire brake that can be locked to restrict controller movement, enabling force delivery only when needed.
                                <li class="font-weight-bold">Weight</li> 
                                The total weight is 750g (without Vive trackers), with one controller weighing 350g and the other 400g.
                            </ul>
                    </ul>
            <li><b style="font-weight:900;">Operation</b></li>
                <ul>
                    <li class="font-weight-bold">Initialization</li> 
                    The device automatically sets the tracks and connectors to a home position and keeps the wire brakes in a free state, allowing for unrestricted movement.
                    <li class="font-weight-bold">Resistive Force Delivery</li> 
                    The resistive motor winds the band, and the rotation and offset motors simultaneously move the connector to the correct PAF. The wire brake then locks, allowing the user to feel resistance when they pull the controllers apart.
                    <li class="font-weight-bold">Impact Delivery</li> 
                    An impact motor extends the band to store power while the connectors move to the target PAF. The wire brake locks, and a servo motor releases the brake to produce the impact before returning to a free state.
                    <li class="font-weight-bold">Limitations</li> 
                    Due to hardware limitations, the track rotation is restricted to a -90 to 60-degree range. The actuation of the motors and brakes involves delays, which are accounted for in the software to ensure proper force delivery.
                </ul>
        </ul>
        <!-- image -->
        <div class="row justify-content-sm-center">
            <div class="col-sm-6 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/elastilinks/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
</div>

<!-- User Study -->
<div>
    <h2 class="mt-5 font-weight-bold">User Study</h2>
    <p>In this series of studies, our primary goal was to evaluate the effectiveness of the ElastiLinks haptic controller. The first study focused on whether users could distinguish different levels of resistive force and impact, while the second investigated if they could perceive changes in the Points of Application of Force (PAFs), specifically in terms of rotation and offset.</p>
    <ul>
        <li><b style="font-weight:900;">Methodology</b></li>
            <ul>
                <li>Both studies involved 12 participants and used identical VR setups.</li>
                <li>In Study 1, participants matched the perceived force intensity to a visual scale.</li>
                <li>In Study 2, the force level was held constant while participants matched the perceived torque and force direction to a virtual PAF location.</li>
            </ul>
        <li><b style="font-weight:900;">Findings</b></li>
            <ul>
                <li><b style="font-weight:900;">Force Level Distinguishability (Study 1)</b></li>
                    <ul>
                        <li><b style="font-weight:900;">Resistive Force & Impact:</b></li>
                        Users could clearly distinguish between all three tested levels for both resistive force and impact.
                        <li><b style="font-weight:900;">Application Note</b></li>
                        While the lowest impact level was distinguishable, its force was too weak to realistically simulate an impact in a VR application.
                    </ul>
                <li><b style="font-weight:900;">PAF Distinguishability (Study 2)</b></li>
                    <ul>
                        <li><b style="font-weight:900;">Resistive Force</b></li>
                        Participants could differentiate between various rotation angles and offset positions. However, they struggled to identify the direction of rotation and had difficulty distinguishing offset positions that were close to the center.
                        <li><b style="font-weight:900;">Impact</b></li>
                        Due to its short duration, the PAF distinguishability of impact was much lower than that of resistive force. Users found it difficult to perceive the subtle changes in rotation and offset.
                    </ul>
            </ul>
        <p>The ElastiLinks system effectively generates multilevel forces and haptic cues to convey torque and direction, with resistive force proving to be more distinguishable than impact for both force level and PAFs due to its longer duration, offering valuable insights for future VR haptic designs.</p>
        <!-- image -->
        <div class="row justify-content-sm-center mt-3">
            <div class="col-sm-7 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/elastilinks/4.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class="col-sm-5 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/elastilinks/5.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
    </ul>
</div>

<!-- Demo Application -->
<div>
    <h2 class="mt-5 font-weight-bold">Demo Application</h2>
    <p>Our objective was to evaluate how dynamic Points of Application of Force (PAFs) affect the VR experience. We recruited 12 participants with prior VR experience to test the ElastiLinks system across three different applications designed to represent various interaction types: a Survival Shooter Game for bimanual use, a Fighting Game for body-grounded interactions, and a Fishing Game where a controller was fixed to the environment.</p>
    <p class="font-weight-bold mt-3"> User Evaluation Study</p>
    <ul>
        <li class="font-weight-bold">Methodology</li>
            <ul>
                <li>Participants: 12 participants (5 female), all with prior VR experience.</li>
                <li><b class="font-weight-bold">Survival Shooter Game: </b>For bimanual interactions (e.g., using a bow and rifle).</li>
                <li><b class="font-weight-bold">Fighting Game: </b>For body-grounded interactions (e.g., with a controller attached to the arm).</li>
                <li><b class="font-weight-bold">Fishing Game: </b>For environment-grounded interactions (e.g., with one controller fixed to a desk).</li>
            </ul>
        <li class="font-weight-bold">Evaluation</li>
        Participants compared three feedback methods: a vibration baseline, fixed PAFs, and dynamic PAFs. They rated each on a 1-7 scale for realism, enjoyment, and distinguishability.
        <li class="font-weight-bold">Key Finding</li>
            <ul>
                <li class="font-weight-bold">Survival Shooter Game</li>
                    Dynamic PAFs significantly outperformed the other methods in all three categories. Participants noted that the changing PAFs in weapons like a slingshot felt more realistic and helped them distinguish between different weapons. While the device's weight and delays were sometimes an issue, participants still found the haptic feedback highly realistic.
                <li class="font-weight-bold">Fighting Game</li>
                    Dynamic PAFs also showed significant improvements in realism, enjoyment, and distinguishability. Participants could perceive the change in the direction of the impact when using different weapons, which made the experience feel more like a real object cutting through the air. The feedback also made the weapons feel distinct by affecting their perceived center of mass.
                <li class="font-weight-bold">Fighting Game</li>
                   Dynamic PAFs were again significantly better. Participants were surprised by how realistic the moving PAF on the grounded controller felt, as it effectively simulated the sensation of a fish struggling on a line, which a fixed PAF could not replicate.
            </ul>
    </ul>
    <p class="mt-3">This study confirms the importance of dynamic PAFs, which significantly enhance the realism, enjoyment, and distinguishability of VR experiences across various interactions, including bimanual, body-grounded, and environment-grounded. Despite hardware limitations like weight and delays, the ElastiLinks system provides highly realistic feedback, offering valuable insights for the design of future VR haptic devices.</p>
    <!-- image -->
    <div class="row">
        <div class="col-md-6">
            {% include figure.liquid path="assets/img/elastilinks/6.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-6">
            {% include figure.liquid path="assets/img/elastilinks/7.png" title="example image" class="img-fluid rounded z-depth-1" %}
            {% include figure.liquid path="assets/img/elastilinks/8.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<!-- Finding -->
<div>
    <h2 class="mt-5 font-weight-bold">Finding</h2>
        <p>The studies confirm that ElastiLinks provides effective kinesthetic feedback by dynamically modulating force application points between VR controllers, enabling users to clearly perceive differences in force direction and strength, which in turn enhanced their sense of object weight, stiffness, and resistance. Compared to vibration-only feedback, ElastiLinks significantly improved realism, immersion, and intuitiveness in VR interactions, suggesting that it offers not only enhancements for VR gaming but also a new interaction paradigm for training, collaboration, and everyday VR applications where realistic two-handed force feedback is crucial.</p>
</div>
<div>
    <p>For more details, please see our paper
        <a href="/assets/papers/ElastiLink.pdf" class="btn-no-shadow btn btn-sm btn-outline-primary ml-1 ml-md-4 mt-1" target="_blank">
        <i class="fa-solid fa-file-pdf"></i> Download PDF
        </a>
    </p>
</div>
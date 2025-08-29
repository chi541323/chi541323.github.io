---
layout: page
title: Gaiters - Exploring Skin Stretch Feedback on Legs for Enhancing Virtual Reality Experiences
description: Leg-worn devices that generate 2D skin stretch feedback to simulate virtual textures and directional cues. Conducted studies on perceivable stretch and evaluated user experiences. Results show rich and enjoyable haptic feedback on the lower limbs in VR.
img: assets/img/gaiters/gaiters_30.gif
importance: 2
category: Human-Computer Interactions
paper: ACM CHI 19
author: <span style='font-weight:900;'>Chi Wang</span>, Da-Yuan Huang, Shuo-Wen Hsu, Cheng-Lung Lin, Yeu-Luen Chiu, Chu-En Hou, Bing-Yu Chen
---

Leg-worn devices that generate 2D skin stretch feedback to simulate virtual textures and directional cues. Conducted studies on perceivable stretch and evaluated user experiences. Results show rich and enjoyable haptic feedback on the lower limbs in VR.

<div class="embed-responsive embed-responsive-16by9 mb-3">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/ZZ0PffUZP70?si=Iht25dGNNinJQtlq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

<!-- Motivation -->
<div>
    <h2 class="mt-5 font-weight-bold">Motivation</h2>

    <p>While haptic feedback in VR has traditionally focused on the hands, torso, or face, the legs have been relatively underexplored, despite their central role in locomotion. This work explores skin-stretch feedback on the legs, aiming to enhance immersion by delivering cues related to inertia, motion guidance, and ground contact. We developed wearable gaiters with shear tactors mounted on the calves to investigate the potential of this feedback modality in VR.</p>

    <div class="row">
        <div class="col-sm mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/gaiters/1.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<!-- Design -->
<div>
    <h2 class="mt-5 font-weight-bold">Design Prototype</h2>
    <p>Regarding the stretch location and size, we considered the complexity of leg muscles and tissues, which could lead to varying sensitivity at different positions. To ensure both effectiveness and ease of wear, we excluded the thighs and focused on the calves. Through pilot testing, we further determined the tactor size to be 35 mm in diameter.
    </p>

    <div class="row justify-content-sm-center">
        <div class="col-sm-6 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/gaiters/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-6 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/gaiters/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>

    <p>
    Before building the wearable prototype, we first implemented a leg-scale grounded apparatus. This grounded configuration allowed us to generate strong and clear forces without introducing additional ambiguous feedback. Using this setup, we conducted two psychophysical studies to investigate:
     </p>

    <ul>
        <li class="font-weight-bold">How well can participants discriminate skin stretch distances?</li>
        <li class="font-weight-bold">How well can participants discriminate skin stretch angles?</li>
    </ul>

    <p><b style="font-weight:900;">Stretch Distance:</b> ANOVA showed a significant main effect of distance, indicating that participants could reliably discriminate larger distances from smaller ones.</p>
    <p><b style="font-weight:900;">Stretch Angle:</b> ANOVA revealed a significant effect of angle, suggesting that participants were also sensitive to directional differences.</p>
    
    <div class="row justify-content-sm-center">
        <div class="col-sm-6 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/gaiters/5.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-6 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/gaiters/6.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>


    <p class="mt-4">Based on the results of the psychophysical studies, we designed a wearable gaiter-like device equipped with four independently controlled shear tactors mounted around the lower legs. Each tactor delivered skin stretch feedback in different directions by rotating small wheels in direct contact with the skin.</p>

   <div class="row align-items-center">
        <!-- 左邊圖片 -->
        <div class="col-md-5 text-center">
            {% include figure.liquid path="assets/img/gaiters/4.png" title="example image" class="img-fluid rounded z-depth-1 w-100"%}
        </div>

        <!-- 右邊條列 -->
        <div class="col-md-7">
            <ul>
                <li><b style="font-weight:900;">Exploratory Phase: </b> Prior to finalizing the design, we conducted informal tests to identify the most comfortable and perceivable skin contact areas on the legs.</li>
                <li><b style="font-weight:900;">Hardware: </b> The gaiters were lightweight and flexible, allowing them to be worn over clothing without restricting walking movements.</li>
                <li><b style="font-weight:900;">Feedback Control: </b> The tactors provided both continuous stretch (e.g., simulating inertia or slopes) and event-based cues (e.g., simulating impacts or environmental changes).</li>
            </ul>
        </div>
    </div>
</div>

<!-- User Study -->
<div>
    <h2 class="mt-5 font-weight-bold">User Study</h2>
    <p>The aim of this exploratory study is to test these action-coupled profiles and to understand how to utilize them to induce different types of perceptions. The action-coupled study evaluated <b style="font-weight:900;">six stretch profiles (Upward, Downward, Forward, Backward, Leftward, Rightward)</b> across <b style="font-weight:900;">three leg actions (Standing, Walking, Kicking)</b> to investigate four perceptual categories: Pulling Force, Weight, Rotational Force, and Friction. </p>

    <p>Results showed that</p>
    <ul>
        <li>Downward and Backward stretches during Standing and Walking effectively induced pulling sensations.</li>
        <li>While Upward and Downward stretches modulated weight perception (heavier vs. lighter legs).</li>
        <li>Leftward and Rightward stretches were effective in evoking rotational forces during Standing but became less perceivable during dynamic actions like Walking or Kicking.</li>
        <li>Friction-related sensations showed consistently high agreement across all profiles, supporting the use of leg skin stretch to simulate rich tactile textures.</li>
    </ul>
    <div class="row justify-content-sm-center">
        <div class="col-sm mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/gaiters/7.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>


<!-- Demo Application -->
<div>
    <h2 class="mt-5 font-weight-bold">Demo Application</h2>
    <p>A user study with 16 participants assessed how effectively the gaiters conveyed direction, intensity, and realism of feedback in VR. Participants engaged in locomotion-related VR tasks with and without haptic feedback, allowing comparison of perceived immersion, guidance, and naturalness of experience.</p>

    <div class="row align-items-center">
        <!-- 左邊圖片 -->
        <div class="col-md-5 text-center">
            {% include figure.liquid path="assets/img/gaiters/8.png" title="example image" class="img-fluid rounded z-depth-1 w-100"%}
        </div>

        <!-- 右邊條列 -->
        <div class="col-md-7">
                <ul>
                    <li class="font-weight-bold">Application 1: Horror Escape Game</li>
                        <ul>
                            <li>Simulated pulling force</li>
                            <li>Leg grazed by something</li>
                            <li>The sensation of water walking resistance</li>
                            <li>Simulated the water flow</li>
                        </ul>
                    <li class="font-weight-bold">Application 2: Fancy Goal Game</li>
                        <ul>
                            <li>Frontal impact</li>
                            <li>Side impact</li>
                            <li>Acceleration force</li>
                        </ul>
                </ul>
        </div>
    </div>
</div>

<!-- Finding -->
<div>
    <h2 class="mt-5 font-weight-bold">Finding</h2>
    <p>The findings show that skin-stretch feedback on the legs effectively conveys direction and intensity, contributing to a stronger sense of inertia, motion, and overall realism in VR. Participants generally found the feedback comfortable and non-intrusive, even during active leg movement. These results highlight the potential of leg-based haptic feedback for applications such as sports training, navigation assistance, and immersive gaming.</p>
</div>

<div>
    <p>For more details, please see our paper
        <a href="/assets/papers/Gaiters.pdf" class="btn-no-shadow btn btn-sm btn-outline-primary ml-1 ml-md-4 mt-1" target="_blank">
        <i class="fa-solid fa-file-pdf"></i> Download PDF
        </a>
    </p>
</div>

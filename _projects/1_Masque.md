---
layout: page
title: Masque - Exploring Lateral Skin Stretch Feedback on the Face with Head-Mounted Displays
description: An HMD prototype with six skin stretch modules providing 2D haptic feedback on the face. Conducted studies on shear tactor design, comfort, and perceivable stretch distances and angles. Results show Masque enhances VR experiences and is well-received by users as a novel HMD feedback modality.
img: assets/img/masque/masque_30.gif
importance: 1
category: Human-Computer Interactions
paper: ACM UIST 19
author: <span style='font-weight:900;'>Chi Wang</span>, Da-Yuan Huang, Shuo-Wen Hsu, Chu-En Hou, Yeu-Luen Chiu, Ruei-Che Chang, Jo-Yu Lo, Bing-Yu Chen
---

An HMD prototype with six skin stretch modules providing 2D haptic feedback on the face. Conducted studies on shear tactor design, comfort, and perceivable stretch distances and angles. Results show Masque enhances VR experiences and is well-received by users as a novel HMD feedback modality.


<div class="embed-responsive embed-responsive-16by9 mb-3">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/-muq7md0flQ?si=7gSHcIBkTvSVgc6S" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

<!-- Motivation -->
<div>
    <h2 class="mt-5 font-weight-bold">Motivation</h2>

    <p>Most existing haptic feedback techniques for head-mounted displays (HMDs) focus on vibration, thermal or air feedback, suction, or electrical stimulation, while lateral skin stretch on the face has remained largely unexplored. We saw an opportunity for facial skin stretch to enrich VR experiences by providing directional guidance (e.g., where to look or move), motion and inertia cues (such as simulating acceleration while cycling), and even emotional or expressive cues by subtly manipulating facial muscles to affect perceived expressions. To explore this space, our goal was to integrate six controllable shear tactors directly into the HMD interface, enabling continuous tactile signals on the face with varying direction and intensity.</p>

    <div class="row">
        <div class="col-sm mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/masque/1.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<!-- Design -->
<div>
    <h2 class="mt-5 font-weight-bold">Design Prototype</h2>
    <p>To design the shear tactors, we first aimed to identify a contact surface size and shape that most people would find both comfortable and perceptible. Since facial geometry varies significantly across individuals, we conducted an informal exploratory study with twelve participants to evaluate different tactor designs. This study helped us understand which dimensions and forms could deliver consistent and noticeable skin stretch.</p>

    <ul>
        <li class="font-weight-bold">Tactor shape & size pre-study: Compared convex, flat, concave shapes (10/20/30 mm):</li>
        <ul>
            <li>Users preferred 30 mm concave tactors: stable contact, clear sensation, less bone pressure</li>
            <li>10 mm felt sharp and uncomfortable</li>
        </ul>
        <li class="font-weight-bold">Masque Prototype:</li>
        <ul>
            <li>Six actuators: L1/R1 (upper, forehead), L2/R2 (cheeks), L3/R3 (jawline)</li>
            <li>Each tactor = 30 mm concave disk + 2 mm silicone cover, max displacement 15 mm, PC-controlled</li>
            <li>To reduce weight, two mounting options: overhead suspension or body-mounted counterweight</li>
        </ul>
    </ul>

    <div class="row justify-content-sm-center">
        <div class="col-sm-4 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/masque/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-8 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/masque/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<!-- User Study -->
<div>
    <h2 class="mt-5 font-weight-bold">User Study</h2>
    <p>We conducted three user studies to evaluate how people perceive and interpret facial skin stretch feedback with Masque. Participants experienced a series of VR scenarios where tactors delivered controlled directional and intensity-based feedback. We collected both <b>quantitative</b> and <b>qualitative</b> data, including <b>Likert-scale ratings</b> and <b>post-experience interviews</b>, to understand the effectiveness of skin stretch for conveying guidance, motion, and expression. The study was designed to assess intuitiveness, comfort, and the potential for skin stretch to enhance immersion in VR environments.</p>

    <ul>
        <li class="font-weight-bold">EVALUATING PHYSICAL COMFORT</li>
            <ul>
                <li>12 participants (20–27 yrs, HMD experience).</li>
                <li>Most found displacements ≤15 mm acceptable.</li>
                <li>Upward stretch caused breathing issues; average upper limit ~14.2 mm.</li>
                <li>Final reference: 5 mm baseline, usable range 0–10 mm (safe across all participants).</li>
            </ul>
        <li class="font-weight-bold">DISTANCE JND (Just Noticeable Difference)</li>
            <ul>
                <li>3-alternative forced choice with staircase method.</li>
                <li>Average JND ≈ 24.6% at 5 mm baseline (~1.23 mm).</li>
                <li>No significant effect of location or direction → same parameters apply across all tactor sites.</li>
            </ul>
        <li class="font-weight-bold">ANGLE DISCRIMINATION</li>
            <ul>
                <li>Measured perceptual threshold for distinguishing stretch directions.</li>
                <li>Average threshold ≈ 22.7°.</li>
                <li>Parallel-to-skin directions were more sensitive than perpendicular ones.</li>
                <li>At least 8 reliable directions (every ~45°) can be distinguished.</li>
            </ul>
    </ul>

    <div class="row justify-content-sm-center">
        <div class="col-sm-4 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/masque/4.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-4 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/masque/5.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-4 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/masque/6.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>


<!-- Demo Application -->
<div>
    <h2 class="mt-5 font-weight-bold">Demo Application</h2>
    <p>We implemented three applications, all developed using the Unity3D game engine, and are integrated with the VIVE developing environment and tracking system. A set of profiles were created based on our previous study results.</p>

    <ul>
        <li class="font-weight-bold">Application 1: Motorcycle Racing</li>
            <ul>
                <li>Simulated the helmet’s weight</li>
                <li>Inertia during sharp turns</li>
                <li>The sensation of riding on bumpy roads</li>
                <li>Simulate wind pressure</li>
            </ul>
        <li class="font-weight-bold">Application 2: Snowball Fight</li>
            <ul>
                <li>Impact of a direct hit</li>
                <li>The subtle graze of a near miss</li>
            </ul>
        <li class="font-weight-bold">Application 3: Virtual Museum Guidance</li>
            <ul>
                <li>Demonstrating the Masque’s potential for fine-grained directional guidance</li>
            </ul>
    </ul>

    <div class="row justify-content-sm-center">
        <div class="col-sm-4 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/masque/7.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-4 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/masque/8.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-4 mt-3 mt-md-0">
            {% include figure.liquid path="assets/img/masque/9.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<!-- Finding -->
<div>
    <h2 class="mt-5 font-weight-bold">Finding</h2>
    <p>Our study revealed that participants could reliably distinguish different directions and intensities of skin stretch feedback, supporting its potential for directional guidance and motion cues. Users reported that the sensation felt natural and immersive, particularly when paired with visual VR content. Some participants also noted that facial skin stretch could evoke emotional or expressive responses, highlighting its unique potential beyond traditional haptic modalities. At the same time, we identified challenges such as calibration for individual facial differences and ensuring long-term comfort, which point toward directions for future refinement.</p>
</div>

<div>
    <p>For more details, please see our paper
        <a href="/assets/papers/Masque.pdf" class="btn-no-shadow btn btn-sm btn-outline-primary ml-1 ml-md-4 mt-1" target="_blank">
        <i class="fa-solid fa-file-pdf"></i> Download PDF
        </a>
    </p>
</div>
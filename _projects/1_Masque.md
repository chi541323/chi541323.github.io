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
    <!-- image -->
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
        <li class="font-weight-bold">Objective & Method</li>
            <ul>
                <li>An informal exploratory study was conducted to design an optimal shear tactor.</li>
                <li>Two geometric factors were tested: shape (convex, flat, and concave) and size (10mm, 20mm, and 30mm diameters).</li>
                <li>The tactors were covered with a 2mm-thick silicone layer to increase friction and user comfort.</li>
            </ul>
        <li class="font-weight-bold">Task</li>
            <ul>
                <li>The task involved dragging different tactors on their facial skin. Participants rated their preference on a continuous 1-7 scale (7 being most acceptable) without restrictions on the movement's location, direction, or distance.</li>
            </ul>
        <li class="font-weight-bold">Results</li>
            <ul>
                <li><b style="font-weight:900;">Statistical Analysis</b></li>
                Both shape and size were found to have a significant effect on preference scores (p < .001). There was no significant interaction between the two.
                <li><b style="font-weight:900;">Statistical Analysis</b></li>
                The concave-shaped tactors received the highest scores, significantly outperforming both flat and convex shapes. Participants reported that the concave shape better fit the contours of their facial bones and created a clearer sensation of skin stretch. In contrast, the convex shape was the least preferred, as it often caused an unpleasant sensation by pressing against facial bones.
                <li><b style="font-weight:900;">Size Preference</b></li>
                Larger tactors led to higher preference scores. Participants noted that larger tactors created a larger contact area, making the skin stretch feedback easier to perceive. The 10mm tactors were generally considered unacceptable, as they caused a tingling pain.
            </ul>
    </ul>
    <p>Based on the statistical results and participant feedback, the final hardware prototype was designed using <b style="font-weight:900;">30mm-diameter</b>, <b style="font-weight:900;">concave-shaped tactors</b>, which received the highest overall preference rating.</p>
    <!-- image -->
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
                <li>Most found displacements ≤ 15 mm acceptable.</li>
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
    <!-- image -->
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
    <!-- image -->
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
    <!-- evaluation study -->
    <p class="font-weight-bold">User Evalutation Study</p>
    <ul>
        <li class="font-weight-bold">Objective & Method</li>
            <ul>
                <li>This study evaluated whether Masque's facial skin-stretch feedback could enhance the user experience of Head-Mounted Displays (HMDs).</li>
                <li>The study compared user experience with and without haptic feedback.</li>
            </ul>
        <li class="font-weight-bold">Participants & Task</li>
            <ul>
                <li>12 participants (7 female, 5 male, ages 22-26), ten of whom had prior VR experience.</li>
                <li>Participants experienced three applications: Virtual Museum Guidance, Motorcycle Racing, and Snowball Fight.</li>
                <li>After each session, they used a continuous 1-7 scale to rate realism and enjoyment.</li>
            </ul>
        <li class="font-weight-bold">Key Findings</li>
            <ul>
                <li class="font-weight-bold mt-2">Realism</li>
                    <ul>
                        <li class="font-weight-bold">Motorcycle Racing</li>
                        Haptic feedback significantly increased realism scores, with participants feeling that the skin stretch simulated wearing a helmet.
                        <li class="font-weight-bold">Snowball Fight</li>
                        The "graze" profile significantly enhanced realism, helping users react and dodge virtual snowballs. The "freezing" profile had mixed reviews, with some users suggesting a need for multimodal feedback (e.g., thermal or vibration) for a more realistic feel.
                    </ul>
                <li class="font-weight-bold">Enjoyment</li>
                    <ul>
                        <li class="font-weight-bold">Games (Motorcycle Racing & Snowball Fight)</li>
                        All haptic profiles significantly increased enjoyment. Participants felt the feedback made the games more exciting and immersive, even reporting that negative sensations like "freezing" or "grazing" made them feel more competitive.
                        <li class="font-weight-bold">Virtual Museum Guidance</li>
                        Haptic feedback did not significantly increase enjoyment scores. Participants found that while the feedback helped them navigate, long-term skin stretch was sometimes annoying, suggesting a need for user control over the feedback.
                    </ul>
            </ul>
        <div class="row justify-content-sm-center mt-3">
            <div class="col-sm-7 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/masque/11.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
    </ul>

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
---
layout: page
title: Gaiters - Exploring Skin Stretch Feedback on Legs for Enhancing Virtual Reality Experiences
description: Leg-worn devices that generate 2D skin stretch feedback to simulate virtual textures and directional cues. Conducted studies on perceivable stretch and evaluated user experiences. Results show rich and enjoyable haptic feedback on the lower limbs in VR.
img: assets/img/gaiters/gaiters_30.gif
importance: 2
category: Human-Computer Interactions
paper: ACM CHI 20
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
    <ul>
        <li class="font-weight-bold">Objective</li>
            <ul>
                <li>To explore how combining leg actions with skin stretch profiles can induce different perceptions.</li>
                <li>The study evaluated four perceptions: Pulling Force, Weight, Rotational Force, and Friction.</li>
            </ul>
        <li class="font-weight-bold">Study Design</li>
            <ul>
                <li class="font-weight-bold">Leg Actions</li>
                Participants performed three common VR actions: Standing, Walking, and Kicking.
                <li class="font-weight-bold">Skin Stretch Profiles</li>
                Six directional profiles were tested: Upward, Downward, Forward, Backward, Leftward, and Rightward.
                <li class="font-weight-bold">Perception Assessment</li>
                Participants experienced each action-stretch combination and gave a binary "Yes" or "No" response as to whether it successfully induced a specific perception.
            </ul>
        <li class="font-weight-bold">Key Finding</li>
            <ul>
                <li class="font-weight-bold">Pulling Force</li>
                Downward or Backward stretches during Standing or Walking were highly effective at inducing a pulling sensation (over 70% agreement). However, during a Kicking motion, the same stretches were perceived as an impact or acceleration force, suggesting that complex muscle movements interfere with the perception of skin stretch.
                <li class="font-weight-bold">Leg Weight</li>
                Upward stretches made legs feel lighter, while Downward stretches made them feel heavier during standing or walking. For kicking, upward and backward stretches enhanced the feeling of leg weight.
                <li class="font-weight-bold">Rotational Force</li>
                Leftward and Rightward stretches only created a clear rotational force sensation when participants were standing still. The sensation weakened significantly as leg actions became more dynamic.
                <li class="font-weight-bold">Friction</li>
                All combinations were highly effective at simulating friction (over 70% agreement). Participants described the sensation as feeling "water splashing," "swimming fish," or "crawling insects."
            </ul>
        <div class="row justify-content-sm-center mt-3">
            <div class="col-sm mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/gaiters/7.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
    </ul>
</div>


<!-- Demo Application -->
<div>
    <h2 class="mt-5 font-weight-bold">Demo Application</h2>
    <p>A user study with 16 participants assessed how effectively the gaiters conveyed direction, intensity, and realism of feedback in VR. Participants engaged in locomotion-related VR tasks with and without haptic feedback, allowing comparison of perceived immersion, guidance, and naturalness of experience.</p>
    <!-- image -->
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
                    <li class="font-weight-bold mt-5">Application 2: Fancy Goal Game</li>
                        <ul>
                            <li>Frontal impact</li>
                            <li>Side impact</li>
                            <li>Acceleration force</li>
                        </ul>
                </ul>
        </div>
    </div>
    <p class="font-weight-bold mt-3"> User Evaluation Study</p>
    <ul>
        <li class="font-weight-bold">Objective</li>
            <ul>
                <li>This study evaluated the value of Gaiters, a leg-worn skin-stretch feedback system, by comparing user experience with and without haptic feedback.</li>
            </ul>
        <li class="font-weight-bold">Task</li>
            <ul>
                <li>12 participants (6 females, ages 20-26), all with prior VR experience but no experience with leg-worn haptic devices.</li>
                <li>They experienced two applications: a Horror Escape Game and a Fancy Goal Game.</li>
                <li>After each session, participants rated their perceived Realism and Enjoyment on a 1-7 scale.</li>
            </ul>
        <li class="font-weight-bold">Key Finding</li>
            <ul>
                <li class="font-weight-bold">Horror Escape Game</li>
                    <ul>
                        <li class="font-weight-bold">Realism</li>
                        Haptic feedback significantly increased realism scores. Participants found that haptics were more noticeable than visual or audio cues during moments of fear, with some reporting they wouldn't have known about a zombie attack without the haptic feedback.
                        <li class="font-weight-bold">Enjoyment</li>
                        Haptics significantly increased enjoyment, as participants found the game more thrilling and exciting. However, one user found the feedback distracting, suggesting that VR applications should give users control over haptic feedback.
                    </ul>
                <li class="font-weight-bold">Fancy Goal Game</li>
                    <ul>
                        <li class="font-weight-bold">Realism & Enjoyment</li>
                        Haptic feedback significantly increased both realism and enjoyment. Participants noted that directional cues from the legs helped them feel the ball's path, enhancing immersion.
                        <li class="font-weight-bold">Design Implication</li>
                        A participant suggested that stronger skin-stretch stimuli could further enhance the realism of actions like a curve shot, indicating a need for improved mechanical design.
                    </ul>
            </ul>
        <p class="mt-3">Leg-worn skin-stretch is a valuable addition to VR, significantly enhancing realism and enjoyment by providing situational awareness and complementing visual and audio cues, especially in high-intensity situations. Future designs should focus on improving tactor coverage and feedback strength while also giving users control over the feedback.</p>
        <div class="row justify-content-sm-center mt-3">
            <div class="col-sm-8 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/gaiters/9.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
    </ul>
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

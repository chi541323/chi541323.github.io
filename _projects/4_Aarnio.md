---
layout: page
title: Aarnio - Passive Kinesthetic Force Output for Foreground Interactions on an Interactive Chair
description: A new type of haptic output for foreground interactions on an interactive chair, where input is carried out explicitly in the foreground of the user’s consciousness, modulating resistive forces when rotating, tilting, or rolling the chair. Conducted studies to determine recognizability of five force profiles. Results demonstrate novel interaction techniques for immersive VR and ubiquitous computing environments.
img: assets/img/Aarnio/Aarnio_30.gif
importance: 4
category: Human-Computer Interactions
paper: ACM CHI 19
author: Shan-Yuan Teng, Da-Yuan Huang, <span class="my-color-b" style='font-weight:900;'>Chi Wang</span>, Jun Gong, Teddy Seyed, Xing-Dong Yang, Bing-Yu Chen
---

A new type of haptic output for foreground interactions on an interactive chair, where input is carried out explicitly in the foreground of the user’s consciousness, modulating resistive forces when rotating, tilting, or rolling the chair. Conducted studies to determine recognizability of five force profiles. Results demonstrate novel interaction techniques for immersive VR and ubiquitous computing environments.

<div class="embed-responsive embed-responsive-16by9 mb-3">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/kFls3r3qJz8?si=l2hPEYAyy0dQcPf8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

<!-- Motivation -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Motivation</h2>
    <div class="row align-items-center">
        <!-- 左邊文字 -->
        <div class="col-md-7">
            <p style="text-align: justify;">Existing haptic interactive chairs focus on subtle, background interactions like posture correction. We argue there is a significant opportunity in exploring haptic output for foreground interactions—where the feedback is directly linked to a user's conscious input. This approach can unlock new applications and enhance the user experience by tightly coupling physical movement with a chair's response. In this work, we propose passive kinesthetic force output for user’s explicit input via rotating, tilting, and rolling the chair.</p>
        </div>
        <!-- 右邊圖片 -->
        <div class="col-md-5">
            {% include figure.liquid path="assets/img/Aarnio/1.png" title="example image" class="img-fluid rounded z-depth-1 w-100"%}
        </div>
    </div>
</div>

<!-- Design -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Design</h2>
        <ul class="mt-3">
            <!-- Kinesthetic Force Feedback -->
            <li><b class="my-color-b" style="font-weight:900;">Kinesthetic Force Feedback</b></li>
            <p>Haptic feedback comes in two main types: tactile (vibrations felt by the skin) and kinesthetic (force felt by muscles and joints). Our project focuses on kinesthetic force feedback, specifically the passive type, which resists a user's motion. This differs from active feedback, which pushes or pulls the user. By using this passive, resistive force, our system directly responds to a user's explicit movements, making it a powerful tool for intentional, foreground interactions.</p>
            <!-- Interaction Design Space -->
            <li><b class="my-color-b" style="font-weight:900;">Interaction Design Space</b></li>
            <p>We focused on a standard swivel office chair, which offers a rich design space for foreground interactions. Our research targeted key components where user input is explicit and intentional. To elicit initial user preferences on the discussed chair interactions, we conducted an informal exploratory study.</p>
            <div class="row justify-content-sm-center">
                <div class="col-sm-6 mt-3 mt-md-0">
                    {% include figure.liquid path="assets/img/Aarnio/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
                </div>
            </div>
                <ul>
                    <!-- Components -->
                    <li><b class="my-color-b" style="font-weight:900;">Components:</b></li>
                    <ul>
                        <li><b class="my-color-b" style="font-weight:900;">Seat:</b> Modifying the natural resistance when rotating, sliding, or tilting the seat to provide dynamic feedback.</li>
                        <li><b class="my-color-b" style="font-weight:900;">Backrest:</b> Adjusting the tension of the backrest to provide information as a user reclines.</li>
                        <li><b class="my-color-b" style="font-weight:900;">Armrest & Headrest:</b> Using the natural mechanical resistance of these components to offer additional channels for haptic output.</li>
                        <li><b class="my-color-b" style="font-weight:900;">Casters:</b> Modulating the friction of the wheels to provide feedback while rolling.</li>
                    </ul>
                    <!-- Methodology -->
                    <li class="mt-2"><b class="my-color-b" style="font-weight:900;">Methodology:</b></li>
                    <ul>
                        <li>Participants were introduced to the study goals,and they were shown sketches of all possible chair movements (pitch, roll, yaw, and x/y/z axis translations).</li>
                        <li>For each of the six degrees of freedom across the seat, backrest, headrest, armrests, and casters, participants gave a binary 'YES' or 'NO' response to indicate whether they would prefer to use that movement for interactive tasks. This binary scale was used to avoid survey bias.</li>
                        <li>Participants were asked about their preferences for receiving feedback from the chair in response to their unplanned or unintentional movements (implicit input).</li>
                    </ul>
                    <!-- Results -->
                    <li class="mt-2"><b class="my-color-b" style="font-weight:900;">Results:</b></li>
                        <ul>
                            <li><b class="my-color-b" style="font-weight:900;">High-Potential Interactions:</b> Rotating, tilting, and rolling were the top-ranked movements, as they were well-balanced for both explicit and implicit input.</li>
                            <ul>
                                <li><b class="my-color-b" style="font-weight:900;">Tilting the backrest:</b> Over 65% of participants preferred this action, describing it as "physically effortless" and "natural to perform."</li>
                                <li><b class="my-color-b" style="font-weight:900;">Rolling the chair:</b> This was preferred more for implicit input than explicit, as participants often make these movements unconsciously to adjust for comfort.</li>
                                <li><b class="my-color-b" style="font-weight:900;">Rotating the seat:</b> This was preferred more for explicit input, as participants found it unlikely to rotate the seat unintentionally.</li>
                            </ul>
                             <li><b class="my-color-b" style="font-weight:900;">Other Findings:</b></li>
                            <ul>
                                <li><b class="my-color-b" style="font-weight:900;">Armrest rotation: </b> Considered suitable only for explicit input.</li>
                                <li><b class="my-color-b" style="font-weight:900;"> Vertical seat movement:</b> Found to be suitable only for implicit input, as it naturally provides haptic information when a user sits down.</li>
                            </ul>
                        </ul>
                    <!-- Conclusion -->
                    <li class="mt-2"><b class="my-color-b" style="font-weight:900;">Conclusion:</b></li>
                    Based on these results, we chose to focus on rotation, tilting, and rolling as the primary interactions for this work.
                </ul>
        </ul>
        <!-- image -->
        <div class="row justify-content-sm-center">
            <div class="col-sm-6 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/Aarnio/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
</div>

<!-- Prototype -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Prototype</h2>
        <p>Based on the results of the informal study, we created a prototype to demonstrate the proposed haptic output. Our prototype was created by augmenting the <b class="my-color-b" style="font-weight:900;">seat</b>, <b class="my-color-b" style="font-weight:900;">backrest</b>, and <b class="my-color-b" style="font-weight:900;">caster</b> of the Swivel office chair. We extended the natural resistive forces of the joints of the chair using carefully designed braking and tilt tension controlling systems.</p>
        <!-- image -->
        <div class="row justify-content-sm-center">
            <div class="col-sm-4 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/Aarnio/4.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class="col-sm-4 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/Aarnio/5.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class="col-sm-4 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/Aarnio/6.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
        <!-- profiles -->
        <p class="mt-3">To demonstrate the capabilities of the proposed passive kinesthetic force output, we designed and implemented five force profiles for each of the three chair interactions supported by our prototype.</p>
        <ul>
            <li><b class="my-color-b" style="font-weight:900;">Profiles for Rotating the Seat:</b></li>
                <ul>
                    <li><b class="my-color-b" style="font-weight:900;">Natural Resistance: </b></li>
                    This profile provides the chair's inherent light friction, without any added resistance from the haptic system.
                    <li><b class="my-color-b" style="font-weight:900;">Strong Resistance: </b></li>
                    This profile applies a significant resistive force, requiring user effort to overcome, which can be used to encode different events or information.
                    <li><b class="my-color-b" style="font-weight:900;">Lock: </b></li>
                    This profile completely locks the seat in place, preventing rotation and signaling a stop or boundary to the user.
                    <li><b class="my-color-b" style="font-weight:900;">Ramp-Down: </b></li>
                    This profile gradually decreases the applied braking force as the user rotates, making the movement feel easier over time and aiding with continuous control.
                    <li><b class="my-color-b" style="font-weight:900;">Click: </b></li>
                    This profile alternates between natural and strong resistance to create a "clicking" sensation, which can encode discrete information or guide users to specific targets.
                </ul>
            <li><b class="my-color-b" style="font-weight:900;">Profiles for Tilting the Backrest:</b></li>
                <ul>
                    <li><b class="my-color-b" style="font-weight:900;">Minimum Tension: </b></li>
                    The backrest offers the lowest resistance, making it effortless for the user to initiate a recline.
                    <li><b class="my-color-b" style="font-weight:900;">Low Tension: </b></li>
                    This profile applies a slightly increased resistance, requiring more user effort to tilt the backrest compared to the minimum setting.
                    <li><b class="my-color-b" style="font-weight:900;">High Tension:</b></li>
                    The backrest requires significant effort to tilt, providing a firm resistance due to a highly compressed spring.
                    <li><b class="my-color-b" style="font-weight:900;">Maximum Tension: </b></li>
                    The backrest is locked in a straight-up position, offering almost no ability for the user to recline.
                    <li><b class="my-color-b" style="font-weight:900;">Tension Ramp-Down: </b></li>
                    The resistance to reclining gradually decreases as the user tilts the backrest further, making the movement feel easier over time.
                </ul>
            <li><b class="my-color-b" style="font-weight:900;">Profiles for Rolling the Chair:</b></li>
                <ul>
                    <li><b class="my-color-b" style="font-weight:900;">Natural Resistance: </b></li>
                    The chair rolls with its inherent friction, as no wheels are locked by the system.
                    <li><b class="my-color-b" style="font-weight:900;">Strong Resistance: </b></li>
                    The chair resists movement with an average force of 25.5 N by locking two wheels.
                    <li><b class="my-color-b" style="font-weight:900;">Lock: </b></li>
                    This profile completely immobilizes the chair by locking all five wheels, resisting an average force of 42 N.
                    <li><b class="my-color-b" style="font-weight:900;">Ramp-Down: </b></li>
                    The chair starts with a high resistance from four locked wheels, which then gradually decreases as the wheels are unlocked one by one.
                    <li><b class="my-color-b" style="font-weight:900;">Click: </b></li>
                    The chair provides a repeated clicking sensation by locking and releasing three wheels for every 60 mm it rolls.
                </ul>
        </ul>
</div>

<!-- User Study -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">User Study</h2>
    <p>We considered it important to understand whether the force profiles are recognizable by users, with the answer determining whether this new output channel can be effectively used for various application tasks. Thus, our goal for this study was to examine how well participants could perceive and distinguish the proposed force profiles using our implementation. </p>
    <ul>
        <li><b class="my-color-b" style="font-weight:900;">Experimental Method</b></li>
            <ul>
                <li><b class="my-color-b" style="font-weight:900;">Tasks:</b></li>
                    <ul>
                        <li><b class="my-color-b" style="font-weight:900;">Primary Task:</b> Participants were asked to identify the force profiles presented through reclining, rotating the seat, or rolling the chair. They could repeat the movement as many times as needed but were not allowed to reverse the motion.</li>
                        <li><b class="my-color-b" style="font-weight:900;">Secondary Task (Cognitive Load):</b> In half the trials, participants performed a modified Stroop test to simulate a distracted state. They had to maintain over 90% accuracy by counting the number of times a word's text and font color matched.</li>
                    </ul>
                <li><b class="my-color-b" style="font-weight:900;">Experimental Design:</b></li>
                    <ul>
                        <li>The study used a 2 x 5 within-subject factorial design with two independent variables: "Cognitive Task" (Load/No Load) and "Force Profile" (five profiles).</li>
                        <li>Each study involved 80 trials per participant (2 Cognitive Tasks x 5 Force Profiles x 8 Repetitions).</li>
                    </ul>
                 <li><b class="my-color-b" style="font-weight:900;">Measures:</b></li>
                    <ul>
                        <li><b class="my-color-b" style="font-weight:900;">Recognition Accuracy:</b> The number of correctly identified force profiles.</li>
                        <li><b class="my-color-b" style="font-weight:900;">Response Time:</b> The time from the start of the force profile to the key press.</li>
                        <li><b class="my-color-b" style="font-weight:900;">Number of Attempts: </b> The number of tries needed to identify a profile.</li>
                        <li><b class="my-color-b" style="font-weight:900;">Questionnaire: </b> After each study, participants rating the recognizability of the profiles on a continuous 1-7 scale.</li>
                    </ul>
            </ul>
        <li><b class="my-color-b" style="font-weight:900;">Results:</b></li>
            <ul>
                <li><b class="my-color-b" style="font-weight:900;">Profile Recognition Accuracy:</b></li>
                    <ul>
                        <li><b class="my-color-b" style="font-weight:900;">Rotation: </b>The force profiles were highly recognizable (93.8% accuracy). The Lock and Click profiles were the easiest to identify, while Ramp-Down was the most confusing. Cognitive load had no significant impact.</li>
                        <li><b class="my-color-b" style="font-weight:900;">Tilt: </b>Recognition was slightly more challenging (87.3% accuracy) and was significantly affected by cognitive load. Participants had difficulty distinguishing between similar tension levels.</li>
                        <li><b class="my-color-b" style="font-weight:900;">Rolling: </b>The profiles were highly recognizable (93.0% accuracy). Click had the highest accuracy, while Strong Resistance was the most confusing. Cognitive load had no significant impact.</li>
                    </ul>
                <li><b class="my-color-b" style="font-weight:900;">Response Time:</b></li>
                    <ul>
                        <li><b class="my-color-b" style="font-weight:900;">Average Times: </b>Rotation (4.25s), Tilt (6s), and Rolling (3.74s).</li>
                        <li><b class="my-color-b" style="font-weight:900;">Rotation and Rolling: </b>Click was the fastest to recognize, thanks to its distinct haptic landmark. Strong Resistance was the slowest.</li>
                        <li><b class="my-color-b" style="font-weight:900;">Counterintuitive Finding: </b>Under cognitive load, participants’ response times were significantly faster for both rotation and rolling. They reported speeding up to finish the cognitive task more quickly, but this did not compromise their accuracy.</li>
                    </ul>
                <li><b class="my-color-b" style="font-weight:900;">Number of Attempts & Subjective Ratings:</b></li>
                    <ul>
                        <li><b class="my-color-b" style="font-weight:900;">Number of Attempts: </b>Participants were highly confident in their answers, requiring an average of only 1.05 to 1.06 attempts to correctly identify a profile. Neither the cognitive load nor the force profile significantly affected the number of attempts.</li>
                        <li><b class="my-color-b" style="font-weight:900;">Subjective Ratings: </b>Participants' subjective ratings of recognizability were consistent with the quantitative accuracy results, confirming that they had a reliable sense of how easy or difficult each profile was to distinguish.</li>
                    </ul>
            </ul>
            <!-- image -->
            <div class="row justify-content-sm-center mt-3">
                <div class="col-sm-7 mt-3 mt-md-0">
                    {% include figure.liquid path="assets/img/Aarnio/7.png" title="example image" class="img-fluid rounded z-depth-1" %}
                </div>
                <div class="col-sm-5 mt-3 mt-md-0">
                    {% include figure.liquid path="assets/img/Aarnio/8.png" title="example image" class="img-fluid rounded z-depth-1" %}
                </div>
            </div>
    </ul>
</div>

<!-- Demo Application -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Demo Application</h2>
    <p>We implemented several applications to demonstrate the capabilities of Aarnio. Each application was designed through a participatory design workshop with people with varying backgrounds and physical capabilities. We brainstormed with our participants about their needs and limitation of the current office chair and how Aarnio can help.</p>
    <div class="row justify-content-sm-center mt-3">
        <div class="col-sm-5 mt-3 mt-md-0">
            <div class ="mt-2">
                {% include figure.liquid path="assets/img/Aarnio/9.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class ="mt-4">
            {% include figure.liquid path="assets/img/Aarnio/10.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class ="mt-4">
            {% include figure.liquid path="assets/img/Aarnio/11.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
        <div class="col-sm-7 mt-3 mt-md-0">
            <ul>
                <li><b class="my-color-b" style="font-weight:900;">On-demand Information Acquisition</b></li>
                Aarnio provides a discreet, hands-on alternative to smartphone notifications, allowing users to query information by rotating, tilting, or rolling their chair. This offers a way to check information, such as the time until a meeting, in social situations without appearing to be distracted by a device.
                <li><b class="my-color-b" style="font-weight:900;">Hands-free Interactions</b></li>
                Our system enables users to interact with applications when their hands are busy. For example, a user can rotate the chair to input calorie ranges in a fitness app or adjust settings in a music program, providing a seamless and hygienic interaction method.
                <li><b class="my-color-b" style="font-weight:900;">Gaming</b></li>
                Haptic feedback from the chair creates a more immersive gaming experience. We implemented force feedback to simulate vehicle damage in a driving game or to provide a "bumpy road" sensation for a racing game, enhancing the player's physical connection to the virtual world.
                <li><b class="my-color-b" style="font-weight:900;">Interaction Techniques for People with Disabilities</b></li>
                Our system offers a new interaction method for people with motor or visual impairments. The chair's force feedback can guide users through menu items or allow them to query information, providing a faster and more accessible way to complete tasks that would otherwise be difficult.
            </ul>
        </div>
    </div>
</div>

<!-- Finding -->
<div>
    <h2 class="mt-5 font-weight-bold my-color-b">Finding</h2>
        <p>We propose passive kinesthetic force output on an interactive chair by modulating the natural resistive forces of rotation, tilt, and rolling. Through a prototype and three user studies, participants distinguished force profiles with high accuracy (up to 93.75%). Beyond technical validation, this approach enables hands-free interactions in everyday life, such as controlling media, browsing content, or operating applications while reading, eating, or holding objects. It offers an alternative interaction paradigm that emphasizes comfort, accessibility, and convenience, pointing toward new directions in interactive furniture and smart IoT systems.</p>
</div>

<div>
    <p>For more details, please see our paper
        <a href="/assets/papers/Aarnio.pdf" class="btn-no-shadow btn btn-sm btn-outline-primary ml-1 ml-md-4 mt-1" target="_blank">
        <i class="fa-solid fa-file-pdf"></i> Download PDF
        </a>
    </p>
</div>
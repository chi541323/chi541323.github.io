---
layout: page
title: PuPoP - Pop-up Prop on Palm for Virtual Reality
description: A lightweight pneumatic palm interface that pops airbags with predefined shapes to simulate grasping virtual objects. Conducted user studies on shape perception and VR interaction. Results show that dynamic PuPoP enhances realism and enjoyment in VR object manipulation.
img: assets/img/PuPoP/PuPoP_30.gif
importance: 3
category: Human-Computer Interactions
paper: ACM UIST 18
author: Shan-Yuan Teng, Tzu-Sheng Kuo, <span style='font-weight:900;'>Chi Wang</span>, Chi-huan Chiang, Da-Yuan Huang, Liwei Chan, Bing-Yu Chen
---

A lightweight pneumatic palm interface that pops airbags with predefined shapes to simulate grasping virtual objects. Conducted user studies on shape perception and VR interaction. Results show that dynamic PuPoP enhances realism and enjoyment in VR object manipulation.

<div class="embed-responsive embed-responsive-16by9 mb-3">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/UpWDa-jgC-I?si=ubBVXP-DD5O_WKbA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

<!-- Motivation -->
<div>
    <h2 class="mt-5 font-weight-bold">Motivation</h2>

    <p>Haptic feedback in VR often relies on vibration or external devices, which cannot fully simulate the sensation of holding physical objects. Many interactions in VR involve grasping, touching, or manipulating items, yet providing realistic haptic cues for these actions remains challenging. PuPoP was motivated by the desire to explore palm-based haptic feedback that can create tangible, on-demand props directly in the user’s hand, without requiring the user to hold external hardware throughout the experience.</p>

    <div class="row">
        <div class="col-sm mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/PuPoP/1.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<!-- Design -->
<div>
    <h2 class="mt-5 font-weight-bold">Design Prototype</h2>
        <p>PuPoP is a wearable system that mounts small foldable props on the palm, which can “pop up” when needed in VR.</p>
        <ul>
            <li><b style="font-weight:900;">Mechanism:</b> The system consists of thin, lightweight structures that fold flat when not in use and expand into different shapes (e.g., sphere, cylinders, box) using a pop-up mechanism.</li>
            <li><b style="font-weight:900;">Customization:</b> Different prop shapes can be mounted on the palm to simulate a variety of virtual objects.</li>
            <li><b style="font-weight:900;">Interaction:</b> By aligning the props with VR visual cues, users perceive the props as virtual objects, creating a stronger sense of presence.</li>
            <li><b style="font-weight:900;">Comfort:</b>The device was designed to be low-profile and lightweight so that it does not interfere with natural hand movement when props are not deployed.</li>
        </ul>

        <div class="row justify-content-sm-center">
            <div class="col-sm-4 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/PuPoP/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class="col-sm-4 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/PuPoP/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class="col-sm-4 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/PuPoP/4.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
</div>

<!-- System Design & Implementation -->
<div>
    <h2 class="mt-5 font-weight-bold">System Design & Implementation</h2>
        <p>PuPoP is a wearable system that mounts small foldable props on the palm, which can “pop up” when needed in VR.</p>
        <ul>
            <li><b style="font-weight:900;">Props on Palm</b></li>
                Props are mounted on the palm using a fabric strap with hook-and-loop fasteners, making them easily attachable/detachable for switching between VR applications.
            <li><b style="font-weight:900;">Prop Stacking</b></li>
                Multiple props can be stacked to support more complex VR tasks. Stacking follows two rules:
                <ul>
                    <li>Props must have similar flattened dimensions.</li>
                    <li>Props are stacked in the order of box → cylinder → sphere, minimizing interference.</li>
                    <li>A deflation system ensures that smaller props remain flat when larger props inflate.</li>
                </ul>
            <li><b style="font-weight:900;">Prop Extension</b></li>
                To enable thumb-and-finger grasping (pad-opposite grasp), props can be extended off the palm using:
                <ul>
                    <li>Parallel extension: A small box airbag lifts the prop upward.</li>
                    <li>Tilt extension: A triangular airbag tilts the prop, allowing pen-like interactions.</li>
                </ul>
            <li><b style="font-weight:900;">Prop Sensing & Finger Operation</b></li>
                <ul>
                    <li>Hand tracking: Leap Motion is used for palm/finger tracking when props are deflated.</li>
                    <li>Touch sensing: Flexible FSR sensors are attached to props, detecting grasp, press, and squeeze events.</li>
                    <li>Force interaction: Sensor data allows the system to infer applied force without recalibration.</li>
                </ul>
            <li><b style="font-weight:900;">Object Properties Emulation</b></li>
                Using pneumatic actuation, props can emulate stiffness, elasticity, and pulsation. For example, inflation patterns simulate a heartbeat, while controlled air pressure creates variable stiffness.
            <li><b style="font-weight:900;">Incorporation into VR</b></li>
                Integrated with HTC Vive + Leap Motion in Unity 3D. Two grasping modes were developed:
                <ul>
                    <li>Natural Grasp: Props inflate just before contact so users can grasp fully-formed props aligned with virtual objects.</li>
                    <li>Magic Grasp: Inspired by Star Wars “Force pull,” users can summon objects from a distance with an open-hand gesture; the corresponding prop inflates automatically.</li>
                </ul>
        </ul>
        <div class="row justify-content-sm-center">
            <div class="col-sm-6 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/PuPoP/5.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class="col-sm-6 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/PuPoP/6.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
        <div class="row justify-content-sm-center">
            <div class="col-sm-6 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/PuPoP/7.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
</div>

<!-- Demo Application -->
<div>
    <h2 class="mt-5 font-weight-bold">Demo Application</h2>
        <p>Two fantasy VR applications with different scenarios of object manipulation have been created to demonstrate the aforementioned designs of PuPoP.</p>
        <ul>
            <li><b style="font-weight:900;">Quidditch Sports Training</b></li>
                <ul>
                    <li>Inspired by the Harry Potter game Quidditch.</li>
                    <li>Players wear two spherical props of different sizes (via prop stacking).</li>
                    <li>Scoring methods:</li>
                        <ul>
                            <li>Pick up balls (big sphere) from a red box and throw them into hoops.</li>
                            <li>Catch the flying Golden Snitch (small sphere) to double the score.</li>
                        </ul>
                    <li>Uses natural grasp: props inflate when approaching a ball and deflate when releasing.</li>
                </ul>
            <li><b style="font-weight:900;">Magic Brush Painting</b></li>
                <ul>
                    <li>A 3D drawing app.</li>
                    <li>Players use a cylindrical prop (brush) and a box prop (eraser) mounted on the palm (prop stacking).</li>
                    <li>The eraser supports prop extension for natural pad-opposite grasp.</li>
                    <li>Equipped with FSR sensors: strokes/erasures are triggered when grasping force exceeds a threshold.</li>
                    <li>Tools are obtained via magic grasp: aiming at a tool with the palm for one second inflates the corresponding prop.</li>
                </ul>
        </ul>
        <div class="row justify-content-sm-center">
            <div class="col-sm-6 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/PuPoP/8.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class="col-sm-6 mt-3 mt-md-0">
                {% include figure.liquid path="assets/img/PuPoP/9.png" title="example image" class="img-fluid rounded z-depth-1" %}
            </div>
        </div>
</div>

<!-- User Study -->
<div>
    <h2 class="mt-5 font-weight-bold">User study</h2>
        <p>The studies focused on whether users could recognize shapes, how natural the interactions felt, and how much the haptic props improved presence in VR.</p>
        <ul>
            <!-- study 1-->
            <li><b style="font-weight:900;">Visual Size Acceptance Range</b></li>
            <ul>
                <li><b style="font-weight:900;">Goal</b></li>
                <ul>
                    <li>Test whether PuPoP can exploit visuo-haptic illusions so one fixed-size prop can represent multiple virtual objects of varying sizes.</li>
                </ul>
                <li><b style="font-weight:900;">Experimental Design</b></li>
                <ul>
                    <li>Props: 9 total (3 primitive shapes × 3 sizes) and only size was varied (not texture, color, or shape details).</li>
                    <li>Medium size props were chosen to fit most hands; smaller/larger props differed by ±1 cm.</li>
                    <li>Used an adaptive staircase method (one-up-one-down) to find upper and lower bounds of acceptable visual sizes.</li>
                    <li>PuPoP mounted on palm (not visible to participant) and participants grasped props and judged whether visual size matched haptic size</li>
                </ul>
                <li><b style="font-weight:900;">Results & Observations</b></li>
                <ul>
                    <li>Acceptance ranges overlapped across prop sizes → a small set of physical props can cover a wide range of virtual sizes.</li>
                    <li>On average:</li>
                        <ul>
                            <li>Lower bounds ≈ 3.5% larger than actual prop size.</li>
                            <li>Upper bounds ≈ 36.2% larger than actual prop size.</li>
                        </ul>
                    <li>PuPoP can effectively serve as physical counterparts for a broad spectrum of virtual object sizes.</li>
                    <li>Findings provide design insights for on-body proxy interfaces; further research is needed to optimize mounting positions and parameters.</li>
                </ul>
            </ul>
            <div class="row justify-content-sm-center mt-3">
                <div class="mt-3 mt-md-0">
                    {% include figure.liquid path="assets/img/PuPoP/10.png" title="example image" class="img-fluid rounded z-depth-1" %}
                </div>
            </div>
            <!-- study 2-->
            <li><b style="font-weight:900;">VR Enjoyment & Object Realism</b></li>
            <ul>
                <li><b style="font-weight:900;">Goal</b></li>
                <ul>
                    <li>Investigate whether PuPoP increases enjoyment and object realism in VR compared to two baselines: (1) HTC VIVE Controller (2) Free-hand manipulation (Leap Motion)</li>
                </ul>
                <li><b style="font-weight:900;">Experimental Design</b></li>
                <ul>
                    <li>Quidditch Sports Training → throwing balls, catching Golden Snitch</li>
                    <ul>
                        <li>Small sphere prop for 50–60mm balls</li>
                        <li>Large sphere prop for 70–80mm balls</li>
                    </ul>
                    <li>Magic Brush Painting → drawing and erasing strokes</li>
                        <ul>
                            <li>Different shape prop (cylinder, box)</li>
                        </ul>
                    <li>Gestures consistent across interfaces:</li>
                        <ul>
                            <li>VIVE: grip button for grasp/release</li>
                            <li>Free-hand: Leap Motion detects grasp/open</li>
                            <li>Free-hand: Leap Motion detects grasp/open</li>
                        </ul>
                    <li>Each participant tested all 3 interfaces (counter-balanced order) and rated enjoyment and object realism on 7-point Likert scale + interview</li>
                </ul>
                <li><b style="font-weight:900;">Results (ANOVA analysis)</b></li>
                <ul>
                    <li>Quidditch:</li>
                        <ul>
                            <li>PuPoP > VIVE controller and Free-hand, no significant diff. between controller vs. free-hand</li>
                            <li>Participants praised natural grasp & haptic realism of PuPoP</li>
                        </ul>
                    <li>Quidditch:</li>
                        <ul>
                            <li>Object Realism: PuPoP and VIVE > Free-hand, no significant diff. PuPoP vs. VIVE realism</li>
                            <li>Enjoyment: no significant diff. across all interfaces</li>
                            <li>PuPoP realism: flexible shape change (brush/eraser), but “too soft” complaints</li>
                            <li>VIVE realism: rigid feel, matched brush expectations</li>
                            <li>Free-hand realism: lowest, awkward grasping posture without proxy</li>
                        </ul>
                </ul>
            </ul>
            <div class="row justify-content-sm-center mt-3">
                <div class="mt-3 mt-md-0">
                    {% include figure.liquid path="assets/img/PuPoP/11.png" title="example image" class="img-fluid rounded z-depth-1" %}
                </div>
            </div>
        </ul>
</div>

<!-- Finding -->
<div>
    <h2 class="mt-5 font-weight-bold">Finding</h2>
        <p>Overall, the studies demonstrated that PuPoP successfully enables palm-mounted inflatable props to serve as versatile physical counterparts for virtual objects in VR. The system effectively leveraged visuo-haptic illusions, allowing a small set of physical props to represent a wide range of virtual sizes. Through prop stacking and extensions, PuPoP supported more complex grasping interactions beyond simple palm-opposite grasps, while the integration of sensing and pneumatic actuation enabled realistic emulation of object properties such as stiffness, weight, and pulsation. User studies showed that participants could accept size variations and interact naturally with the props, validating PuPoP as an effective and flexible on-body proxy interface for enhancing immersion in VR.</p>
</div>
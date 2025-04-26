---
layout: default
---

<div class="double-column-container">
  <video autoplay muted controls>
    <source src="assets/videos/dashes.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <video autoplay muted controls>
    <source src="assets/videos/pulls.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>

# Abstract
Having a well-rounded fixed leg design for a quadruped inevitably limits performance across diverse tasks, while tunability enables specialization and leads to better performance. We introduce a sub-500-gram quadruped robot with a rich leg design space. Reinforcement learning is used to train a locomotion policy that works across designs and exploits their unique dynamics. It also enables mapping from designs to task performance, where interpretable and insightful performance trends and design principles emerge. 

With two papers, we showcase the proposed methdos in selecting leg designs for two distinct tasks: pure locomotion, such as running and turning, and force-based locomotion, such as pulling, pushing, and carrying payloads.

The fast running design reaches a maximum speed of 0.7 m/s or 5.4 body-lengths per second, and the efficient design has a cost of transport of 0.3. The top performer in pulling walks at 0.5 body-lengths per second while exerting a force that is almost 60% of its weight.

# Tunable Legs
The proposed leg design has a range of tunable design parameters, including leg length, foot travel, transmission ratio, and passive parallel and series stiffness. Thanks to  laminate design and fabrication techniques, it is also straightforward to model, low-cost, and fast to manufacture. Its feasible leg design space can be spanned with a "flood fill" algorithm. 400 designs were generated and 6 designs were made. 

![tunable legs](assets/images/legs.png)

# Design-aware Policies
The locomotion policies observe leg designs. Curriculum strategies, also similar to "flood fill", are employed to gradually increase the task difficulties, so that each design's physical limits can be identified and reached. 

<div class="double-column-container">
  <video muted controls>
    <source src="assets/videos/loc_sims.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <video muted controls>
    <source src="assets/videos/forced_loc_sims.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>

# Trend Discoveries
With the learned polices, performance can be evaluated in simulation and analyzed against design parameters. Two most notable trends are: there is an optimum passive series stiffness for locomotion, and the longer the legs the more efficient the locomoiton. Although these trends have been discovered in biomechanics or robotics, we believe they showcase the potential our proposed methods in discovering robot design principles while considering their controls. 

<div class="double-column-container">
  <img src="assets/images/vx_trend.png" alt="vx trend">
  <img src="assets/images/cot_trend.png" alt="cot trend">
</div>

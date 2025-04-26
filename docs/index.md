---
layout: default
---

<div class="teaser">
  <video autoplay muted controls>
    <source src="assets/videos/dashes.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <video autoplay muted controls>
    <source src="assets/videos/pulls.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>

Having a well-rounded fixed leg design for a quadruped inevitably limits performance across diverse tasks, while tunability enables specialization and leads to better performance. We introduce a sub-500-gram quadruped robot with a rich leg design space. Made with laminate design and fabrication techniques, its legs have a range of tunable design parameters, including leg length, foot travel, transmission ratio, and passive parallel and series stiffness. The legs are also straightforward to model, low-cost, and fast to manufacture. We propose methods to span the leg's feasible design space and construct simulation environments for training a locomotion policy with reinforcement learning to remove the need for manual controller design and tuning. This policy not only works across leg designs but also exploits their unique dynamics for better locomotion. A curation process is employed to select designs given performance goals, which is more interpretable than optimization and provides insights for design improvements and discoveries of design principles. We showcase the proposed pipeline in selecting leg designs for two distinct tasks: pure locomotion, such as running and turning, and force-based locomotion, such as pulling, pushing, and carrying payloads. 
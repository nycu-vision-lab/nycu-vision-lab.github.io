## Multi-Target Labeling and Correspondence over Multi-Camera Surveillance System

The goal of this work is to locate, label, and correspond multiple targets with ghost
suppression over a multi-camera surveillance system. Practical challenges arise from
the unknown number of targets, inter-occlusion among targets, and ghost effects caused
by geometric ambiguity.

Instead of directly corresponding objects among different camera views, the proposed
framework adopts a fusion–inference strategy. In the fusion stage, a posterior
distribution is formulated to indicate the likelihood of having moving targets at
certain ground locations, from which a rough scene model is constructed.

In the inference stage, the scene model is input into a Bayesian hierarchical detection
framework, where target labeling, correspondence, and ghost removal are treated as a
unified optimization problem subject to 3D scene priors, target priors, and foreground
detection results. Target priors such as height and width are further refined via an EM
mechanism.

<span class="muted">
Reference: Ching-Chun Huang and Sheng-Jyh Wang, “A Bayesian Hierarchical Framework for
Multitarget Labeling and Correspondence with Ghost Suppression over Multicamera
Surveillance System”, <em>IEEE Transactions on Automation Science and Engineering</em>, Vol.9,
No.1, pp.16–30, January 2012.
</span>

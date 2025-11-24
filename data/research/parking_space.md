## Automatic Outdoor Vacant Parking Space Detection

We propose a vacant parking space detection system that operates both day and night.
In the daytime, major challenges include dramatic lighting variations, shadow effects,
inter-object occlusion, and perspective distortion. At night, insufficient illumination
and complex lighting conditions pose additional difficulties.

To tackle these problems, we adopt a structural 3D parking lot model consisting of
plentiful planar surfaces and propose a plane-based classification process to alleviate
the interference of unpredictable lighting changes and shadows. A Bayesian hierarchical
framework is then used to integrate the 3D model and plane-based classification for
systematic inference of parking status.

A pre-processing step is also introduced to enhance nighttime image quality, enabling
robust operation across different lighting conditions.

<span class="muted">
Reference: Ching-Chun Huang, Yu-Shu Tai, and Sheng-Jyh Wang, “Vacant Parking Space
Detection Based on Plane-based Bayesian Hierarchical Framework”, <em>IEEE Transactions on
Circuits and Systems for Video Technology</em>, Vol.23, No.9, pp.1598–1610, September 2013.
</span>

## UAV Aerial Image Analysis

In this work, we utilize the self-supervised model DINOv2 to identify whether grape
farms are infected with downy mildew from UAV aerial images and compare its analysis
accuracy with supervised models. We also evaluate the degradation in classification
performance as the number of training images is reduced.

To expedite the processing of UAV aerial imagery, we perform automatic 3D projection
and image stitching on the raw images to form a large-scale infection map. The entire
workflow is further accelerated using multiprocessing, which saves substantial time
and cost compared to off-the-shelf software.

<span class="muted">
Application: agricultural disease monitoring, UAV image processing, DINOv2.
</span>

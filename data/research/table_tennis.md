## Table Tennis Ball Detection based on Self-supervised Pre-trained Backbone

This work primarily explores how to develop a table tennis ball detector based on a small set
of training data. After some detailed studies over two popular models—the CenterNet
model based on the CNN structure and the DINO DETR model based on the transformer
structure—we propose a new object detection model.

The proposed detector replaces the backbone of the CenterNet model with the
state-of-the-art self-supervised pretrained model DINOv2, followed by several
modifications to further boost the performance in detecting small, fast-moving objects
such as table tennis balls.

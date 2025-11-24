## Low-shot Image Classification based on Self-supervised Pretrained Model

The core of low-shot learning is how we can train models effectively with limited data.
Recent studies have revealed that pre-trained models obtained through self-supervised
learning may inherently possess excellent low-shot learning capabilities. In this work,
we explore the performance of self-supervised pre-trained models in low-shot image
classification tasks using one of the best current self-supervised learning methods,
DINOv2.

We propose a stable and robust two-step fine-tuning pipeline to address potential
issues when fine-tuning the DINOv2 pre-trained model on small datasets. Next, we
compare the performance of DINOv2 and supervised pre-trained models in linear probing
and fine-tuning evaluations across four diverse datasets with varying data quantities.
We conclude that the DINOv2 pre-trained model not only consistently achieves higher
classification accuracy but also demonstrates better low-shot performance.

<span class="muted">
Key topics: self-supervised learning, DINOv2, low-shot image classification.
</span>

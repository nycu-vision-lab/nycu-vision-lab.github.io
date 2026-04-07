## Fast Blind Image Deblurring Based on Cross Partial Derivative

This work addresses the problem of blind image deblurring. Unlike conventional optimization-based iterative methods and recent deep learning methods, we propose a novel blind image deblurring algorithm for uniform blur that achieves both high efficiency and accuracy. The proposed method consists of two stages: blur kernel estimation and non-blind deconvolution. First, a novel blur kernel estimation method is applied to rapidly estimate the blur kernel. Then, we use the estimated kernel to perform non-blind deconvolution to restore the image.

In the blur kernel estimation stage, a key observation is that the blur kernel information is typically embedded in the peaks of the cross partial derivative (CPD) image of the blurred input. Based on this property, we develop a pipeline to find sparse peaks in the CPD image and extract multiple kernels as candidates. These candidates are further refined by exploiting the spectral correlation between the blurred image and the blur kernels, allowing us to select the most suitable kernel as the final estimated kernel.

In the non-blind deconvolution stage, since our kernel estimation method can obtain a fairly accurate blur kernel, we can achieve effective image restoration using a relatively simple Tikhonov regularization in the subsequent non-blind deconvolution process. To improve the quality of the restored image, we further adopt an efficient filtering technique to suppress periodic artifacts that may appear in the restored images.

The proposed algorithm is implemented in MATLAB. Experimental results demonstrate that our algorithm can efficiently restore high-quality sharp images on standard CPUs without relying on GPU acceleration or parallel computation. For blurred images of approximately 800x800 resolution, the proposed method can complete image deblurring within 1 to 5 seconds, which is significantly faster than most state-of-the-art methods.

Source Code: https://github.com/e11tkcee06-a11y/CPD-Deblur.git

<span class="muted">
Keywords: Blind image deconvolution, blur kernel estimation, second-order cross partial derivative, Tikhonov regularization filter.

Reference: K.-C. Ting, S.-J. Wang, and R.-B. Hwang, “Fast Blind Image Deblurring Based on Cross Partial Derivative,” IEEE Transactions on Image Processing, vol. 34, pp. 8627–8640, 2025, doi: 10.1109/TIP.2025.3645574.
</span>

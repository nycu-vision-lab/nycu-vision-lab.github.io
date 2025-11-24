## Hierarchical Image Segmentation

We propose a new framework for hierarchical image segmentation based on iterative
contraction and merging. The hierarchical image segmentation problem is treated as a
sequence of optimization problems, each realized by a contraction-and-merging process
to identify and merge the most similar data pairs at the current resolution.

At the beginning, pixel-based contraction and merging are performed to quickly
combine image pixels into initial region elements with visually indistinguishable
intra-region color differences. Then, region-based contraction and merging are
iteratively applied to group adjacent regions into larger ones and progressively form a
segmentation dendrogram for hierarchical segmentation.

Compared with state-of-the-art techniques, the proposed algorithm not only produces
high-quality segmentation results in a more efficient way, but also preserves a large
amount of boundary details.

<span class="muted">
Reference: Syu, Jia-Hao, Sheng-Jyh Wang, and Li-Chun Wang, “Hierarchical image
segmentation based on iterative contraction and merging,” <em>IEEE Transactions on Image
Processing</em>, 26(5):2246–2260, 2017.
</span>

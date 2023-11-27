---
layout: page
title: Image Segmentation with extension on MAE and SAM
description: Supervised by Prof. Yibin Xie, Cedars-Sinai, UCLA (remote), 2023.06 -
img: assets/img/SAM_model.jpg
importance: 1
category: research
# related_publications: einstein1956investigations, einstein1950meaning
---

**Research Focus**: based on foundation model SAM, enhance it to accept 3D medical images to segment volumetric labels.

**Methodology**: Investigated MAE, the image encoder SAM referenced, and modified an effective 3D image encoder through operating on patch embedding. Then plugged it into SAM, with staged training strategy, and confirmed the unnecessary use of adapters, which is a widely used strategy for SAM-related 3D segmentation.

**Performance**: For now, the tested organs in amos22 dataset can best achieve a dice score around 0.83 using base SAM model, which is a small size model, proving our strategy’s effectiveness.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/SAM_model.jpg" title="model structure demonstration" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    It's the overall model of this work.
</div>

**Demo of Results**:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/video/visualization.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="caption">
    Segmentation of right kidney.
</div>
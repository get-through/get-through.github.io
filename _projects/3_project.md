---
layout: page
title: Cell Image Reconstruction by SIM
description: Supervised by Prof. He Sun, Peking University, 2022.09 - 2023.06
img: assets/img/SIM_model.jpg
# redirect: https://unsplash.com
importance: 3
category: research
---

**Research Focus**: Using learning approach to perform SIM reconstruction.

**Methodology**: 
- Traditional structured illumination microscopy (SIM) is manually calculated and concatenated, combined with wiener deconvolution.
- A simple neural network of initializing a picture, rendering it through a forward process, and training on loss is conducted to get a high resolution single picture.

**Performance**: Can outperform traditional method of deconvolution.

**Further Progress**: Combine with generative models, and accept fewer than 9 pictures.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/SIM_model.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    It's the overall model of this work.
</div>
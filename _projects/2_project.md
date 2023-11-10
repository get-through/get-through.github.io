---
layout: page
title: Multislice phase reconstruction based on BRIEF and NeRF
description: Supervised by Prof. Yi Xue, UC Davis (remote), 2023.06 -
img: assets/img/RI_model.jpg
importance: 2
category: research
giscus_comments: true
---

**Research Focus**: By using IDT modality, recover better 3D RI using a deep learning framework. 

**Methodology**: 
- Traditional IDT and uses only the intensity image obtained with different light directions to reconstruct the RI.
- A former work by Prof. Yi Xue introduced BRIEF to combine fluorescence imaging with IDT, exciting a fluorescent point to light up the upper samples, and used FISTA to compute gradient and do backward updates.
- NeRF’s MLP layers were adopted to compute a 1 channel output as input for RI, a rendering process of multislice model was used to process the RI into intensity image, then loss was computed and trained.

**Performance**: Can now reconstruct intensity on simulated data, need improvement on RI.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/RI_model.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    It's the overall model of this work.
</div>
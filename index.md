---
layout: project_page
permalink: /

title: "OceanSplat: Object-aware Gaussian Splatting with Trinocular View Consistency for Underwater Scene Reconstruction"
authors: Minseong Kweon, Jinsun Park
affiliations: University of Minnesota, Pusan National University
paper(soon): https://mnseong.github.io/OceanSplat
code(soon): https://mnseong.github.io/OceanSplat
data(soon): https://mnseong.github.io/OceanSplat
---

<!-- Using HTML to center the abstract -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Abstract</h2>
        <div class="content has-text-justified">
We introduce OceanSplat, a novel method that captures geometric structures in scattering media with high fidelity for real-time 3D underwater scene representation. To overcome the severe attenuation and scattering effects inherent in underwater environments, our method imposes trinocular stereo consistency on views translated along two orthogonal axes, effectively constraining the spatial placement of 3D Gaussians and preserving object geometry under complex medium conditions. We further apply self-supervised geometric regularization using a synthetic epipolar depth prior derived from these translated views to suppress medium-induced misplacement of 3D Gaussians. In addition, we align the rendered depth with the $z$-component of individual 3D Gaussians to suppress floaters and enhance structural fidelity. Furthermore, we propose a depth-aware alpha adjustment module that uses directional and depth cues to guide visibility learning in the early stages of training, preventing erroneous placements and medium entanglement. Our method effectively represents 3D scenes under scattering media without external geometric cues by preventing foreground 3D Gaussians from erroneously contributing to the medium in novel views, thereby preserving overall scene quality. Experiments on real-world underwater and simulated scenes demonstrate that our method outperforms prior approaches in 3D scene representation under scattering media.
        </div>
    </div>
</div>

---

## Qualitative Results

![Results1](/static/image/oceansplat_img1.png)
_**Fig. 1.** Qualitative results of novel view synthesis on diverse real-world underwater 3D scenes._

## Quantitative Results

![Results2](/static/image/oceansplat_img2.png)
_**Fig. 2.** Quantitative results of novel view synthesis on SeathruNeRF and In-the-Wild datasets._

> Note: This work is currently under review at double-blind conference.

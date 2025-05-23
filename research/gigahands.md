---
layout: project
title: "GigaHands: A Massive Annotated Dataset of Bimanual Hand Activities"
authors:
  - author:
      name: "Rao Fu"
      affiliation: 1*
      link: https://freddierao.github.io/
  - author:
      name: "Dingxi Zhang"
      affiliation: 2*
      link: https://kristen-z.github.io/
  - author:
      name: "Alex Jiang"
      affiliation: 1
      link: https://www.alex-jiang.com/about/
  - author:
      name: "Wanjia Fu" 
      affiliation: 1
      link: https://wanjia-fu.com/
  - author:
      name: "Austin Funk"
      affiliation: 1
      link: https://austin-funk.github.io/
  - author:
      name: "Daniel Ritchie"
      affiliation: 1
      link: https://dritchie.github.io/
  - author:
      name: "Srinath Sridhar"
      affiliation: 1
      link: https://cs.brown.edu/people/ssrinath/
affiliations:
  - "<sup>1</sup>[Brown University]"
  - "<sup>2</sup>[ETH Zurich]"
  - "*[Equal Contributions]"
journal: CVPR 2025
redirect_from:
  - add redirect_path here
  - another path here
---

{% include icons.html paper="https://www.arxiv.org/abs/2412.04244" code="https://github.com/Kristen-Z/GigaHands" dataset="https://github.com/Kristen-Z/GigaHands" %}

{% include full_image.html path="/assets/images/projects/gigahands/teaser.jpg" alt="[Teaser Figure]" %}
**We present GigaHands, a massive annotated bimanual hand activity dataset, unlocking new possibilities for animations, robotics and beyond.**
Each column above shows an activity sequence from the dataset. The bottom row show other annotations in the dataset including text, hand shape, object shape and pose (left half images). The right half images show novel views from dynamic radiance field fitting.

---
# Abstract
Understanding bimanual human hand activities is a critical problem in AI and robotics. We cannot build large models of bimanual activities because existing datasets lack the scale, coverage of diverse hand activities, and detailed annotations. We introduce GigaHands, a massive annotated dataset capturing 34 hours of bimanual hand activities from **56 subjects** and **417 objects**, totaling **14k motion clips** derived from **183 million frames** paired with **84k text annotations**. Our markerless capture setup and data acquisition protocol enable fully automatic 3D hand and object estimation while minimizing the effort required for text annotation. The scale and diversity of GigaHands enable broad applications, including text-driven action synthesis, hand motion
captioning, and dynamic radiance field reconstruction.
{% include video.html path="/assets/images/projects/gigahands/gigahands_explain.mp4" alt="[Video Teaser]" %}
(video contains audio)

---
# Dataset Annotations
**To be released soon**

GigaHands is a diverse, massive, and fully-annotated 3D bimanual hand activities dataset. All sequences in GigaHands are fully annotated with: detailed activity text descriptions; 3D hand shape and pose; 3D object shape, pose and appearance; hand/object segmentation masks; 2D/3D hand keypoints; camera pose.
{% include video.html path="/assets/images/projects/gigahands/example_video_small.mp4" alt="[Dataset]" %}

---
# Application: Text-driven Motion Generation
We showcase text-driven motion generation enabled by training a generative model with GigaHands.
{% include video.html path="/assets/images/projects/gigahands/motion_small.mp4" alt="[Motion Results]" %}

---
# Application: Motion Captioning

<b><u>Within Dataset</u></b>
We showcase 3D hand motion captioning by training a generative model with GigaHands.
{% include video.html path="/assets/images/projects/gigahands/caption_small.mp4" alt="[Caption Result]" %}

<b><u>Other Dataset</u></b>
Using generative model trained only GigaHands, we enable 3D hand motion captioning for other datasets.
{% include video.html path="/assets/images/projects/gigahands/caption_itw_small.mp4" alt="[Caption in-th-wild Result]" %}

---
# Application: Dynamic 3D Scene Reconstruction
GigaHands provides hand motions captured from **51 camera views**, enabling dynamic 3D scene reconstruction. The examples below showcase frame-wise 2DGS (Huang et al.) reconstruction results.
{% include video.html path="/assets/images/projects/gigahands/2dgs.mp4" alt="[Reconstruction Result]" %}

---
# Application: Motion Retargeting (with Physics)
Thanks to the accurate 3D motion tracking, complex manipulation sequences can be retargeted to robot grippers (inspire hand) with ManipTrans (Li et al.).
{% include video.html path="/assets/images/projects/gigahands/motion_retarget.mp4" alt="[Retarget Result]" %}

---
# Citations
```
@article{fu2025gigahands,
  title={GigaHands: A Massive Annotated Dataset of Bimanual Hand Activities},
  author={Fu, Rao and Zhang, Dingxi and Jiang, Alex and Fu, Wanjia and Fund, Austin and Ritchie, Daniel and Sridhar, Srinath},
  year={2025},
  publisher={CVPR 2025}
}

```

# Acknowledgements
This research was supported by AFOSR grant FA9550-21-1-0214, NSF CAREER grant #2143576, and ONR DURIP grant N00014-23-1-2804. We would like to thank the OpenAI Research Access Program for API support and extend our gratitude to Ellie Pavlick, Tianran Zhang, Carmen Yu, Angela Xing, Chandradeep Pokhariya, Sudarshan Harithas, Hongyu Li, Chaerin Min, Xindi Qu, Xiaoquan Liu, Hao Sun, Melvin He and Brandon Woodard. 

# Contact
Rao Fu ([contact email](rao_fu@brown.edu))

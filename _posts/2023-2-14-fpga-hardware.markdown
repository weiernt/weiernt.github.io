---
layout: post
title: "FPGA Hardware Acceleration for Image Super-Resolution"
date:   2023-2-14 14:00:00 +1100

thumbnail: "/assets/fpgahardware/sidebyside-LR-SR.png"

excerpt_separator: <!--more-->


---

In January 2023, I had the opportunity to undertake a research project about hardware acceleration using FPGAs. <!--more--> 
I had applied to undertake this project as part of a subject for credit over the summer, back in late 2022, since the department was advertising these research subjects to high achieving students.
I think I was quite fortunate to have been selected to work on this, since I wanted to get more hands-on experience working with FPGAs, which I hadn't worked with since my last subject in digital systems (which was back in 2021!). As part of taking this subject, I was also granted a scholarship stipend.

Through the 6 weeks of this project, I was working on designing an FPGA implementation of the [Super-Resolution Convolutional Neural Network](https://arxiv.org/abs/1501.00092) (SRCNN) by Dong et al., using general hardware acceleration techniques such as:
- Loop pipelining,
- Loop unrolling,
- Loop tiling,
- Array partitioning

My work was mainly on the inference stage of this CNN, rather than the training stage.



|![image tooltip here](/assets/fpgahardware/sidebyside-LR-SR.png){:.centered , width="50%"}|
|:--:| 
| *Example of image super-resolution, where the image on the left is low resolution and blurry, but the image on the right is of a higher resolution which was obtained by super-resolution.* |



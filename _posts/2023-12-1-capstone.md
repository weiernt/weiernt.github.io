---
layout: post
title: "Fabricating Photodiodes"
date:   2023-12-1 12:00:00 +1100

thumbnail: "/assets/capstone/chip-in-carrier.jpg"

excerpt_separator: <!--more-->


---


|![image tooltip here](/assets/capstone/chip-in-carrier.jpg){:.centered , width="50%"}|
|:--:| 
| * The silicon photodetectors are placed in a chip carrier and wirebonded. There are multiple photodiodes on the rectangular silicon wafer shown. * |


Many electronics students are coming out of university without ever having worked on, seen or touched a silicon wafer. <!--more--> 
While just being able to use MOSFETs, diodes and other semiconductor devices as if they were black boxes that obeyed their IV characteristics is fine, the students' learning experiences and intuitive understanding of these devices could be significantly improved if they knew *why* (for example) BJTs are designed in a certain way and *how* to build them.



The main goal of this final year project was to design a device fabrication workflow which could be easily and relatively safely replicated by undergraduate or graduate students. Naturally this isn't going to be competing with the likes of Samsung or TSMC's foundries where they're reaching down to feature sizes in the nanometer scale, but as a learning environment for students? This will do. 

**Make no mistake**. This is not the first time a "budget" and simple fabrication workflow has been developed. Other authors such as [Morsin et al. (2009)](https://ieeexplore.ieee.org/abstract/document/5356421/) and [Ryan (2016)](https://digitalscholarship.unlv.edu/cgi/viewcontent.cgi?article=3901&context=thesesdissertations) have investigated low cost methods for fabrication, in the pursuit of allowing students to be exposed to device fabrication.

Even the homebrew and "Youtube" scene, there are tinkerers who have created working [MOSFETs](https://www.youtube.com/watch?v=w_znRopGtbE), diodes and even a [differential amplifier](http://sam.zeloof.xyz/first-ic/)!





|![image tooltip here](/assets/capstone/a4_crosssection.png){:.centered , width="50%"}|
|:--:| 
| * Simplified diagram showing the steps involved in our fabrication process to create a doped region and metal pads. * |
|![image tooltip here](/assets/capstone/EEE-Discipline-Award-Simplified-Silicon.png){:.centered , width="50%"}|
|:--:| 
| * With this project, we won the Electrical and Electronics Engineering Discipline Award. From left to right: me, Yumin Li, Jimmy Sun, Mark Cassidy (Dean of the Faculty of Engineering and IT) * |


|![image tooltip here](/assets/capstone/capstone_poster_annotated_microscope.png){:.centered , width="50%"}|
|:--:| 
| * A microscope view of the photodiodes. The base wafer is an N-type doped (Phosphorous) wafer, while the doped regions are P-type doped (Boron). * |


|![image tooltip here](/assets/capstone/booth_endeavour.jpg){:.centered , width="50%"}|
|:--:| 
| * Our booth during the Endeavour Exhibition (Semester 2, 2023). On the right of the table are a collection of silicon samplpes at various different stages of the process. On the left is a set-up to demonstrate the functionality of the photodiodes to detect different intensities of light. * |

|![image tooltip here](/assets/capstone/depositer.jpg){:.centered , width="50%"}|
|:--:| 
| * The electron-beam evaporator used to deposit both the oxide layer and the conductive metal layer. * |



|![image tooltip here](/assets/capstone/iv-curve.png){:.centered , width="50%"}|
|:--:| 
| * Voltage and current plot when the photodiode was illuminated (around 1/10th of a Sun) and in the dark. This curve is typical for diodes in general, where the negative voltage region does not allow significant current flow, but the positive voltage region shows an exponentially **increasing** current flow as voltage **increases**.* |
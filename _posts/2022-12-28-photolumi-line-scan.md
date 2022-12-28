---
layout: post
title: "Photoluminescence Line Scan Set Up"
date:   2022-12-28 17:00:00 +1100

thumbnail: "/assets/researchassistant/infrared-scan.png"

excerpt_separator: <!--more-->


---

In late November of 2022, I began working as a casual research assistant at the [Sustainable Energy & Environmental Devices (SEED) Laboratory](https://people.eng.unimelb.edu.au/jbullock/index.html).
<!--more-->  
<!-- The group needed a device which was able to perform  -->

### Equipment

The controller, which controls the stepper motor uses:

- A TB6560 stepper driver module
- An Arduino Uno (in my case, a CH340 version, which is just a cheaper clone of the regular UNO)
- A 24V power supply, rated for at least 1.5A

The stepper-motor-controlled platform was from [Beijing PDV Instrument](https://www.pdvcn.com/), though I was not able to find the exact model on their website. It was using a stepper motor from Shinano (`Y07-43D1-4275`). Also worth noting the platform already had (Hall effect) limit switches installed, which made life easier when it was time to set up those limits.

### Software

The Arduino was flashed with [GRBL](https://github.com/gnea/grbl)





---



[Link](https://www.orca.unsw.edu.au/line-scan-pl-imaging) to a UNSW article about Photoluminescence (PL) line scans.

|![image tooltip here](/assets/researchassistant/infrared-scan.png){:.centered , width="50%"}|
|:--:| 
| *Initial scan of a piece of marked silicon, an infrared lamp was shone on the silicon sample. Worth noting that it is possible to see the mounting screw holes behind the silicon sample in this image* |

|![image tooltip here](/assets/researchassistant/original-sample-cropped.jpg){:.centered , width="50%"}|
|:--:| 
| *Image of the silicon sample taken with a normal camera* |

|![image tooltip here](/assets/researchassistant/laser-set-up.jpg){:.centered , width="50%"}|
|:--:| 
| *The moving stage placed inside of the black enclosure, with the controller (in the blue/green container) placed outside of the enclosure.* |

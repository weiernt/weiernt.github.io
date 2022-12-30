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

### Software Configuration

The Arduino was flashed with [GRBL](https://github.com/gnea/grbl)

### 3D Printed Enclosure

Not having done extensive 3D modelling and printing before, I based the design off from [this example](https://www.youtube.com/watch?v=E0bhdr84FNU). Though the enclosure needed to fit an extra TB6560 module, and some other connectors. I also tried to have the heatsink exposed to the air, rather than kept in the enclosure, just so there isn't any risk of the module overheating.

Some mistakes I did not consider with the modified design included not properly thinking about how the Arduino would slide in to the case, since in the original design (from the example), the USB type-B and DC power jack holes in the enclosure was contained in both the top and bottom half of the case, but in my attempt to make the enclosure taller, I forgot to have the USB and power jack be included for both parts of the case, so the Arduino needed to be somewhat harshly pushed into place (and have the poles/shafts connecting the top and bottom to be snapped off).

After printing the enclosure out, I also found the dimensions for the poles/shafts to be a bit thin (the smaller pole has a diameter of 2.8mm), so in the future, I would increase this to probably around 3.4 or 3.6mm.



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

|![image tooltip here](/assets/researchassistant/fusion360-bot.png){:.centered , width="50%"}|
|:--:| 
| *Bottom half of the 3D printed enclosure* |

|![image tooltip here](/assets/researchassistant/fusion360-top.png){:.centered , width="50%"}|
|:--:| 
| *Top half of the 3D printed enclosure (viewed from the bottom)* |

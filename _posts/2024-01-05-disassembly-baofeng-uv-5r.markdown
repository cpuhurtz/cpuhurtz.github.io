![image](https://github.com/cpuhurtz/cpuhurtz.github.io/assets/83088408/13667fcd-a724-49fc-91b9-8376beec3c34)![image](https://github.com/cpuhurtz/cpuhurtz.github.io/assets/83088408/fbd33309-c089-451a-86b9-2534a791235f)---
title: "Basic Disassembly of the Baofeng UV-5R"
layout: post
date: 2024-01-05 20:35
image: /assets/images/Baofeng-UV-5R.jpg
headerImage: true
tag:
- radio
- hardware
- firmware
category: blog
author: CHz
description: Rough overview of the disassembly of a Baofeng UV-5R, followed by the extraction of its IC-resident firmware.
---

## Summary:

Prolific within the intersection between amateur radio and civilian tactical groups, the Baofeng UV-5R is an exceptional first choice for anyone trying to understand programmable radios and their application within the field. I rarely use mine, if at all, so I figured it's better suited in the queue for teardown.

## Overview
- [Disassembly](#disassembly)
- [Components](#components)
- [Lifting Firmware](#lifting-firmware)
- [References](#references)

---

## Disassembly

I don't take credit for the [disassembly][1] video \[1\]; it was particularly useful for tearing down the coax port / feed line. Prior to removing the UV-5R's face, various header components had to be removed or at least loosened in order for me to have access to the board. I resorted to using an iFixit Precision Toolkit which was more than enough for my purposes. I recommend following this video to the 'T' if you intend on reassembling the radio; my method was clumsy at best, so a couple of components (namely the coax and LED) were slightly bent, but not horrifically so. Also, if anyone asks, I'm using a generic mouse pad as my "workspace" as opposed to an ESD mat on a lab bench. I'm not overly concerned with breaking this radio, and it's relatively inexpensive, so I did not take those precautions. Anyway, successful disassembly roughly results in:

* a backplate with spongy contact pads
* a rubber button cutout
* a display panel (which is situated against the plastic face cover for data display)
* at least 16 screws (four various sizes, depending on mounting point)
* a volume dial
* butt plate (also plastic in composition)
* a speaker which is glued to the front face of the radio
* a wire which is soldered between the spearker and contact patches on the circuit board
* and the circuit board itself ...

A lot of this is stuff you can find on forums across the internet, ranging from RU to JP.

---

## Components

Really helpful [resource][2] for identifying integrated component datasheets. A lot of the circuitry was identified [here][3], to include components of interest. But it's still worth noting the changes here. The most interesting ones here (of the ones I could actually discern):

* KDHM8F2K6 8-Bit Microcontroller, Serial No. 3SGV200391-Q 2034
    * 
* K24C64 EEPROM, Serial No. 2050TFX
* AT1688, Serial No. A459S922
* LT-ZY2012, Serial No. 2012
* TDA2822A, Serial No. ZXAX050



---

## Lifting Firmware

---

## References

\[1\] <https://www.youtube.com/watch?v=uvRocFQHOy0>
\[2\] <https://www.alldatasheet.com/>
\[3\] <https://www.allaboutcircuits.com/news/teardown-tuesday-baofeng-amateur-radio-transceiver/>

[1]: https://www.youtube.com/watch?v=uvRocFQHOy0
[2]: https://www.alldatasheet.com/
[3]: https://www.allaboutcircuits.com/news/teardown-tuesday-baofeng-amateur-radio-transceiver/

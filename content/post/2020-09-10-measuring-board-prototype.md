---
title: Measuring Board Prototype
author: Greg Buck
date: '2020-09-10'
slug: measuring-board-prototype
categories:
  - Equipment
tags: [FDMS]
description: ''
thumbnail: ''
---

In the fall of 2019 Roy Murray was contracted to develop the electronic components for a prototype fish measuring board. The imputus for this contract was the belief that a measuring board using commonly available electronic components could be developed that would be substantially cheaper and more rugged than the digital calipers currently used.

The specific requirements were:

-	Using an open source single board computer such as a Raspberry Pi or an open source microcontroller such as an Arduino, a device will be constructed that will transmit sex and length data to a Windows operating system via Bluetooth or directly by communications cable.

-	Two length sensors will be evaluated for the protoype.  One is a magnet-operated length sensor (EP-2 from MTS systems) and the other a touch-operated  linear potentiometer (Spectra Symbol ThinPot).  A single device will be constructed that can interface with either sensor for evaluation purposes.

-	System will operate on rechargeable battery power with minimum operating time before recharge of 6 hours at 35 degrees F.  Batteries will be recharged using off-the-shelf recharging hardware.

-	Sex data will be in numeric three digit code (1=male, 2=female, 3=unknown) and length data will be in millimeters with 1-2 mm of precision, measurable up to 1000mm.

-	Code written in Python for a Windows-based computer will be developed to receive and store transmitted fish data.

-	The device will be waterproof and sufficiently rugged to withstand the rigors of fieldwork. Design considerations will also include the goal of in-house maintenance and reproducibility.

-	At the end of this project an electronic schematic, parts list, and software along with any other design notes and/or drawings developed during this design process will be delivered to the state of Alaska along with any and all intellectual property rights.


[User's Manual](/FMBE_v_1_02_Operators_Manual.doc)

Sensors that will work with this device:

[EP2](https://mts.partcommunity.com/3d-cad-models/temposonics-ep2-stroke-length-50-3000-mm-mts-sensors?info=mts%2Findustriesensoren%2Fe_serie%2Fe_serie_ep2_asmtab.prj&cwid=8441)

[ThInpot](https://www.spectrasymbol.com/product/thinpot/)

[magnetopot](https://www.spectrasymbol.com/product/magnetopot/)

Currently we own one EP2 sensor. The EP2 sensor costs $400. The Spectrasymbol sensors cost about forty dollars. I recommend buying a few thinpot sensors for testing. Even if the thinpot sensors are not as robust as the EP2 the price difference may make them the more attractive option.

All files archived on the Anchorage network here:
S:\REG2\GBuck\Bristol Bay\CatchSampling\MeasuringBoard


Spectrasymbol salesperson's contact info:

Natalie Hardman 
Inside Sales
SPECTRA SYMBOL CORP
Email:  sales@spectrasymbol.com
Phone: 801-972-6995 EXT 20  
Fax: 801-972-8012


![electronics box](/IMG_0367.jpg)

Figure 1. Measuring board electronics.


![EP2](/IMG_0368.jpg)

Figure 2. EP2 sensor with (red) magnet.
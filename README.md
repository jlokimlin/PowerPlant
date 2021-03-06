PowerPlant
==========

This project documents how I'm automatically watering my patio plants with a solar powered Arduino and aquarium pump.

I wrote this code before I left for an extended vacation. My wonderful neighbor refilled the 8L container every few days and watered the parts the soaker tube did not water well. Water is pumped vertically from the reservoir in 1/4" tubing, then pushed through three rows of soaker tubing on the three rows of herbs. The water feeds down off the pallet and runs the length of my balcony, covering all my plants.

![This photo was taken the day we got back!](http://i.imgur.com/HziK3qG.png)

This is a [10W solar panel]("http://www.amazon.com/gp/product/B007YT5XCA/ref=as_li_ss_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=B007YT5XCA&linkCode=as2&tag=12vdcs-20) with a small [12V 7Ah Sealed Lead Acid Battery](http://www.amazon.com/gp/product/B003GXP10W/ref=as_li_ss_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=B003GXP10W&linkCode=as2&tag=12vdcs-20). The only other electrical components are a [insanely cheap 99 cent shipped eBay charge controller](http://www.ebay.com/itm/10A-Solar-Charge-Controller-Regulator-12V-24V-Autoswitch-100W-Solar-Panel-10A-/111262571836?pt=LH_DefaultDomain_0&hash=item19e7c41d3c) and some male/female [barrel plugs](http://www.amazon.com/gp/product/B002QWNZHU/ref=as_li_ss_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=B002QWNZHU&linkCode=as2&tag=12vdcs-20).


The Arduino is powered from the solar panel's battery, through an [automotive phone charger ](http://www.amazon.com/gp/product/B0088U4YAG/ref=as_li_ss_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=B0088U4YAG&linkCode=as2&tag=12vdcs-20). It takes 12-24V and has a pair of 2.1A 5V USB ports. My aquarium/fountain pump is designed for 12V but runs fine on unregulated 11-14V DC from the  battery.

Note: The above links to Amazon products are affiliate links. Any income earned will fund future open source automated gardening projects!

Here's a Fritzing image of the circuit breadboarded out. The ? PCB is an INA219 breakout for monitoring the power consumption of the pump.

![The circuit](http://i.imgur.com/zYkL1aL.png)



Components
=================

* Rectifier Diode 1N4001
* 12V aquarium Pump (Motor on diagram)
* Arduino
* Male + Female Power plugs for pump. Pass-through ports for power. 
* TIP120	NPN-Power transistor to switch the pump on and off
* 4k Ω Resistor
* $2 RTC Module DS1302 from eBay
* INA219 for current monitoring.

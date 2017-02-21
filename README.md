# DIY Split-Flap Display

This is a fork of scottbez1's project to create a Split Flap display. 
My attempt is to create a display that is simpler, sacrificing some functionality/correctness in order to create a tutorial that anyone can follow, even if they have no knowledge on the area. 
Since I'm a Software Engineer, I'm focusing on having an attractive software and a very simple hardware design.
If you know something about industrial design/electronics, I encourage you to take a look at https://github.com/scottbez1/splitflap
in order to develop a more professional display, and contribute with your ideas.

### I'm currently working on updating the documentation with details on how to build it, and I will load the controller code shortly.

This is a work in progress DIY [split-flap display](https://en.wikipedia.org/wiki/Split-flap_display).
Prototype two-character display: [video](https://www.youtube.com/watch?v=bslkflVv-Hw).

![animated rendering](https://s3.amazonaws.com/splitflap-travis/latest/3d_animation.gif)
[![prototype video](renders/prototypeVideoThumbnail.jpg)](https://www.youtube.com/watch?v=bslkflVv-Hw)

The goal is to make a low-cost display that's easy to fabricate at home in small/single quantities (e.g. custom materials can be ordered from Ponoko or similar, and other hardware is generally available).

The 3d model is built using OpenSCAD in `3d/splitflap.scad`, the driver board is designed in KiCad in `electronics/splitflap.pro`, and the driver firmware is written using Arduino in `arduino/splitflap/splitflap.ino`.

### Current Status ###
This design is currently at a *prototype* stage. The source files provided here were able to produce a working prototype (with some manual modifications to correct for slight errors/omissions), but aren't necessarily recommended yet unless you enjoy incomplete documentation, frustration, and adventure!

| Component | Status | Notes |
| --- | --- | --- |
| Enclosure/Mechanics | *Release Candidate* | Need documentation on ordering. |
| Electronics | *Beta* | Works but requires SMD soldering experience. Considering creating simpler variant: [#12](https://github.com/scottbez1/splitflap/issues/12) |
| Firmware | *Alpha* | Works, but needs cleanup, testing, and stable serial protocol |
| Control Software | *none* | No work started; currently manual control using Arduino Serial Monitor |

I'd love to hear your thoughts and questions about this project, and happy to incorporate any feedback you might have into these designs! Please feel free (and encouraged) to [open GitHub issues](https://github.com/scottbez1/splitflap/issues/new), email me directly, reach out [on Twitter](https://twitter.com/scottbez1), and [get involved](https://github.com/scottbez1/splitflap/pulls) in the open source development and let's keep chatting and building together!

### Design Highlights ###
* laser cut enclosure and mechanisms from a single material
* cheap, widely available 28byj-48 stepper motor (less expensive than NEMA-17 motors, and doesn't require an expensive high current stepper driver)
* CR80 PVC cards for flaps, cheap in bulk
* store-bought vinyl stickers for flap letters

![2d laser cut rendering](https://s3.amazonaws.com/splitflap-travis/latest/3d_laser_raster.png)

### Cost Breakdown ###
* $5/2 units -- MDF 3.2mm P2 [on Ponoko](http://www.ponoko.com/make-and-sell/show-material/64-mdf-natural)
* $20 -- laser cutting on Ponoko (can save ~$0.70 by skipping engraved label)
* $7 -- shipping from Ponoko
* ~$2 -- 28byj-48 motor (12V preferred!) and ULN2003 driver (see [motor notes](https://github.com/scottbez1/splitflap/wiki/Motor-info) for specific details)
* ~$5/5 units -- 5mmx100mm rod
* $6.39/2 units -- vinyl letter stickers (minimum letter duplication per pack is 2) [on Amazon](http://www.amazon.com/Duro-Decal-Permanent-Adhesive-Letters/dp/B0027601CM)
* $12/5 units or $36/25 units -- CR80 cards (each CR80 card becomes 2 flaps, each unit requires 40 flaps) on [Amazon](http://www.amazon.com/Plastic-printers-DataCard-Evolis-Magicard/dp/B007M413BC) or [Amazon](http://www.amazon.com/White-Blank-CR80-020-Graphic-Quality/dp/B007PKD6MW)
* ? -- M4x12mm button head bolts (e.g. ISO 7380)
* ? -- M4 nuts

TBD:
* $0.76 -- GP2S60 reflectance sensor [on digikey](http://www.digikey.com/product-detail/en/GP2S60B/425-2670-1-ND/1642454)
* $14/10 units -- PCB for reflectance sensor [on seeedstudio](http://www.seeedstudio.com/service/index.php?r=pcb)
* $6.66/4 units -- ATmega32U4 microcontroller for driver board [on digikey](http://www.digikey.com/product-detail/en/atmel/ATMEGA32U4-AUR/ATMEGA32U4-AURCT-ND/3440960)
* ? -- Other electronics components for driver/sensor boards

Tools:
* $9.17 -- badge slot punch (for cutting notches out of cards to make flaps) [on Amazon](http://www.amazon.com/gp/product/B009YDRRB4)

## Build Your Own: Instructions ##
This design is still a work in progress; a build log/instructions for building a prototype split-flap display of your own is posted in [the wiki](https://github.com/scottbez1/splitflap/wiki).

<a href="https://github.com/scottbez1/splitflap/wiki">
<img height="320" src="https://github.com/scottbez1/splitflap/wiki/images/assembly/laserPieces.jpg"/>
<img height="320" src="https://github.com/scottbez1/splitflap/wiki/images/flaps/punchedCard.jpg"/>
</a>

Note: most of the diagrams and downloadable files on this README page are auto-generated from the latest *experimental* code, which may be untested or broken. If you are interested in building one without digging into the design details much, I recommend using a stable design, as described in [the wiki](https://github.com/scottbez1/splitflap/wiki).

## License ##
I'd love to hear your thoughts and questions about this project, and happy to incorporate any feedback you might have into these designs! Please feel free (and encouraged) to [open GitHub issues](https://github.com/scottbez1/splitflap/issues/new), email me directly, reach out [on Twitter](https://twitter.com/scottbez1), and [get involved](https://github.com/scottbez1/splitflap/pulls) in the open source development and let's keep chatting and building together!

The vast majority of this project is licensed under Apache v2 (see [LICENSE.txt](LICENSE.txt) for full details).

    Copyright 2015-2016 Scott Bezek and the splitflap contributors
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
        http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

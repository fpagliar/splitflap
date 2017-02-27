# DIY Split-Flap Display

This is a fork of scottbez1's project to create a Split Flap display. 
My attempt is to create a display that is simpler, sacrificing some functionality/correctness in order to create a tutorial that anyone can follow, even if they have no prior knowledge on the area. 
Since I'm a Software Engineer, I'm focusing on having an attractive software and a very simple hardware design.
If you know something about industrial design/electronics, I encourage you to take a look at https://github.com/scottbez1/splitflap
in order to develop a more professional display, and contribute with your ideas.

### I'm currently working on updating the documentation with details on how to build it, and I will load the controller code shortly.

This is a work in progress DIY [split-flap display](https://en.wikipedia.org/wiki/Split-flap_display).
Prototype two-character display: [video](https://www.youtube.com/watch?v=bslkflVv-Hw).

![animated rendering](https://s3.amazonaws.com/splitflap-travis/latest/3d_animation.gif)
[![prototype video](renders/prototypeVideoThumbnail.jpg)](https://www.youtube.com/watch?v=bslkflVv-Hw)

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

### Materials ###

## Build Your Own: Instructions ##
This design is still a work in progress; a build log/instructions for building a prototype split-flap display of your own is posted in [the wiki](https://github.com/scottbez1/splitflap/wiki).

<a href="https://github.com/scottbez1/splitflap/wiki">
<img height="320" src="https://github.com/scottbez1/splitflap/wiki/images/assembly/laserPieces.jpg"/>
<img height="320" src="https://github.com/scottbez1/splitflap/wiki/images/flaps/punchedCard.jpg"/>
</a>

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

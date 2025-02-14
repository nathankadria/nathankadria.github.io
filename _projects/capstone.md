---
layout: page
title: Wire EDM Bandsaw
description: July - December 2024
img: assets/img/Capstone/GroupPic.jpeg
importance: 2
category: work
---

Before my final semester at Northeastern, I had been getting a bit obsessed with wire EDM machines. I was even considering building one myself, so you can imagine I was excited to see that one of the available capstone projects was to build custom wire EDM machine! The market for WEDM machines is dominated by extrememly capable machines with 6 figure price tags, and we had around 1/20th of that budget. In order to finish the project within a few months and on budget, we addressed a niche use case that required a smaller, much different set of requirements.

#### Client’s requirements
- Cut a metal 3D printed (DED) part off of a 18” build plate - previously a bandsaw or angle grinder was used
- Cuts must be flat within ±.020”
- Adjustable cut height
- Affordable (<$3000 w/o power supply)

#### Responsibilities
- Work with group of 6 to brainstorm novel format of Wire EDM machine
- Design X/Z axis, wire tensioning, end effector subassemblies
- Lead design and build of machine over extreme timeline
        
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Capstone/GroupPic.jpg" title="Capstone day group pic" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Capstone day group pic
        </div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Capstone/WEDMSystemFull.png" title="Full system" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Full system
        </div>
    </div>
</div>

#### Subsystem: X/Z Stage and Wire tensioning
- X/Z stage driven with geared stepper motors and EtherCAT drivers
- Hand calculations used to determine vertical displacement of wire due to X axis flex
- 2 servos run closed loop with load cell to control wire tension and speed
- Wire tensioning was inconsistent, so a planetary reduction was added to servos to increase precision and torque
- Further iteration necessary to reduce skipping on output wire tensioning assembly

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
       <div class="embed-responsive embed-responsive-16by9">
            <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/F96JPgQnWrg?si=0DWk4l375OWbe68q" allowfullscreen></iframe>
        </div>
        <div class="caption">
            Wire tensioning test
        </div>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
         {% include figure.liquid path="assets/img/Capstone/XZStage.png" title="XZ Stage" class="img-fluid rounded z-depth-1" %}
         <div class="caption">
            X/Z Stage
        </div>
    </div>
</div>

#### Subsystem: End Effectors
- End effectors were suspended on cantilevered beams to reach through 18” diameter build plate
- Water blocks mount diamond wire guides, nozzles, pulleys, and NPT fittings
- CFD used to determine correct nozzle orifice size, hand calculations used to determine necessary post-pump pressure
- End effector designed to be extremely compact in order to fit around workpiece in COTS stainless steel tank, significantly reducing cost
- Machinability of water block was crucial, as it was done in-house
- More bracing on end effectors was added to deal with inconsistent wire tension

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
       <div class="embed-responsive embed-responsive-16by9">
            <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/9p8HkfyGvnU?si=ImPcTZkd4Q4B8_Mf" allowfullscreen></iframe>
        </div>
        <div class="caption">
            Nozzle/water block pressure test
        </div>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
         {% include figure.liquid path="assets/img/Capstone/WaterBlockPart.png" title="Water block" class="img-fluid rounded z-depth-1" %}
         <div class="caption">
            Water block - my favorite part on the machine
        </div>
    </div>
</div>

#### What I Learned
- On large projects, splitting up the system and doing subsystem testing is critical
- Test early and often
- There is always a way - even if it's me buying a 3D printer with personal funds and running it around the clock to make stand-ins for machined parts
- Good project management means communicating failures early and delegating work, even if I’d prefer to do it myself
- Any engineering assumption made will be tested and could cause failures
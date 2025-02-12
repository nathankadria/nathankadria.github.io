---
layout: page
title: Wire EDM Bandsaw
description: Dec 2023 - Jul 2023
img: assets/img/Capstone/GroupPic.jpg
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
            <iframe class="embed-responsive-item" src="hhttps://www.youtube.com/embed/F96JPgQnWrg?si=0DWk4l375OWbe68q" allowfullscreen></iframe>
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





#### Design Process and Results
- New planetary gearset designed with helical gears
- Quotes showed that custom ring gears were too expensive and had long lead times
- Needed to pivot - a gearset from a junkyard automatic transmission was harvested and retrofitted to the assembly
- Testing with sound level meter proved significant NVH reduction
- Engineer sent from a major automaker from Wolfsburg approved the proof of concept’s NVH, resulting in a contract with the automaker

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
       <div class="embed-responsive embed-responsive-16by9">
            <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/mO29dz6uq9s?si=jJons5ZZu0bz3p0Z" allowfullscreen></iframe>
        </div>
        <div class="caption">
            NVH testing with retrofitted gearset
        </div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
         {% include figure.liquid path="assets/img/Orbis/RetrofitGearsetCADExploded.webp" title="Retrofit CAD exploded view" class="img-fluid rounded z-depth-1" %}
         <div class="caption">
            Retrofit CAD exploded view
        </div>
    </div>
</div>



## Gearbox, Motor, Brake, and Upright Assembly

##### Requirements
- Redesign previous assembly, keeping successful design elements and addressing failures
- Small form factor/stack height
- Lightweight

##### My contribtions
- Redesigned gearset stack - bearings, oiling, gearset selection
- Designed and optimized brake bell (red) with FEA
- Designed integrated upright (orange)
- Redesigned frustum that contains gearset (green)
- Work with machinist to make a printed model

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Orbis/WheelAssemblyCAD.webp" title="Assembly CAD" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Assembly CAD
        </div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Orbis/WheelAssemblyCADCutaway.webp" title="Assembly CAD section view" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Assembly CAD section view
        </div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Orbis/BellFEA.png" title="Bell FEA" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Bell FEA
        </div>
    </div>
</div>

#### Design Process

##### Address failures
- Previous bearing solution caused gears to take load from wheels and fail - redesigned to isolate gears from external forces
- New sealing solution designed to stop leaking

##### Reduce assembly’s stack height and weight
- McLaren MP4-12C upright integrated into motor mount
- Power dense axial flux motor used
- Lightweight brake bell, external rotor/internal caliper setup
- FEA used to optimized brake bell, reducing unsprung and rotating mass
  
  

## External Brake Rotor/Bell
- Designed and worked closely with machinist to make “bell” to mount external brake rotor
- Mustang GT rotor lightweighted and adapted to function as an external rotor
- Tested at Greening to validate performance vs. original rotor
- Underperformed compared to original rotor, but was significantly lighter

##### Conclusions
- Promising results, but an equal mass comparison would be
more valuable
- Brake rotor cooling optimization needed

<div class="row">
    <div class="col-sm-7 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Orbis/GreeningBrakeSetup.png" title="Greening test setup" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Brake test setup at Greening
        </div>
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Orbis/GreeningPreTest.png" title="Rotor pre-test" class="img-fluid rounded z-depth-1" %}
        {% include figure.liquid path="assets/img/Orbis/GreeningPostTest.png" title="Rotor post-test" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Brake rotor/bell pre and post test
        </div>
    </div>
</div>
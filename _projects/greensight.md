---
layout: page
title: Greensight
description: Jan-Sept 2024
img: assets/img/Greensight/HiveAtDemoLeft.jpg
importance: 1
category: work
---

During my time as a co-op at Greensight, I almost exclusively worked on the Hive team of the WeatherHive project. The “Hive” is a drone silo capable of storing, deploying, retrieving, and charging a swarm of 10 weather drones. About a month in, I was given full responsibility for the mechanical side of the hive, and I eventually extended my co-op to make sure I could see the project through.

I joined the project during an early revision of the hive, and designed a subsystem. I was then given full responsibility for the next revision of the mechanical side of the hive. I redesigned the Hive from the ground up with reliability, assembly, and an IP55 rating in mind. I constantly communicated with the electronics, software, and drone-side mechanical teams to avoid integration issues & allow for parallel development. I leveraged the use of sheet metal and 3D printed parts to prototype quickly and scale production up to 6 Hives, and then managed part procurement and assembly of these 6 Hives under an extreme timeline (3 months from design to demo).

Subsystems were tested individually to catch problems before we started full system integration. This project helped me hone my CAD skills, and taught me a lot about how to design for manufacturing as I had to scale up production from 1 unit to 6. Even with this small quantity, I started to run into issues I had never run into before and really had to plan out exactly how each hive was going to be made.

## WeatherHive

##### Requirements:
- Store 10 weather drones
- Autonomously launch, load, and charge drones
- Keep sensitive electronics with significant heat generation isolated from the elements
- Lightweight, rugged, and compact

##### My contributions:
- Solely responsible for mechanical design and testing
- Managed part sourcing and manufacturing under extreme timeline - 3 months to design and build 6 Hives
- Coordinated with electrical, software, and drone-side mechanical team to ensure smooth integration
- Traveled to demonstrate Hives to customers
        
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
         {% include figure.liquid path="assets/img/hiveBS/HiveAtDuskCropped.jpg" title="Hive At Dusk" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Testing the "Enhanced Hive" with autonomous landing and loading capabilities the night before demo day.
</div>

#### Subsystem: Drone Alignment and Charging
- Stores and charges 10 drones
- Minimally invasive on drone shape
- Low part count - only 5 unique parts
- Easy to manufacture sheet metal and COTS parts used wherever possible
- FEA done on charging contacts and alignment sheet metal
- Fatigue and wear testing done on charging spines and tin contacts

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
       <div class="embed-responsive embed-responsive-16by9">
            <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/4O0Wk7AeFi8?si=bXOy-hxiWUxjfM6B" allowfullscreen></iframe>
        </div>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Greensight/AlignmentASSY.png" title="Alignment Assembly" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left - fatigue/wear testing charging contacts | Right - half of alignment geometry
</div>

#### Subsystem: Drone Loading
- Drones land on ramp guided by vision system on Hive
- Ramp funnels drones into hive and starts to fold props
- Internal geometry passively aligns props and drone
- Zero additional actuators required with passive loading design
- Elevator actuator is reused and a passive ratchet mechanism stops drones from falling into loading zone
- Lots of iterations were tested to perfect the loading mechanism

<div class="row">
    <div class="col-sm-4 mt-3 mt-md-0">
       <div class="embed-responsive embed-responsive-16by9">
            <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/S1a7ZZE8yOE?si=KltshceoosIBTmsW" allowfullscreen></iframe>
        </div>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Greensight/DroneLoading.png" title="Drone Loading" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Greensight/HiveAtDemoLeft.png" title="Hive with Ramp" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left - loading testing | Middle - passive loading mechanism | Right - enhanced hive with landing ramp
</div>

#### Subsystem: Electronics "Dry Box"
- COTS IP65 aluminum enclosure was used for all sensitive electronics
- Waterproof bulkhead connectors used
- Heat sources were mated directly to the aluminum enclosure with thermal paste
- Heat sink on outside of enclosure was actively cooled with ducting and server fan
- Hand calculations and manufacturer specs were used to guide duct design
- High power jetson orin nano was used without overheating issues

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Greensight/HiveAtDemoBackRightCloseUp.jpg" title="Dry box in Hive" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Dry box in hive
        </div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Greensight/DryBoxDucts.png" title="Dry box ducts" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Cooling ducts for dry box
        </div>
    </div>
</div>

#### What I learned from WeatherHive

###### CAD
- Created and maintained a large assembly with multiple subassemblies
- Transferred SolidWorks experience to OnShape

###### Project management / collaboration
- Established clear plan and timeline for part design and procurement of 6 Hives
- Communicated with electrical, software, and drone-side hardware team to ensure easy integration
- Dummy hives built for other teams to test with helped with parallel development
- Subsystem testing conducted before final build

###### Design and iteration
- Fail early and often - design flaws caught earlier were much easier to address than those caught later in the process
- Ironing out issues with manufacturability and assembly helped reduce part procurement / assembly time when making multiple hives

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Greensight/HiveAtDemoDuskFar.jpg" title="Hive with mast" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Greensight/6Hives.jpg" title="6 Hives" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left - enhanced hive at dusk | Right - 6 Hives in various stages of assembly
</div>




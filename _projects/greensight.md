---
layout: page
title: Greensight
description: see my work on the WeatherHive project at Greensight
img: assets/img/Greensight/HiveAtDemoLeft.jpg
importance: 1
category: work
---

During my time as a co-op at Greensight, I almost exclusively worked on the Hive team of the WeatherHive project. The “Hive” is a drone silo capable of storing, deploying, retrieving, and charging a swarm of 10 weather drones. About a month in, I was given full responsibility for the mechanical side of the hive, and I eventually extended my co-op to make sure I could see the project through.

I joined the project during an early revision of the hive, and designed a subsystem. I was then given full responsibility for the next revision of the mechanical side of the hive. I redesigned the Hive from the ground up with reliability, assembly, and an IP55 rating in mind. I constantly communicated with the electronics, software, and drone-side mechanical teams to avoid integration issues & allow for parallel development. I leveraged the use of sheet metal and 3D printed parts to prototype quickly and scale production up to 6 Hives, and then managed part procurement and assembly of these 6 Hives under an extreme timeline (3 months from design to demo).

Subsystems were tested individually to catch problems before we started full system integration. This project helped me hone my CAD skills, and taught me a lot about how to design for manufacturing as I had to scale up production from 1 unit to 6. Even with this small quantity, I started to run into issues I had never run into before and really had to plan out exactly how each hive was going to be made.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        Requirements:
        - Store 10 weather drones
        - Autonomously launch, load, and charge drones
        - Keep sensitive electronics with significant heat generation isolated from the elements
        - Lightweight, rugged, and compact  
          
        My contributions:
        - Solely responsible for mechanical design and build of Hives
        - Managed part sourcing and manufacturing under extreme timeline - 3 months to design and build 6 Hives
        - Coordinated with electrical, software, and drone-side mechanical team to ensure smooth integration
        - Traveled to demonstrate Hives to customers
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets\img\Greensight\6Hives.jpg" title="6 Hives" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        Requirements:
            ● Store 10 weather drones
            ● Autonomously launch, load, and charge drones
            ● Keep sensitive electronics with significant heat generation isolated from the elements
            ● Lightweight, rugged, and compact
        My contributions:
            ● Solely responsible for mechanical design and build of Hives
            ● Managed part sourcing and manufacturing under extreme timeline - 3 months to design and build 6 Hives
            ● Coordinated with electrical, software, and drone-side mechanical team to ensure smooth integration
            ● Traveled to demonstrate Hives to customers
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}

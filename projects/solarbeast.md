---
layout: project
type: project
image: images/solarbeast.png
title: Solar Beast
permalink: projects/solarbeast
date: 2016
labels:
  - angular.js
  - Arduino
  - PID Loop
summary: Embedded Systems Design--Team based EE x96 project course focused on using Arduino.
forked: With permission from https://github.com/icarus0/unjammy.github.io/blob/master/projects/solarbeast.md
---

<div class="ui black inverted center aligned segment">

    <h2 class="ui header">Video Demonstration</h2>

</div>

<div class="ui container">
	<div class="ui embed" data-source="vimeo" data-id="199945024" data-placeholder="/images/solarbeast.png"></div>
</div>


### Scope:

   <p> Embedded System Design challenged us to use the popular Arduino microcontroller to build an innovative new product.  The project culminated with a sales pitch presentation at the end of the semester.  Many of the teams created intersting prodcuts that pushed the limits of what is possible with just an Arduino.  The motivation behind our project was to develop a cheap, peripheral system that can improve the power quality of solar arrays.  In particular, one way to improve power quality is to include a magnification lens transposed over the solar panel, the drawback, however, is angle of incidence must be nearly perfect for the power quality to improve.  Our system set to solve this problem using Log-Scale Analog Light Sensors, 180-degree Servo, and 3200-N Linear Actuater in conjunction with our Arduino.  Although initially designed as a theoretically addition to a magnified solar array, the system was capable of maintaing a 14V floating charge on a lead-acid powerbank, and led to data that supports a 13% increase in energy collection on traditional solar panels. </p>

### Role:

   <p>  In this project, I was a lead programmer who was responsible for programming the P-I-D algorithm and subsequent tuning.  I started by programming a basic iteration of the P-I-D that was capable of making binary decisions.  After which, I began deciding how aggressive the movement of the motors should be in relation to the analog data stream from our ICs.  The pedagogy of the algorithm was that the system should try to minimize the standard deviation of the IC Light Sensors.  To achieve this, a schematic of edges between the ICs was devised and movement was tuned based on a greatest-edge calculation.  From there I worked to improve our Angular.JS web application which included a User-Interface for viewing metrics.  The project was a success as shown by the systems ability to keep a floating charge on the lead-acid powerbank. </p>
    
#### Further Reading:

   <p> You can learn more at the <a href="http://ee.hawaii.edu">UH EE Department</a>. </p>
   
Forked with permission of [team member](https://github.com/icarus0/unjammy.github.io/blob/master/projects/solarbeast.md0.)
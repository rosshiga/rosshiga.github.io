---
layout: project
type: project
image: images/solarbeast.png
title: Solar Beast
permalink: projects/solarbeast
date: 2016-05-30
labels:
  - angular.js
  - Arduino
  - Cordova
  - Ionic
  - MySQL
  - Teamwork
summary: Team based sophomore project course focused on using Arduino.
---
<div class="ui large rounded images">
  <img class="ui image" src="../images/solarbeast.png">
</div>

Embedded System Design challenged us to use the popular Arduino microcontroller to build an innovative new product.  
The project culminated with a sales pitch presentation at the end of the semester.  Many of the teams created intersting
 prodcuts that pushed the limits of what is possible with just an Arduino. 
 The motivation behind our project was to develop a cheap, peripheral system that can improve the power quality of 
 solar arrays.  In particular, one way to improve power quality is to include a magnification lens transposed over the 
 solar panel, the drawback, however, is angle of incidence must be nearly perfect for the power quality to improve.  
 Our system set to solve this problem using Log-Scale Analog Light Sensors, 180-degree Servo, and 3200-N Linear 
 Actuator in conjunction with our Arduino.  Although initially designed as a theoretically addition to a magnified 
 solar array, the system was capable of maintaing a 14V floating charge on a lead-acid powerbank, and led to data that 
 supports a 13% increase in energy collection on traditional solar panels.

### Role:

In this project, I was a lead programmer who was responsible for programming the PhoneGap app using angular.js and Ionic to create a iOS and Android app using a single code base. JavaScript and HTML are combined in Ionic along with the INA219 High Side DC Current Sensor Breakout on our Arduino. I was able to gather current and voltage output rates on a Arduino and feed the power data using an ethernet shield into a simple PHP script which ingested the data to a MySQL table I setup. MySQL processed and averaged charging rates to display to the end user on their smartphone.

I also made contributions to logic chip selection and was the main designer and integrator of the lead acid battery charging logic which used the TI TPS5420 and TI UC3906N. I implemented the resistor feedback network, from the datasheets, needed to accommodate our charge rates.  

We suffered many set backs, mostly with the physical aspect of the project. Most notable is that we broke our solar panel mounting base while transporting it to the final showcase. All of us learned valuable lessons in ball bearings, epoxy, part selection, ordering, and of course failure. We did not size the solar panel correctly the first go an ended up with a beast, a 50W polycrystalline 2 foot square, which we then had to use and kicked off several redesigns. For someone more adept at the keyboard, I thank my fellow partners for the sleepless nights wondering how we can rotate and push a 4 pound beast with a tiny Arduino.

#### Further Reading:

You can learn more at the [UH EE Department](http://ee.hawaii.edu)
   
Forked with permission of [team member](https://github.com/icarus0/unjammy.github.io/blob/master/projects/solarbeast.md)
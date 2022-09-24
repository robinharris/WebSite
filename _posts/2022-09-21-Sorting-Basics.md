---
layout: post
title:  "Sorting some basics"
date:   2022-09-21 13:00:00 +0100
categories: jekyll update
---

# Getting a Wemos running on a battery with a solar panel charger

<img src="/WebSite/images/IMG_8174.JPG" alt="First Test" width="200" height="320" title="First Test Setup" margin=20px style="padding: 10px; float: left;">

Would my 6V solar panel provide enough power to keep a Wemos D1 Mini running?  Better check this first so set up a Wemos to measure its own battery voltage every 6 minutes and send it to an mqtt broker.  Between readings the Wemos goes into deep sleep to minimise its power consumption.  After 6 minutes it wakes up, takes a reading and sends it before going back to sleep.


The solar charge controller is a module built around an MCP73781.  It manages the charging of the battery and supplies power to the load from the solar panel (if available) and tops that up from the battery.


It **does not** regulate the output voltage so I needed to add a step down converter to provide a stable 3.3V supply for the Wemos.

In this photo the Wemos is lower left and to its right is the voltage regulator (down converter).  Top is the charge controller and the 18650 battery is top left.

This went into a 3D printed enclosure:

<img src="/WebSite/images/IMG_8177.JPG" alt="First Test" width="280" height="200" title="First Test Setup" margin=20px style="padding: 10px; float: right;">

For the first quick test the lid isn't fitted 

<img src="/WebSite/images/IMG_8178.JPG" alt="First Test" width="300" height="200" title="First Test Setup" margin=20px style="padding: 10px; float: left;">

The down converter doesn't have a mounting place in the enclosure so for now it is hanging by the conecting wires.  There will no doubt, be several other changes required so will wait to try and get a few in the next version.
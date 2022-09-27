---
layout: post
title:  "First Step"
date:   2022-09-18 20:40:57 +0100
categories: Weather-station
---

# Setting Up a Development Environment for a Wemos D1 Mini

<img src="/WebSite/images/wemos.jpg" alt="wemos" width="220" height="220" title="Wemos D1 Mini" margin=20px style="padding: 10px; float: right;">

I have used a Wemos D1 Mini (ESP8266 board) for several previous projects and have several to hand, so it seemed like a good choice for the brains of a weather station.  It has built in wi-fi so will easily send data from outdoor sensors to a server and indoor display. Also it can be put into a deep sleep mode to conserve power.

The project is taking shape with a Wemos as the controller, a LiPo battery with solar panel to charge it and a selection of sensors -  a DS18B20 temperature sensor, a tipping rain gauge, wind direction and wind speed detectors.

My preferred editor and development tools are VSCode with Platformio.  This produces Arduino compatible code which can be run on the Wemos D1 Mini.
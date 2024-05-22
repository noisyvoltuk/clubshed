---
layout: post
title:  "Garden Pond Depth Sensor"
date:   2024-04-16 13:18:24 -0400
series: "pond filler"
categories: renewables
---

# A starting point

The obvious starting point to maitianing the water level in a pond must be soem reliable way of sensign the actual water level

Considerations
- Accuracy
- Robustness
- Maintenenance

Solution options:
- Ultrasonic sensor
- Pressure sensor
- Conductivity sensor

It seems to be that both ultrasonic and conductivity methods may be subject to conditions, cleanliness etc.

A pressure sensor may also have the advantage of being easier to conceal.


For instance [MS5837-30BA](https://docs.rs-online.com/c97e/A700000006772506.pdf).

https://learn.adafruit.com/lps35hw-water-resistant-pressure-sensor/arduino

I'll use the I2C serial interface here, using just four wires: Vcc (red), 0V(black), SCL(yellow) and SDA (blue)

On the NodeMCU - SCL is pin D1, SDA is D2

Following the tutorial above, there's an example program that just records the temperature and pressure, and all looks good, so on to the real setup!



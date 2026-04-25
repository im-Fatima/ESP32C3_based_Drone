# ESP32C3_based_Drone

![drone] (drone.jpg)

![complete_drone] (drone2.jpeg)


## OVERVIEW
I started this project with a simple goal: build a quadcopter from scratch, write my own firmware, and get it into the air. I wanted to understand exactly how it all connects and work together.
I didn't reach the "perfect flight" stage, but I learned more about embedded systems in these few weeks than I have in months of reading textbooks. This repo is a documentation of my journey, the mistakes I made, and why I’m already moving on to V2.

### Below are some lessons I have learned while building my drone

## The Frame

I opted for a cheap solution which was using an Acrylic sheet for the frame, apparently it turned out to be too heavy for the drone. As for my next version I am designing a 3d chasis to avoid this issue.
![Frame_Image] (frame.jpg)

## The Flight Controller

I used ESP32C3 for two reasons, first that I initially aimed for ESPNOW protocol but it turns out, this was nearly impossible for a good drone as this protocol isn't good enough for a long range, and second that it is the cheapest version of ESP32, but apparently that comes with it's own cost, because it turns out, it doesn't have BLE that could support a connection with mobile and writing my own firmware from scratch including a browser interface for the drone control was really hard for me because I didn't have much experience with complex firmwares. Still it does work well over Wifi but only for a short range. For the V2.0, I have planned to design my flight controller using an STM32.
![Flight controller] (controller.jpg)


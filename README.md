# MACKLEMOUSE

## Overview

Key features:
  3 wheels, 2 powered and ball caster

  V1
  <img width="1032" height="762" alt="image" src="https://github.com/user-attachments/assets/efefab2f-501a-4c21-bb05-2f3d10cd09b5" />


Length: 10.5cm

Width: 8.0cm

Height: 5.5cm


### Hardware Plan:
10/12/26

The core of the mouse is an ESP32 Dev Board featuring 38 pins. This Microcontroller performs all logic and control for the rest of the robot. The power system comprises of 2 3.2V Lithium Ion batteries connected in series. These connect directly to the power of the motors, and to a 3.3V Buck Converter, dropping it down for the voltage logic level. The sensors are comprised of 2 side facing LED Emitters and Photo Transistors mounted roughly 10mm from each other as well as a forward facing Time of Flight (T.O.F.) sensor. The motor controller is mounted directly to the breadboard, and connects the ESP32 to the Motors. An additional sensor is the IMU, which is connected with I2C to the ESP 32. Additional peripherals include an LED display, 2 buttons, and a Piezo. The buttons will be used for interfacing with the bot during competition, and the screen and piezo will be used to feed the user information regarding the bot, as well as for entertainment purposes. 


  
9/20/26

This hitherto unnamed micromouse will be a mostly constructed from COTS parts powered by a central ESP32 devboard. It will consist of two geared brushed dc motors each connected to two wheels through a simple drivetrain. It will contain 4 IR sensors for positioning relative to the walls, and a accelerometer/gyrometer unit for additional precision. It will lastly use a Lithium Ion battery for power, as the safety and relative high energy per weight ratio are pros, and the relatively higher discharge rate of the LiPo battery is not required as speed is not (yet) a priority. The frame will be a width of 10cm and a length of 15. This is to allow cornering, although likely the first phase of this micromouse will not have the software ability to do this. The mouse will move orthagonally until I learn how to do it better. It will be programmed in C++. 




The overview should be a general description of your project. This should be a high level overview of your design decisions and how you will implement them, including detailed information on how you will handle difficulties such as software and hardware integration. This should also contain information on the hardware including references to the electrical requirements of all the individual components of your system and how those requirements will be managed. You should also discuss what kind of software you will be running, undergo a brief analysis to show you have the compute power to run your software, and discuss how the software will use the inputs your hardware gives it to complete its task. 

### Software Plan
10/12/2026
I will program the robot in C++. It is the language I am most familiar in and is the default language of the ESP32. I will be using VSCode for my IDE. I will communicate with the mouse over Bluetooth using a serial connection, as is built in with the ESP32. Below is a list of libraries I will be using. 
Note: This is not a complete list, and I will continue to add libraries as I begin to more fully understand what will be required. 

Software Libraries:

VL53L4CD (TOF) Library



Here you should include a detailed explanation of how your software will work. This should include the programming language(s) you will be using, any libraries, what IDE(s) you will be working with, your approach for testing your software, and how you will be using the inputs from your hardware to complete your task.

### Hardware Plan

LiPo Battery

Geared Motors, solder encoder, 50:1 gear ratio 

ESP32 Because I cool like that


This should be a more detailed explanation of how your hardware will work. This should include the electrical requirements of all the individual components of your system and how those requirements will be managed. This should also include a detailed explanation of the hardware components of your system and how they will interact with each other. This should include a detailed explanation of the sensors you will be using, how they work, and how you will be using them to complete your task. This should also include specifications of your components, including the voltage/current ranges they support as well as their physical dimensions (when applicable). 

Please include an Electrical Schematic somewhere in this repository showing excatly how each component connects together. You may use any software for this. We recommend KiCAD (ignore the PCB design part of the application, just use the schematic builder), but you may use any software you like.

Also include a CAD model of your robot, showing the placement of each component on your robot and any 3D printed parts you will need to construct. We recommend using OnShape because it makes collaboration easy, but any CAD software is acceptable.

### Bill of Materials (BOM)

Include a Bill of Materials document in this repository containing a list of all components you plan to use to construct your robot. Use Excel, Google Sheets, or another spreadsheet software.
For each component include a link to its product page, quantity, price, and a description of what it is used for. If you want to use a part that we already have in-stock, still include it in your BOM but indicate that it does not need to be ordered. Components must be from SA approved vendors: [https://safe.sa.buffalo.edu/vendors/preferred](https://safe.sa.buffalo.edu/vendors/preferred). Plan for a budget of around $100.

## Teammates and Responsibilities

### Sam Virkler
### Responsibilities:
Everything

## Milestones
Getting Started (9/16/26)
Electrical Schematic (9/26/26)
3D model (10/12/26)

## Targets:
Rough Draft Design (9/30/26)
BOM (10/10/26)
Finished Proposal (11/1/26)

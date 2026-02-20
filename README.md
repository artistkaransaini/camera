# SIMPLE FPV CAMERA SYSTEM

this is a bare bones low latency analog camera setup built with the runcam phoenix 2 micro. this project focuses on a minimalist hardware approach by bypassing complex flight controllers for a direct to monitor feed.

## THE HARDWARE

this project uses the Runcam phoenix 2 micro fpv camera.

### why this specific camera?
I chose the phoenix 2 micro specifically for its superior dynamic range and high voltage tolerance. unlike many standard micro cameras that require a strictly regulated 5v power source, the phoenix 2 can handle anywhere from 5v to 36v. this allows us to wire it directly to a variety of battery types (from 2s to 6s lipos) without the need for an external voltage regulator. this significantly reduces the point of failure and overall circuit complexity.

## WHY AM I MAKING THIS CAM?
Tho i know very little about tech i want to help my friend whos building a rocket and so this is the simplest place by which i help him witout messing up. like i literally spent *3 hours* on that Schematic cuz i have really never made one before in my life lol.



## WIRING LOGIC

the circuit is designed for maximum simplicity using a common ground architecture.

### COMPONENTS
* camera: runcam phoenix 2 micro
* power: 7.4v to 22.2v lipo battery
* switch: latching push button
* display: analog fpv monitor

### STEP BY STEP CONNECTIONS
**1. the power line**
* connect battery (+) to switch pin 1.
* connect switch pin 2 to camera vcc (red).

**2. the video line**
* connect camera vid (yellow) to screen vid.

**3. the ground loop**
* connect camera gnd (black) to screen gnd.
* connect screen gnd to battery (-).

## technical specifications
* sensor: 1/2" cmos sensor
* resolution: 1000tvl
* input voltage: 5v to 36v
* signal system: pal/ntsc switchable

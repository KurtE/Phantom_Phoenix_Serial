Warning
=======
This project is specific to the Trossen Robotics Phantom Phoenix Robots (both Hexapod a Quadrupod) 

This project is a split off of my main project (Arduino_Phoenix_Parts) that I do my work on to support a variety of Hex Robots.   
Actually this project is forked off of the Phantom_Phoenix project.  What makes this project different is that I am experimenting 
with talking to the Bioloid AX-12 servos using the Arduino hardware Serial objects (Serial1, Serial2), instead of using custom version of Arduino.  
This appears to work well using the Arduino 1.5.6 release which has updates to the hardware serial code base.  I have tried this out using standard 
Arduino Mega boards, as well as with the Arbotix controller.  I have a version of the Hardware definitions, which does not duplicate the core.   
I have uploaded a zip file with this to the Trossen forums before and may include a version here as well.

In addition, the BioloidSerial project has been updated to work with the Teensy 3.1 and I am using this with my own Teensy breakout boards. 

This project relies on installing one of my other projects BioloidSerial, which has the actual version of the Bioloid library that was updated 
to use the actual serial object.


Sometimes this project will be ahead of the other projects, other times it will be behind.  I will try to keep most of these projects in sync. 

General
=======

Most of the code in these libraries are in header files, which allows them to be compiled specifically for each project.   


Installation
============

Note: Hopefully this code is reasonably self-contained and can be located anywhere.  I personally keep this project
in my Arduino Sketchbook, such that I can load it, using the Arduino File/Sketchbook menu.   

This code requires that you have also installed the Arbotix extensions to the Arduino environment as well as their libraries.


Major Contributors
==================

Jeroen Janssen [aka Xan] -  The original Phoenix code was written by to run on the Lynxmotion Phoenix 
(http://www.lynxmotion.com/c-117-phoenix.aspx). It was originally written in Basic for the Basic Atom Pro 28
processor by Basic Micro.  

Kare Halvorsen (aka Zenta) -  The Lynxmotion Phoenix was based on the original Phoenix that was developed by
him.  In addition a lot of the software was based off of his earlier Excel spreadsheet (PEP).  More details up on his 
Project page (http://www.lynxmotion.com/images/html/proj098.htm).

Me - I later ported the code to C/C++ and the Arduino environment and with the help of Kåre and Jeroen hopefully 
reduced the number of bugs I introduced as part of this port.   

Michael E. Ferguson (lnxfergy up on Trossen) - Arbotix Commander, Ax12.

Again Warning
=============

This is a WIP - No promises or guarantees!


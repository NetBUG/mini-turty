# mini-turty


ROS package for the Mini-Turty robot.

Original product website: https://www.rhoeby.com/product/mini-turty
    
The Mini-Turty Robot from Rhoeby Dynamics represents a new level of value and functionality in a ROS navigation-capable robot. Designed with the lowest cost and complete user serviceability in mind, this robot is providing greatly improved access to advanced robotics navigation and much more!

## Hardware
The repository contains a [sample platform](mini_turty3/hw/lasercut) designed to be made with laser cutting. 
The base is cut out of 3mm birch plywood with principal strength direction oriented transversely (i.e. robot does not bend between the wheels).
Any other elements are cut out of 3 or 4mm acrylic sheet of any color. Motor holders are not optimal and will be improved soon to provide active suspension.
Unfortunately, the front navigation module (can be seen on sheets as a rectangle of 120x85 mm) was made long ago and design was lost. It contains:
 - Raspberry Pi 3 with heatsink, mounted on 4xM2 screws on the bottom sheet;
 - Neato xv11 lidar, mounted on upper sheet (which is elevated with 30mm M3 screws and pipe-like stands)
 - Raspberry Pi 3 extension made on a prototyping board with PLS connectors, providing connections to
  * lidar through on-board UART (serial kernel logging was disabled)
  * lidar motor power through a low-power SOT23 MOSFET
  * stepper driver outputs
  * I2C connector for  sensors (used for IMU)
  * 4xGPIO pins

The following external components have been used and fit on the base:
 - [18650-sized battery holder](https://www.thingiverse.com/thing:456900)
 - [LV8729 drivers](https://www.aliexpress.com/item/32808950520.html)
 - 2xNEMA17 stepper motors with Makeblocks wheels and wheel hubs
 - A [ball stand](https://pandao.ru/product/233c3d45-5e80-4f82-84e4-e2d594d67a44)

The following components have been fit on the upper board
 - A stepdown module using XL6009 chip
 - An [IMU](https://amperka.ru/product/troyka-imu-10-dof)
 - An IR receiver
 - [Power controller board](mini_turty3/hw/controller)

## Things You Can Do With Your Mini-Turty Robot

There are many things you can do with your Mini-Turty robot, including:

- Basics: ROS learning
- Teleop: robot remote control
- Map Building: make maps of your home or office for the robot to use
- Navigation: the robot moves autonomously around your home or office
- Tele-Viewing: see what your robot sees, even from another room*
- Frontier Exploration: the robot autonomously explores unknown terrain*
- Computer Vision: Mini-Turty recognizes objects in its environment*

*Coming soon, to a robot near you!

Available in kit form*, or fully assembled and ready to go. Either way, Mini-Turty provides endless hours of educational fun and represents the ideal platform for learning the Robot Operating System.

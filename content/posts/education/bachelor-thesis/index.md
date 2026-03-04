---
title: "Bachelor Thesis - Rover Simulation in the Unreal Engine 4"
hero: "Unreal.png"
date: 2019-09-15
menu:
  sidebar:
    name: Bachelor Thesis
    identifier: bachelor-thesis
    parent: education
    weight: 400
---

### Abstract
The subject of this bachelor's thesis is the development of a framework for simulating robots
and rovers in the Unreal Engine 4 (UE4). The simulation will connect to the robotic
framework Robot Operating System (ROS) and provides photo-realistic images for
computer vision applications. The well-established hardware abstraction layer interface
called `ros_control` was used to support actuator control in the simulation. To extract
sensory information from the photo-realistic virtual environment the rosbridge package
was used.
The newly proposed framework is a proof of concept for a game-engine-based simu-
lator with the Robot Operating System (ROS) to perform computer vision experiments
without requiring specialized hardware. It is also possible to use this
framework to gather a dataset to train neural networks on or to evaluate existing
machine learning techniques.
This framework will be evaluated on the example of the European Rover Challenge
(ERC). The student team from the Scientific Workgroup for Rocketry and Spaceflight
(WARR) already created a simulation, which will be used as reference. The results of
this bachelor's thesis show that the framework works as intended for controlling simple
actuators and joints; however, the current physics simulation of Unreal Engine 4 (UE4)
does not provide enough stability to simulate the proposed complex scenario without
major artifacts. Moreover, the camera plugin used in this thesis influences the physics
simulation negatively when parameters are changed to achieve real-time high-definition
support.
The framework does, however, provide a real alternative to already in-use state-of-the-
art solutions, as it enables an easy-to-manipulate robotic simulator with a powerful
graphics engine for photo-realistic simulations.
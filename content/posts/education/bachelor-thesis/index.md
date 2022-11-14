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
Subject of this bachelor thesis is the development of a framework for simulating robots
and rovers in the Unreal Engine 4 (UE4). The simulation will connect to the robotic
framework Robot Operating System (ROS) and provides photo-realistic images for
computer vision applications. The well established hardware abstraction layer inter-
face called ros control was used to support actuator control in the simulation. To extract
sensory information from the photo-realistic virtual environment the rosbridge package
was used.
The novel proposed framework is a proof of concept for a game-engine based simu-
lator with the Robot Operating System (ROS) to perform computer vision experiments
without the need of the required specialized hardware. It is also possible to use this
framework to gather a data set to train neural networks on or to do evaluation of existing
machine learning techniques.
This framework will be evaluated on the example of the European Rover Challenge
(ERC). The student team from the Scientific Workgroup for Rocketry and Spaceflight
(WARR) already created a simulation, which will be used as reference. The results of
this bachelor thesis show that the framework does work as intended for controlling sim-
ple actuators and joints, however the current physics simulation of the Unreal Engine
4 (UE4) does not provide enough stability to simulate the complex scenario proposed
to test the framework without major artifacts. Moreover does the camera plugin used
in this thesis influencing the physics simulation in a negative way if the parameters are
changed to gain realtime high definition support.
The framework does however give a real alternative to the already in use state-of-
the-art solutions as it enables a easy to manipulate robotic simulator with a powerful
graphics engine to support photo-realistic simulations.
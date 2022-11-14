---
title: "Master Thesis - Algorithm for Landing and Uprighting the MMX Rover with Gyroscopes"
hero: "mmx.png"
date: 2022-04-15
menu:
  sidebar:
    name: Master Thesis
    identifier: master-thesis
    parent: education
    weight: 300
---

### Abstract
The Martian Moons eXploration (MMX) mission is planned by the Japanese space
agency JAXA and will travel to Mars and its moons Phobos and Deimos. The main
objective of the spacecraft is to collect a sample from Phobos. As a part of this Mission
a small rover will be used to de-risk the main probe by letting it explore Phobos prior to
touch down. This rover is developed by CNES and the DLR and will be released from
the spacecraft approximately 50m above ground where it will then fall onto Phobos. Af-
ter some bounces on the surface the rover will autonomously unfold itself, deploy solar
panels and start recharging its batteries. The Problem arises from the fact that after
the fall and the bounces, the folded rover could be in any orientation and therefore it
is not guaranteed that the rover is able to stand up and deploy its solar panels. The
current implementation to tackle this problem is to just follow a pre-defined sequence
of steps blindly. As this is a very critical single point of failure of this whole sub-mission
it is desirable to increase the success rate of the deployment. It is very important to get
the unfolding right the first time, as if the rover tries to unfold its solar panels without
being in an upright position, the mechanism could get stuck and therefore the mission
would fail. Once the solar panel deployment is done, the leg movement is restricted
very drastically from a free rotation to operate within a specific angle range. This fact
limits further recovery attempts and therefore it is unlikely to succeed the rover mission.
From early prototypes it is shown that with the help of additional sensory feedback the
success rate can be increased. The hardware for the mission is already finalized an
therefore only the sensor suite present at the current time can be used to supplement
the uprighting process. The onboard two axis MEMS gyroscopes are the best option
to be used for this purpose. The hypothesis of this thesis is, that with the help of the
build-in two axis MEMS gyroscopes as feedback a better result can be achieved. As the
current implementation does nothing else then doing a blind guess and hoping for the
best it should yield better results when some sort of informed guess is taken, and different conditions are checked to ensure the rover does not fall over. To do this, different
approaches to incorporate gyroscopic sensors in this uprighting process are collected
and implemented. Finally, all implementations are evaluated and compared to the cur-
rent implementation to see if they are more successful. As access to real hardware is
not feasible and the environmental conditions on Phobos with its low gravity are very
special, it is not possible to do those experiments on real hardware and instead it is
necessary to simulate everything. The whole system, including the sensors, need to
be simulated in an effort to being able to create an ensemble of simulation runs, which
is necessary to infer statistic relevant information and draw a conclusion on the suc-
cess of the different methods. As this also includes the sensor, it is required to create
a representative model of the sensor that is comparable to the real world counterpart.
This model should model all necessary noise sources and uncertainties, but at the
same time it should not over complicate the already extensive simulation to keep the
simulation times low. In the end there will be a big comparison between all those approaches and the current implementation to see if the hypothesis is correct and where
the strengths and weaknesses of the different methods are.
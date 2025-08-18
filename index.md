---
layout: default
title: Zhiheng Chen
---

<div style="display: flex; gap: 40px; align-items: flex-start;">

  <!-- hovering avatar and navigation -->
  <div style="position: sticky; top: 4rem; flex-shrink: 0; width: 7.7rem; text-align: center;">
    <img src="./assets/avatar.JPG" width="120" style="border-radius: 0.8rem; margin-bottom: 0.1rem;">
    <div style="margin-top: 1rem; font-size: 0.88rem;">
      <a href="#personal-info" style="display: block; margin: 0.5rem 0;"> Personal Info </a>
      <a href="#research-overview" style="display: block; margin: 0.5rem 0;"> Research Overview </a>
      <a href="#project-demos" style="display: block; margin: 0.5rem 0;"> Project Demos </a>
    </div>
  </div>

  <!-- start of main contents -->
  <div style="flex-grow: 1;">

## Zhiheng Chen {#personal-info}
📍 Ithaca, NY  
📧 Email: zc548@cornell.edu | ericczh1@outlook.com  
🔗 [CV](./assets/CV.pdf) | [GitHub](https://github.com/Zhiheng-Chen?tab=repositories)

Hello! I'm a Master of Science student in the [Sibley School of Mechanical and Aerospace Engineering](https://www.engineering.cornell.edu/mae/) at Cornell University. 

---

## Research Overview {#research-overview}
I am intrigued by the analytical and data-driven modeling of dynamical systems, as well as their analysis and control based on the resulting models. Specifically, my research interests include:

#### Analytical Dynamics Modeling
I am interested in the analysis on the kinematics and kinetics of dynamical systems based on mechanics principles.
- In my undergraduate research (summer 2023), I worked on the 3D hybrid dynamics modeling and numerical simulations of a [legged hopping robot](https://ieeexplore.ieee.org/abstract/document/10611545). 
- As a self-driven project, I also modeled and simulated the 3D dynamics of a [wobbling coin rolling along the ground](https://github.com/Zhiheng-Chen/3D-Rolling-Disk-Dynamics-Simulation) (winter 2023). 
- In summer and fall 2024, I worked in the [UW Marine Robotics Laboratory](https://mrl.engr.wisc.edu/) on the dynamics modeling and simulations of a micro autonomous surface vehicle (MicroASV). 
- One of my current research projects is the dynamics modeling of a flexible robotic fish based on Hamilton's principle. The dynamics involve the sophisticated and interesting interactions among rigid bodies, elastic bodies, and fluids. I have coded up a working simulator of the robotic fish in Julia, and I am currently working on parameter and design optimizations based on the simulation results.

#### Data-Driven Modeling
In addition to analytical modeling, I am also fascinated by system identifications and equation learning for dynamical systems. 
- My research project at Cornell University revolves around the weak formulation of the Sparse Identification of Nonlinear Dynamics (SINDy) algorithm. [My advisor](https://www.engineering.cornell.edu/people/anastasia-bizyaeva/) and I are working towards improving the test functions of the weak-form SINDy to improve the interpretability, efficiency, and noise-robustness of the algorithm. 
- In the MicroASV project, I also designed a weak formulation-based parameter estimation algorithm to iteratively refine the dynamics model. 
- In Spring 2025, I designed the [EKF-ST](https://github.com/Zhiheng-Chen/EKF-ST) algorithm that combines the extended Kalman filter and sequential thresholding techniques. The algorithm enables recursive and simultaneous state estimations and equation learning.

#### Nonlinear Dynamics and Control
I am interested in the analysis and control of dynamical system based on the resulting models.
- I study fixed points, limit cycles, chaotic attractors, and bifurcations of nonlinear dynamical systems.
- In the legged hopping robot project, I designed aerial phase PD controllers to adjust the foot placement.
- In the MicroASV project, I designed LQR and variational principle-based (nonlinear) controllers for the robot, enabling it to accurately perform trajectory tracking tasks.

---

## Project Demos {#project-demos}
I am happy to share the demos of some of my projects mentioned in my research overview.

#### Rigid-Soft-Fluid Coupling Dynamics of a Robotic Fish 
This is a project I am currently working on. I model the fish as a rigid head and an elastic body connected by a motor-driven revolute joint. I use Hamilton's principle, [elastica theory](https://en.wikipedia.org/wiki/Elastica_theory), [Lighthill's elongated body theory](https://royalsocietypublishing.org/doi/10.1098/rspb.1971.0085), and Ritz series approximations to obtain the projected weak form of the equations of motion. Then I code up the numerical simulations in [Julia](https://julialang.org/):

<div style="text-align: left">
    <img src="assets/Fish.gif" width=700/>
</div>

#### 3D Contact Dynamics of a Rolling Disk
This was a self-driven project when I was an undergraduate student at UW-Madison. I modeled the 3D dynamics of the disk (size of a coin) using Lagrange's equations with 6 generalized coordinates. In the rolling phase, the equations of motion are solved in parallel with 3 constraint equations (2 nonholonomic constraints for roll without slip, and 1 holonomic constraint for the height of the contact point). I implememnted the [numerical simulations of the disk](https://github.com/Zhiheng-Chen/3D-Rolling-Disk-Dynamics-Simulation) in MATLAB:

<div style="text-align: left">
    <img src="assets/RollingDisk1.gif" width=330/>
    <img src="assets/RollingDisk2.gif" width=330/>
</div>

#### Hybrid Dynamics of a Legged Hopping Robot
In my undergraduate research, I was responsible for the 3D hybrid dynamics modeling and numerical simulations of a single-legged hopping robot named [PogoX](https://ieeexplore.ieee.org/document/10611545). I modeled PogoX as 2 rigid bodies connected by a prismatic joint. The hybrid dynamics model consists of the aerial phase, the impact mapping, and the stance phase, assuming a smooth transition from the stance phase to the aerial phase. I coded up the numerical simulations in MATLAB:

<div style="text-align: left">
    <img src="assets/PogoX.gif" width=800/>
</div>
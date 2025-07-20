<div style="display: flex; gap: 40px; align-items: flex-start;">

  <!-- hovering avatar and navigation -->
  <div style="position: sticky; top: 4rem; flex-shrink: 0; width: 7.7rem; text-align: center;">
    <img src="./assets/avatar.JPG" width="120" style="border-radius: 0.8rem; margin-bottom: 0.1rem;">
    <div style="margin-top: 1rem; font-size: 0.88rem;">
      <a href="#personal-info" style="display: block; margin: 0.5rem 0;"> Personal Info</a>
      <a href="#research-overview" style="display: block; margin: 0.5rem 0;">Research Overview</a>
    </div>
  </div>

  <!-- start of main contents -->
  <div style="flex-grow: 1;">

## Zhiheng Chen {#personal-info}
📍 Ithaca, NY  
📧 Email: zc548@cornell.edu | ericczh1@outlook.com  
🔗 [CV](./assets/CV.pdf) | [GitHub](https://github.com/Zhiheng-Chen?tab=repositories)

Hello! I'm a Master of Science student in the [Sibley School of Mechanical and Aerospace Engineering](https://www.engineering.cornell.edu/mae/) at Cornell University. 

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
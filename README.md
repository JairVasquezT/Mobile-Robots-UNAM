# Mobile Robotics Portfolio - Jair Vásquez Torres

This repository contains the work developed during my "Mobile Robots" course at UNAM (2024-2). I have implemented key autonomy modules, ranging from path planning and probabilistic localization to robotic manipulation and neural networks.

## 🛠 Key Technical Contributions

The following algorithms and systems were successfully implemented, tuned, and tested:

### 1. Autonomous Navigation & Path Planning
* **Pathfinding Algorithms:** Implementation of **A*** (Graph-based) and **RRT** (Rapidly-exploring Random Trees) for global navigation.
* **Path Smoothing:** Trajectory optimization using gradient descent algorithms to generate executable curves for the mobile base.
* **Path Following:** Implementation of control laws for linear and angular velocity ($v, \omega$) to ensure precise trajectory tracking.
* **Potential Fields:** Development of reactive obstacle avoidance methods using real-time attractive and repulsive forces.



### 2. Localization & Perception
* **Particle Filter (Monte Carlo):** C++ implementation of particle generation, motion update, and importance resampling for probabilistic localization using LIDAR data.
* **Extended Kalman Filter (EKF):** Mathematical modeling and Jacobian calculations for sensor fusion and state estimation.
* **Neural Networks:** From-scratch programming of **Backpropagation** algorithms for pattern classification.
* **Environment Representation:** Generation of inflated cost maps and Generalized Voronoi Diagrams (GVD) for safe navigation.



### 3. Integrated Project: Service Robot
Development of a Finite State Machine (FSM) for a mobile manipulator:
* **HRI:** Integration of voice commands for "Search and Carry" tasks.
* **Manipulation:** Implementation of inverse kinematics for grasping specific objects (e.g., Pringles can, apple).
* **Robustness Analysis:** Experimental system evaluation, identifying areas for improvement in final positioning precision and voice recognition success rate (60% accuracy).

---

## Requirements
* Ubuntu 20.04 (Focal Fossa)
* ROS Noetic

## Installation
*Note: It is assumed that Ubuntu and ROS are already installed.*

* $ cd
* $ git clone https://github.com/mnegretev/Mobile-Robots-2024-2
* $ cd Mobile-Robots-2024-2
* $ ./Setup.sh
* $ cd catkin_ws
* $ catkin_make -j2 -l2
* $ echo "source ~/Mobile-Robots-2024-2/catkin_ws/devel/setup.bash" >> ~/.bashrc
* $ source ~/.bashrc

## Testing

To verify the installation and compilation:

* $ cd 
* $ source Mobile-Robots-2024-2/catkin_ws/devel/setup.bash
* $ roslaunch surge_et_ambula movement_planning.launch

If correctly installed, you should see the following visualizers:
RViz Visualizer:
![rviz](https://github.com/mnegretev/Mobile-Robots-2024-2/blob/main/Media/rviz.png)

Gazebo Simulation:
![gazebo](https://github.com/mnegretev/Mobile-Robots-2024-2/blob/main/Media/gazebo.png)

GUI:

![GUIExample](https://github.com/mnegretev/Mobile-Robots-2024-2/blob/main/Media/gui.png)


## Contact
Dr. Marco Negrete<br>
Associate Professor C<br>
Signal Processing Department<br>
Faculty of Engineering, UNAM <br>
marco.negrete@ingenieria.unam.edu<br>

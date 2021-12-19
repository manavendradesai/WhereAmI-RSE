# WhereAmI-RSE

## Description --> 

Project 3 of the Robotics Software Engineering Nanodegree Program at Udacity. The objective was to learn the utilization of the ROS AMCL (Adaptive Monte Carlo Localization) algorithm to localize a mobile robot inside a map in the Gazebo simulation environment. During this process, ROS AMCL parameters were to be tuned to achieve sufficiently accurate and quick localization. Lastly, the tele-operation/navigation ROS stack was to be utilized to move the mobile robot. 

## Outcomes -->

- Learnt the basics of and coded (in C++) Kalman filters, extended Kalman filters and the Monte-Carlo localization algorithm in lab exercises
- Utilized the ROS **AMCL (Adaptive Monte-Carlo Localization)** package to accurately localize a mobile robot inside a map of my apartment in the Gazebo simulation environment
- Used the Tele-operation package to drive the mobile robot and over time **tuned the AMCL algorithm parameters** to achieve fast localization

## Directory structure -->

    ├── my_robot                       # my_robot package                   
    │   ├── launch                     # launch folder for launch files
    │   │   ├── RvizLaunch.launch
    │   │   ├── amcl.launch
    │   │   ├── robot_descriptionGoChaseIt.launch
    │   │   ├── worldGoChaseIt.launch
    │   ├── maps                       # folder containing the Gazebo world map and metadata
    │   │   ├── home.yaml
    │   │   ├── map.pgm
    │   ├── model                      # folder containing the Gazebo world model
    │   │   ├── homeGoChaseIt
    │   │   │   ├── model.config
    │   │   │   ├── model.sdf
    │   ├── meshes                     # meshes folder for the lidar sensor
    │   │   ├── hokuyo.dae
    │   ├── urdf                       # urdf folder for xarco files
    │   │   ├── my_robotGoChaseIt.gazebo
    │   │   ├── my_robotGoChaseIt.xacro
    │   ├── worlds                     # world folder for world files
    │   │   ├── homeGoChaseIt
    │   │   ├── homeGoChaseIt.world
    │   │   ├── myApartment
    │   ├── CMakeLists.txt             # compiler instructions
    │   ├── package.xml                # package info
    ├── teleop_twist_keyboard          # Tele-operation package for navigating the mobile robot in Gazebo
    │   ├── CHANGELOG.rst              
    │   ├── CMakeLists.txt             
    │   ├── README.md                  
    │   ├── package.xml                # package info
    │   ├── teleop_twist_keyboard.py   # package info
    ├── media                          # screenshots of the world and the robot
    └── Localization_screenshots       # screenshots showing progression in localizing the mobile robot

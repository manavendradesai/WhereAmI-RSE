# WhereAmI-RSE
Project 3 of the Robotics Software Engineering Nanodegree Program at Udacity

## Outcomes -->

- Utilized the ROS **AMCL (Adaptive Monte-Carlo Localization)** package to accurately localize a mobile robot inside a map of my apartment in the Gazebo simulation environment
- Used the Tele-operation package to drive the mobile robot and over time **tuned the AMCL algorithm parameters** to achieve fast localization

## Directory structure -->

    ├── my_robot                       # my_robot package                   
    │   ├── launch                     # launch folder for launch files   
    │   │   ├── robot_descriptionGoChaseIt.launch
    │   │   ├── worldGoChaseIt.launch
    │   ├── meshes                     # meshes folder for the lidar sensor
    │   │   ├── hokuyo.dae
    │   ├── urdf                       # urdf folder for xarco files
    │   │   ├── my_robotGoChaseIt.gazebo
    │   │   ├── my_robotGoChaseIt.xacro
    │   ├── world                      # world folder for world files
    │   │   ├── homeGoChaseIt.world
    │   ├── CMakeLists.txt             # compiler instructions
    │   ├── package.xml                # package info
    ├── ball_chaser                    # ball_chaser package                   
    │   ├── launch                     # launch folder for launch files   
    │   │   ├── ball_chaser.launch
    │   ├── src                        # source folder for C++ scripts
    │   │   ├── drive_bot.cpp          # takes commands for and runs the differential-drive
    │   │   ├── process_images.cpp     # searches for the white ball and requests drive_bot.cpp for a service to drive the robot 
    │   ├── srv                        # service folder for ROS services
    │   │   ├── DriveToTarget.srv
    │   ├── CMakeLists.txt             # compiler instructions
    │   ├── package.xml                # package info                  
    └── media                          # screenshots of the world and the robot

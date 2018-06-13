# Project description

An attempt to simulate a robot capable of mapping the scene and register objects movement or deviation from reference map.
The example of such robot is [DOXEL](https://www.doxel.ai/)

![](https://github.com/EgorOs/lidar_building_analysis/blob/master/imgs/rviz.png  "")  

### Required packages

* loam_velodyne

### Installation
    cd ~/catkin_ws/src
    git clone https://github.com/EgorOs/youbot_integration.git
    git clone http://github.com/youbot/youbot_description.git -b kinetic-devel
    git clone https://github.com/youbot/youbot_simulation.git
    git clone https://bitbucket.org/DataspeedInc/velodyne_simulator.git
    git clone https://github.com/team-vigir/flexbe_behavior_engine.git
    https://github.com/EgorOs/youbot_lidar_moveit.git
    cd ~/catkin_ws
    catkin_make

To install octomap use the following lines:

    sudo apt-get install ros-kinetic-octomap-server ros-kinetic-turtlebot ros-kinetic-turtlebot-teleop ros-kinetic-turtlebot-description ros-kinetic-turtlebot-navigation ros-kinetic-turtlebot-rviz-launchers ros-kinetic-turtlebot-simulator ros-kinetic-turtlebot-simulator

### Known issues

* Reinstall gazebo
    sudo apt-get install ros-kinetic-gazebo-ros-pkgs ros-kinetic-gazebo-ros-control
* Install joint state contoroller
    sudo apt-get install ros-kinetic-joint-state-controller

### Usage

    source ~/catkin_ws/devel/setup.bash
    roslaunch youbot_launch youbot_velodyne.launch

### Demo

[Watch video](https://drive.google.com/open?id=1HGKcpqTT_lGjj5pPZCfWLw5elG-Cj0WQ)
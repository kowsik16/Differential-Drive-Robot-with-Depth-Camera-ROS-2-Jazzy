# Differential-Drive-Robot-with-Depth-Camera-ROS-2-Jazzy
URDF and simulation package for a rectangular differential drive robot equipped with a depth camera, built for ROS 2 Jazzy. Includes RViz and Gazebo launch files for visualization, control, and perception.


### Installation

### Clone the Repository:


cd ~/your_workspace_name/src 

git clone https://github.com/kowsik16/differential_drive_robot_with_lidar.git

### Install Dependencies:

sudo apt update && rosdep update

rosdep install --from-paths src --ignore-src -r -y


### Build the Package:

cd ~/your_workspace_name

colcon build --packages-select demo_description

source install/setup.bash


### Launch in RViz:

ros2 launch demo_description display.launch.py


### Launch in Gazebo:

ros2 launch demo_description gazebo.launch.py

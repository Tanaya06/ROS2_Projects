# ROS 2 Jazzy Learning Projects
## Setup
### Installation
sudo apt update
sudo apt upgrade

### Desktop Install (Recommended): ROS, RViz, demos, tutorials.
sudo apt install ros-jazzy-desktop

### ROS-Base Install (Bare Bones): Communication libraries, message packages, command line tools. No GUI tools.
sudo apt install ros-jazzy-ros-base

## Sourcing
echo "source /opt/ros/jazzy/setup.bash">> ~/.bashrc

## Install turtlesim
sudo apt install ros-jazzy-turtlesim
ros2 pkg list --> Should have turtlesim

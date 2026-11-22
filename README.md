# ROS 2 Jazzy Learning Projects
## Setup
### Installation
```bash
sudo apt update
sudo apt upgrade
```

### Desktop Install (Recommended): ROS, RViz, demos, tutorials.
```bash
sudo apt install ros-jazzy-desktop
```

### ROS-Base Install (Bare Bones): Communication libraries, message packages, command line tools. No GUI tools.
```bash
sudo apt install ros-jazzy-ros-base
```

## Sourcing
```bash
echo "source /opt/ros/jazzy/setup.bash">> ~/.bashrc
```

## Install turtlesim
```bash
sudo apt install ros-jazzy-turtlesim
ros2 pkg list #Should have turtlesim
ros2 run turtlesim turtlesim_node # Run turtle sim
```

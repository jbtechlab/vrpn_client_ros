# vrpn_client_ros
VRPN ROS Client

## Only some little changes for ros2-eloquent-devil

# Installation of the VRPN Software 

## Installation of VRPN Driver and Libraries
Create directory, load reposity and installation
```bash
mkdir -p ~/dev_vrpn/src && cd ~/dev_vrpn/src
git clone --recurse-submodules https://github.com/vrpn/vrpn.git
colcon build --merge-install --install-base ../ --packages-select VRPN
```

## Installation of vrpn_ros_client
```bash
cd ~/dev_vrpn/src
git clone --branch ros2 --recurse-submodules https://github.com/metalrod/vrpn_client_ros.git
colcon build --merge-install --install-base ../ --packages-select vrpn_client_ros
```

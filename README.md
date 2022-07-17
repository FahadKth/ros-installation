# ROS-installation
guide for installing ROS on Ubuntu using Virtual box.

***
##  **Step 1 :**
###  Download and install Virtual Box :
choose version for your OS : https://www.virtualbox.org/wiki/Downloads

***

##  **Step 2 :**
### Install Ubuntu 20.04.4 on VM :
Download Ubuntu 20.04.4 : https://releases.ubuntu.com/20.04/ubuntu-20.04.4-desktop-amd64.iso


<img width="960" alt="Screenshot 2022-07-17 220248" src="https://user-images.githubusercontent.com/108236308/179421354-42dc2a2e-e0ba-403e-8c9d-8d7dec3276c6.png">

***

##  **Step 3 :**
### ROS Noetic Installation :
Open the terminal then enter the following commands:

**Set up ROS Noetic repo for Ubuntu 20.04 :**
```
echo "deb http://packages.ros.org/ros/ubuntu focal main" | sudo tee /etc/apt/sources.list.d/ros-focal.list
```
**Add official ROS keyring :**
```
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
```
**Update ROS package index :**
```
sudo apt update
``` 
**Install ROS Noetic package :**
```
sudo apt install ros-noetic-desktop-full
```
**Set up ROS Noetic environment :**
```
source /opt/ros/noetic/setup.bash
```
**Verify Noetic installation :**
```
roscore
```
<img width="960" alt="Screenshot 2022-07-17 224819 123" src="https://user-images.githubusercontent.com/108236308/179422443-ec3aa422-51fc-45f2-aac3-528fccaae2fc.png">


***

## Reference : https://varhowto.com/install-ros-noetic-ubuntu-20-04/

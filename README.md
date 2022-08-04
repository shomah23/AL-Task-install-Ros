# AL-Task-install-Ros
Install Ros on Ubuntu 18.04
Configure your Ubuntu repositories

Configure your Ubuntu repositories to allow "restricted," "universe," and "multiverse." You can follow the Ubuntu guide for instructions on doing this.
# Setup your sources.list
Setup your computer to accept software from packages.ros.org.

$sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" >

$/etc/apt/sources.list.d/ros-latest.list'

# Set up your keys
first: $sudo apt install curl # if you haven't already installed curl

second: $curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -

# Installation
make sure your Debian package index is up-to-date:

$sudo apt update

In case of problems with the next step, you can use following repositories instead of the ones mentioned above ros-shadow-fixed

Desktop-Full Install: (Recommended): 

$sudo apt install ros-melodic-desktop-full

To find available packages, use:

$apt search ros-melodic

# Environment setup

It's convenient if the ROS environment variables are automatically added to your bash session every time a new shell is launched:

$echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc

$source ~/.bashrc

If you just want to change the environment of your current shell you can use:

$source /opt/ros/melodic/setup.bash


# you can use this link you help:
https://www.youtube.com/watch?v=WKlk_2EGfM4&t=568s&ab_channel=MieRobot

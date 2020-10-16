# ROS RViz

This repository demenstrates the basic usage of rviz and rviz config.

## Installing RViz

RViz should be already installed along side with ROS.

```bash
sudo apt-get install ros-$ROS_DISTRO-rviz
```

## Running RViz from terminal

```bash
# Normal way
rosrun rviz rviz
# Quick way
rviz
```

## Running RViz with roslaunch
```xml
<?xml version="1.0" encoding="UTF-8"?>
<launch>

    <node pkg="rviz" type="rviz" name="rviz"/>

</launch>
```

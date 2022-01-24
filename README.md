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

## Running RViz from terminal with custom configuration

```bash
rosrun rviz rviz -d `rospack find ros-rviz`/rviz/config.rviz
```

## Running RViz from roslaunch

This roslaunch script launches rviz with default configurations. The default configuration can usually be found here `/opt/ros/melodic/share/rviz/default.rviz`.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<launch>

    <node pkg="rviz" type="rviz" name="rviz"/>

</launch>
```

## Running RViz from roslaunch with custom configuration

```xml
<?xml version="1.0" encoding="UTF-8"?>
<launch>

    <node pkg="rviz" type="rviz" name="rviz" args="-d $(find ros-rviz)/rviz/config.rviz"/>

</launch>
```

## Reference to RViz Development

https://github.com/ros2/rviz/blob/ros2/docs/plugin_development.md
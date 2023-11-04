# ROS2 installation Tutorial with Binary File

## Follow this tutorial

<https://docs.ros.org/en/humble/Installation/Alternatives/Ubuntu-Install-Binary.html>

to install error will ocurr, it is required to check the ros distribution and append it this command:

```bash
rosdep install --from-paths ~/ros2_humble/ros2-linux/share --ignore-src -y --skip-keys "cyclonedds fastcdr fastrtps rti-connext-dds-6.0.1 urdfdom_headers"
```

its required to add: ```--os=ubuntu:jammy --rosdistro humble```
where ```humble``` comes from the binary downloaded webpage or after running the command: ```rosdep update``` and the current ubuntu distribution where the installation is happening.

## Enable environmene

```bash
# Current env must be located at
# /home/joseamair/ros2_humble
. ~/ros2_humble/ros2-linux/setup.bash
```

## error when enabling ROS2 environment

```bash
. ~/ros2_humble/ros2-linux/setup.bash
[rti_connext_dds_cmake_module][warning] No RTI Connext DDS installation specified.. RTI Connext DDS will not be available at runtime,unless you already configured LD_LIBRARY_PATH manually.
```

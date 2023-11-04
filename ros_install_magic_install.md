# Magic Install Repo for ROS 1 and 2

```bash
wget -c https://raw.githubusercontent.com/qboticslabs/ros_install_noetic/master/ros2_install_humble.sh && chmod +x ./ros2_install_humble.sh && ./ros2_install_humble.sh

```

## Add ros to your bashrc

```bash
 # Replace ".bash" with your shell if you're not using bash
 # Possible values are: setup.bash, setup.sh, setup.zsh
. ~/ros2_humble/ros2-linux/setup.bash
```

## Test installation

Do remove any active enviroment like (conda base). The installation can be test from some commands of this webpage/repo:

<https://docs.ros.org/en/humble/Installation/Alternatives/Ubuntu-Install-Binary.html>

```bash
# One Side
. ~/ros2_humble/ros2-linux/setup.bash
ros2 run demo_nodes_cpp talker

# Second Side
. ~/ros2_humble/ros2-linux/setup.bash
ros2 run demo_nodes_py listener
```

PD: Tested and it works!!

# Orangewood ROS Task

This repository contains the code and setup for the Orangewood ROS Task. The task involves creating a solution using ROS (Robot Operating System) to simulate and control the movement of a turtle in a specific path. The objective is to use ROS to guide the turtle in a rectangular pattern.

## Objective

The goal of this task is to control the movement of a turtle in a rectangular trajectory using ROS, Python, and ROS libraries. The task involves publishing velocity commands to guide the turtle along a defined rectangular path and stopping the turtle once the rectangle is completed.

## Installation and Setup

### Prerequisites

- ROS (Robot Operating System) installed on your machine
- Python 3.x
- ROS workspace set up and sourced (`~/ros_ws` or equivalent)
- Ubuntu 18.04 or newer

### Install ROS and `turtlesim`

Follow these steps to install the required ROS packages and `turtlesim`:

1. **Update and Install ROS Packages**

    ```bash
    sudo apt update
    sudo apt install ros-melodic-ros-tutorials ros-melodic-turtlesim
    sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
    ```

2. **Initialize `rosdep`**

    ```bash
    sudo rosdep init
    rosdep update
    ```

3. **Set up Your ROS Workspace**

    If you haven't already set up your ROS workspace, you can do so by running the following commands:

    ```bash
    mkdir -p ~/ros_ws/src
    cd ~/ros_ws/
    catkin_make
    source devel/setup.bash
    ```

### Clone the Repository

Clone this repository into your `~/ros_ws/src` directory:

```bash
cd ~/ros_ws/src
git clone https://github.com/yourusername/Orangewood-ROS-Task.git
cd ~/ros_ws
catkin_make


---
id: getting-started
title: Rowma: A Reconfigurable Robot Network Construction System
sidebar_label: First Step
---

Rowma is a framework for ROS-based robots that can form a **robot network** easily.

The key features are below:

* Execute a rosrun/roslaunch command over the Internet
* Send a rostopic over the Internet
* Distribute SDKs to develop an application
* Send a rostopic **among an application and a robot** or **between robots**

This video shows an example of controlling a wheeled robot over the Internet from a smartphone.

<iframe width="560" height="315" src="https://www.youtube.com/embed/cOwHWh60PCk" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Getting Started
There are 2 steps to connect your robot to Rowma network.

First, clone `rowma_ros` into your ROS workspace from the GitHub repository (we are planning to upload it to apt repository).

```
$ cd catkin_ws/src
$ git clone https://github.com/rowma/rowma_ros
```

Second, run the node.

**Note that your robot will connect to the default public network for test use.**

```
$ rosrun rowma_ros rowma
```

You would see the output of `Your UUID is: xxxxxx-xxxxxx-xxx-xxx` after your robot successfuly connects to the network. That is your robot's UUID to connect.

The next step is operating the connected robot over the Internet. Open [https://rowma.github.io/sample-application](https://rowma.github.io/sample-application).

First, select the robot's UUID from the select box and push the `Connect` button. After that, you can see a list of rosrun/roslaunch commands in a select box.

Finally, you can push `Run` button after select a command.

<!-- Need figures -->

## System Architecture
This system consists of 3 components: 1) ConnectionManager; 2) Rowma ROS; 3) Application implemented by using a distributed SDK.

This is the overview of the system architecture.

## Acknowledgement
This software is maintained as a part of research in the Cloud Robotics field.

<!--
## Supported Environments
Only ROS1 is supported for now though, we are ready to implement ROS2 version of the package if we have many requests from you.
-->

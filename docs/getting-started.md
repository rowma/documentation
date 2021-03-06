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
* Integrate a robot **easily**
* Reconfigurate robot nodes easily

This video shows an example of controlling a wheeled robot over the Internet from a smartphone.

<iframe width="560" height="315" src="https://www.youtube.com/embed/cOwHWh60PCk" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Getting Started
There are 2 steps to connect your robot to Rowma network.

First, clone `rowma_ros` into your ROS workspace from the GitHub repository (we are planning to upload it to apt repository).

```sh
python <(curl "https://raw.githubusercontent.com/rowma/rowma_ros/master/install.py" -s -N)
```

Second, run the node.

**Note that your robot will connect to the default public network for test use.**

```
$ roscore
$ rosrun rowma_ros rowma
```

![rowma-ros-screenshot](/documentation/img/rowma-ros-screenshot.png)

You would see the output of `Your UUID is: xxxxxx-xxxxxx-xxx-xxx` after your robot successfuly connects to the network. That is your robot's UUID to connect.

The next step is operating the connected robot over the Internet. Open [https://rowma.github.io/public-console](https://rowma.github.io/public-console).

![rowma-public-console](/documentation/img/rowma-public-console.png)

First, select the robot's UUID from the select box and push the `Connect` button. After that, you can see a list of rosrun/roslaunch commands in a select box.

Finally, you can push `Run` button after select a command.

<!-- Need figures -->

## Acknowledgement
This software is maintained as a part of research in the Cloud Robotics field.

<!--
## Supported Environments
Only ROS1 is supported for now though, we are ready to implement ROS2 version of the package if we have many requests from you.
-->

---
id: system-architecture
title: System Architecture
sidebar_label: System Architecture
---

This system consists of 3 components: 1) ConnectionManager; 2) Rowma ROS; 3) Application implemented by using a distributed SDK.

This is the overview of the system architecture.

![overview](/documentation/img/overview.png)

## Rowma Network
The types of Rowma Network are **public** and **private**.

Each Rowma Network has 1 ConnectionManager. So developers can create a private network by hosting ConnectionManager.

**We provide Public Network** for test use and Rowma ROS try to connect the public network **by default**.

And the private-network owner can connect their robots to the network.

![networks](/documentation/img/networks.png)

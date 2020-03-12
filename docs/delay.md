---
id: delay
title: Delay Mesurement
sidebar_label: Delay Mesurement
---

The time lag of Application-to-Robot data transmission and Robot-to-Robot data transmission is investigated.

## TL;DR
The time-lag can be ignored in most cases unless your system is a real-time system that requires 10 ms level response time.

## Method
The measurement was performed by sending data while increasing the data size for one WebSocket connection little by little. Text data of 460 different sizes from 1 byte to 10 MB was used as the data.

The payload format is like following.

```
{
  op: "publish",
  msg: {
    size: "10",
    data: "aaaaaaaaaa"
  },
  timestamp: 1583912257.673818
}
```

## Environment
Only 1 computer was used to conduct this experiment because of avoiding time lag between different machines. This means that 2 Rowma ROS Docker containers ran on 1 computer.

The environment where the ConnectionManager is on the same machine is the L environment, and the environment where the EC2 instance is on the EC2 instance is the C environment.

## Result
This graph is Application-to-Robot transmission delay.

![a2r](/documentation/img/a2r_experiment.png)

This graph is Robot-to-Robot transmission delay.

![r2r](/documentation/img/r2r_experiment.png)

These experiments show that Rowma can transmit data among Application and Robot with relatively low latency (<100ms) if the data size is less than 100KB (e.g. /scan is 10KB-15KB).

## When you feel laggy
Please make sure following points:

* Server location and robot location
* Data size
* Data receiver environment

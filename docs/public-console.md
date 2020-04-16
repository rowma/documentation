---
id: public-console
title: Rowma Public Console
sidebar_label: Rowma Public Console
---

This video shows that `rowma_ros` starts an roslaunch command from Public Console via the Internet.

<iframe width="560" height="315" src="https://www.youtube.com/embed/7Rl0_7da47k" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Setup rowma_ros
Run this command (for more information, see [rowma_ros document](https://rowma.github.io/documentation/en/rowma-ros-overview)).

```sh
python <(curl "https://raw.githubusercontent.com/rowma/rowma_ros/master/install.py" -s -N)
```

## Open Public Console
![public-console](/documentation/img/public-console-screenshot.png)

Access [Public Console](https://rowma.github.io/public-console/). We recommend you to use Google Chrome.

## Run rowma_ros
![first-run-rowma-ros](/documentation/img/first-run-rowma-ros.png)

```
rosrun rowma_ros rowma
```

## Click connect button
![click-connect-button](/documentation/img/click-connect-button.png)

Click the `Connect` button after you see `rowma_ros` starts successfuly.

## Select a robot
![select-robot](/documentation/img/select-robot.png)

Select a robot by UUID that is displayed in the terminal, and click `Connect` button.

## Run a roslaunch
![select-roslaunch](/documentation/img/select-roslaunch.png)

After you click the Connect button, then available commands appears.

You can select a command and click it.

![roslaunch-terminal](/documentation/img/roslaunch-terminal.png)

Finally, a roslaunch command starts over the Internet.

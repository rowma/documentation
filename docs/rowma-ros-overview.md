---
id: rowma-ros-overview
title: Overview
---

`rowma_ros` works as a WebSocket client to receive commands from ConnectionManager and run the received commands.

## Install
You can run the following command below at your terminal.

```sh
python <(curl "https://raw.githubusercontent.com/rowma/rowma_ros/master/install.py" -s -N)
```

```sh
cd ~/catkin_ws/src
git clone https://github.com/rowma/rowma_ros
cd rowma_ros && pip install -r requirements.txt && cd..
```

## Options
There are some options specified at `rosrun`.

|name|value|description|
|:-|:-|:-|
|ROWMA_DEBUG|boolean|Debug logs are shown if you set this value as True.|
|API_KEY|string|API_KEY can be specified for authentication. This value is used along with an authenticator server specified by ROWMA_SERVER_URL.|
|ROWMA_SERVER_URL|string|This value describes ConnectionManager URL. The default value is https://rocky-peak-54058.herokuapp.com.|
|UUID|string|You can use an arbitrary UUID by using this variable.|

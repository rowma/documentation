---
id: host-your-network
title: Host Your Network
sidebar_label: Host Your Network
---

This page explains how to host your own network to the cloud.

## Host on Heroku
You should follow these 3 steps below.

1. Fork [rowma/rowma](https://github.com/rowma/rowma) and clone it
2. Prepare Heroku related processes
3. Push to Heroku

First, clone the repository into your computer.

```
$ git clone https://github.com/rowma/rowma
$ cd rowma
```

Second, you need to install heroku command from [this page](https://devcenter.heroku.com/articles/heroku-cli)

```
$ heroku login
$ heroku create
```

In the end, push it.

```
$ git push heroku master
```

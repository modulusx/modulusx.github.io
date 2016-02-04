---
layout: post
title: Is it cold in here, or is it just me?
---

What do you do when you move into an apartment with no heat? Grab an Electric Imp and start logging the all the environmental data you can of course!

The Electric Imp is a pretty handly little device that happens to do a few things I really like in an IoT device:
* OTA programming!
* A super-simple breakout board for power with a header for sensors
* It costs $30, seriously

One of my old coworkers used to accuse me of often using a Howitzer to kill a Horse Fly but I don't think he was ever bit by one.

## The goal
This started as a simple one. I just wanted to log the environmental data to InfluxDB and graph it with Grafana.

### The components
* An Electric Imp running [this software](https://github.com/modulusx/electric-imp-envtail-to-pubnub)
* An instance of InfluxDB, Grafana, and the hub

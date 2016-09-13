---
title: Is it cold in here, or is it just me?
date: 2016-02-03 00:00:00 Z
layout: post
---

What do you do when you move into an apartment with no heat? Grab an [Electric Imp](https://electricimp.com/) and start logging the all the environmental data you can of course!

### The Goal
This started as a simple one. I just wanted to log the environmental data to InfluxDB and graph it with Grafana. Then I realized I can use Kapacitor to trigger events off of readings in InfluxDB. It might be overkill, and one of my old coworkers used to accuse me of often using a Howitzer to kill a Horse Fly, but I doubt that he was ever bit by one.

## Electric Imp Features
* OTA programming!
* A super-simple breakout board with a GPIO header supporting available [Tails](https://electricimp.com/docs/tails/)
* Priced at only $30 with the [EnvTail](https://electricimp.com/docs/tails/env/)

### Hardware 
* An Electric Imp running [this software](https://github.com/modulusx/electric-imp-envtail-to-pubnub)

### Software
* InfluxDB
* Grafana
* A hub to bind it together

### The results
![_config.yml]({{ site.baseurl }}/images/2016-02-03-imp01-grafana.png)

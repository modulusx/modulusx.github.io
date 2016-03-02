---
layout: post
title: Lights On!
---

I thought having network controlled lights would be amazing, and it is, but sometimes you just need a light switch.

This Thing is really just a WiFi SoC with some buttons and some really crappy software.  It doesn't run on kinetic energy, but then it's not 60 bucks either.

## ESP8266 Thing Features
* At about $16 on Prime, you can't beat the Thing for value.
* Wifi with a Lipo charging circuit on a respectably small board!

### Tell me it doesn't just scream buy me:
![_config.yml]({{ site.baseurl }}/images/2016-03-02-huemote_top.jpg)

### Other necessary hardware
* A Philips Hue Bridge and Lights
* A USB to FTDI serial adapter
* Some buttons and proto board, a 3.7V lipo, mine is from a camera, and a project box.
* You'll need to mash and mangle all of your parts together into some kind of button-shield that will interface with the Thing, someday I'm going to learn CircuitMaker, seriously.

### Check out my mad routing skills
![_config.yml]({{ site.baseurl }}/images/2016-03-02-huemote_bot.jpg)

### The software
* You'll need some kind of rest client, like this really [crappy one](https://github.com/modulusx/esp8266-arduino-restclient), I mean, who doesn't check response codes, or provide even a modest amount of security?
* On top of the rest client, we can write a simple [hue remote](https://github.com/modulusx/esp8266-arduino-hueremote) app to make pretty much any web request, but in this case, we'll make get requests the the Philips Hue bridge to turn lights on and off.

### Customize it
The Hue supports a lot of configuration that their app doesn't expose.  For example, you can create light groups using the API that combine other bulbs (GE anyone?) which lets you control a tri-bulb lamp easily without dumping $180 into the bulbs.

### The end result, one of the ugliest remote controls you've ever seen.
![_config.yml]({{ site.baseurl }}/images/2016-03-02-huemote_box.jpg)

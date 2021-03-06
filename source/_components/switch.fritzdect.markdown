---
layout: page
title: "AVM FRITZ!DECT Switch"
description: "Instructions how to integrate your AVM FRITZ!DECT switches into Home Assistant."
date: 2017-01-24 21:00
sidebar: true
comments: false
sharing: true
footer: true
logo: avm.png
ha_category: Switch
ha_iot_class: "Local Polling"
ha_release: 0.38
---


The `fritzdect` switch platform allows you to control the state of your [AVM FRITZ!DECT DECT-based wireless switches](https://en.avm.de/products/fritzdect/). The AVM FRITZ!DECT switches need to be paired to your Fritz!Box and then can be monitored and controlled via Home Assistant.

Supported devices (tested):

- FRITZ!DECT 200

Supported Firmwares (tested):

- FRITZ!OS: 06.80 / FRITZ!DECT: 03.83
- FRITZ!OS: 06.60 / FRITZ!DECT: 03.83

To use your AVM FRITZ!DECT switch(es) in your installation, add the following to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry
switch:
  - platform: fritzdect
    username: YOUR_USERNAME
    password: YOUR_PASSWORD
```

Configuration variables:

- **username** (*Required*): The username for your Fritz!Box.
- **password** (*Required*): The password for your Fritz!Box.
- **host** (*Optional*): The IP address/hostname of your Fritz!Box. Defaults to `fritz.box`.

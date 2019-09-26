# Hello there! 👋

So this is my Home Assistant instance 🎉

This repository exists mostly for my own amusement, but it may contain some things that others might find useful.

## Statistics from the instance

Description | Value
-- | --
Entities in the [`alarm_control_panel`](https://www.home-assistant.io/components/alarm_control_panel) domain | 1
Entities in the [`automation`](https://www.home-assistant.io/components/automation) domain | 22
Entities in the [`binary_sensor`](https://www.home-assistant.io/components/binary_sensor) domain | 35
Entities in the [`calendar`](https://www.home-assistant.io/components/calendar) domain | 6
Entities in the [`camera`](https://www.home-assistant.io/components/camera) domain | 5
Entities in the [`climate`](https://www.home-assistant.io/components/climate) domain | 2
Entities in the [`cover`](https://www.home-assistant.io/components/cover) domain | 8
Entities in the [`device_tracker`](https://www.home-assistant.io/components/device_tracker) domain | 48
Entities in the [`group`](https://www.home-assistant.io/components/group) domain | 15
Entities in the [`input_boolean`](https://www.home-assistant.io/components/input_boolean) domain | 35
Entities in the [`input_number`](https://www.home-assistant.io/components/input_number) domain | 1
Entities in the [`input_select`](https://www.home-assistant.io/components/input_select) domain | 3
Entities in the [`input_text`](https://www.home-assistant.io/components/input_text) domain | 1
Entities in the [`light`](https://www.home-assistant.io/components/light) domain | 31
Entities in the [`media_player`](https://www.home-assistant.io/components/media_player) domain | 3
Entities in the [`persistent_notification`](https://www.home-assistant.io/components/persistent_notification) domain | 1
Entities in the [`person`](https://www.home-assistant.io/components/person) domain | 2
Entities in the [`scene`](https://www.home-assistant.io/components/scene) domain | 8
Entities in the [`script`](https://www.home-assistant.io/components/script) domain | 13
Entities in the [`sensor`](https://www.home-assistant.io/components/sensor) domain | 452
Entities in the [`sun`](https://www.home-assistant.io/components/sun) domain | 1
Entities in the [`switch`](https://www.home-assistant.io/components/switch) domain | 35
Entities in the [`timer`](https://www.home-assistant.io/components/timer) domain | 1
Entities in the [`vacuum`](https://www.home-assistant.io/components/vacuum) domain | 1
Entities in the [`weather`](https://www.home-assistant.io/components/weather) domain | 2
Entities in the [`weblink`](https://www.home-assistant.io/components/weblink) domain | 5
Entities in the [`zigbee2mqtt_networkmap`](https://www.home-assistant.io/components/zigbee2mqtt_networkmap) domain | 1
Entities in the [`zone`](https://www.home-assistant.io/components/zone) domain | 3
Entities in the [`zwave`](https://www.home-assistant.io/components/zwave) domain | 15
Total state objects | 756

## Hardware and general setup

For my setup I use an old Lenovo Yoga Pro 2, it has a touch screen so I have mounted it on the wall by the front door so I can easily access some controls in my Lovelace UI.

OS | Ubuntu desktop 18.04
-- | --
SSD | 512GB
RAM | 8GB
Processor | Intel® Core™ i7-4500U Processor
Connectivity | WiFi

For the installation method of Home Assistant I went with [the generic Linux installation of Hassio](https://www.home-assistant.io/hassio/installation/#alternative-install-on-a-generic-linux-host)

This method stores the files used by hassio/Home Assistant in `/usr/share/hassio`.

I have mounted a share from my NAS to the `/usr/share/hassio` dir, that way I can handle backups and replication on my NAS.

To have this work I added this line to my `/etc/fstab` file:

```
192.168.2.123:/volume1/SSD/hassio       /usr/share/hassio       nfs     auto    0       0
```

For my theme I use a [custom version](https://paste.ubuntu.com/p/jvVdXM8sY5/) of [slate](https://github.com/seangreen2/slate_theme) theme modified by [@Villhellm](https://github.com/Villhellm) on all my devices.  


To access my instance I'm using my [Nabu Casa ❤️](https://www.nabucasa.com/) link both internally and externally.

## Core integrations that I use

- [AdGuard Home](https://www.home-assistant.io/components/adguard/)
- [Belkin WeMo](https://www.home-assistant.io/components/wemo/)
- [Default Config](https://www.home-assistant.io/components/default_config/)
- [Entur public transport](https://www.home-assistant.io/components/entur_public_transport/)
- [File](https://www.home-assistant.io/components/file/)
- [Input Boolean](https://www.home-assistant.io/components/input_boolean/)
- [LG webOS Smart TV](https://www.home-assistant.io/components/webostv/)
- [Met.no](https://www.home-assistant.io/components/met/)
- [Shell command](https://www.home-assistant.io/components/shell_command/)
- [Speedtest.net](https://www.home-assistant.io/components/speedtestdotnet/)
- [Spotify](https://www.home-assistant.io/components/spotify/)
- [Time & Date](https://www.home-assistant.io/components/time_date/)
- [Wake on LAN](https://www.home-assistant.io/components/wake_on_lan/)

## custom_components that I use

A summary of custom_components that I use.

### [ICY E-thermostaat](https://github.com/custom-components/climate.e_thermostaat)

### [HACS (Home Assistant Community Store)](https://custom-components.github.io/hacs)

_Manage (Install, track, upgrade) and discover custom elements for Home Assistant._

I use this to discover new awesome stuff, and to keep the custom elements I use up to date with the latest version of it from the developer.

This integration has been configured in the UI "Configuration" -> "Integrations", so you will not find my configuration for it.

### [Afvalbeheer](https://github.com/pippyn/Home-Assistant-Sensor-Afvalbeheer)

### [Browser mod]()

### [Breaking Changes](https://github.com/custom-components/breaking_changes)

### [Radarr Upcoming Media](https://github.com/custom-components/sensor.radarr_upcoming_media)

### [ESXi Stats](https://github.com/wxt9861/esxi_stats)

_ESXi component for Home Assistant_

I use this to get information about my ESXi host.

This integration has been configured in the UI "Configuration" -> "Integrations", so you will not find my configuration for it.

### [Postnl](https://www.home-assistant.io/components/postnl)

### [Generate readme](https://github.com/custom-components/readme)

_Generates this awesome readme file._

I use this integration to generate this readme, and to convert my lovelace configuration.

This integration has been configured in the UI "Configuration" -> "Integrations", so you will not find my configuration for it.

### [Sonarr Upcoming Media](https://github.com/custom-components/sensor.sonarr_upcoming_media)


## Custom Lovelace plugins that I use

A summary of custom Lovelace plugins that I use.

### [Compact Custom Header](https://github.com/maykar/compact-custom-header)

_CCH - Customize the header and add enhancements to Lovelace. Features: kiosk mode, conditional header styling, per user/device views, swiping between views on mobile, and more._

I use this to get more screen space by minifying the space used by the header, and to lock my laptop that I have in the hallway by the door to one view.

### [Favicon Counter](https://github.com/custom-cards/favicon-counter)

_Show a notification count badge.._

I use this to show a badge on the Home Assistant tab in my browser when there are active [Persistent notifications](https://www.home-assistant.io/components/persistent_notification/)

### [Mini Graph Card](https://github.com/kalkih/mini-graph-card)

_Minimalistic graph card for Home Assistant Lovelace UI_

I use this to create beautiful statistics cards for my UI.

### [Lovelace Markdown Mod](https://github.com/thomasloven/lovelace-markdown-mod)

_Makes the built-in [markdown](https://www.home-assistant.io/lovelace/markdown/) card better._

I use this to add functions to the markdown card, like showing states of entities.

***

Like all other Home Assistant instances this is also a Work in Progress :D

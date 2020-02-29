# The Depot

This repo contains things that ease my experience with my setup. Will be documented over time as required.

## Bluetooth A2DP issues
Gnome and bluetooth is weird. I've had a device _Failed to set card profile to a2dp_sink_. The fix was:
```shell
setfacl -m u:gdm:r /usr/bin/pulseaudio
sudo pkill pulseaudio
```

# Flickering screen fix for Intel i915 (linux)
...using modprobe.

## Disclaimer
Actions described here may cause damage to your hardware. Do at your own risk.

## Installation and configuration
* Install `intel-gpu-tools`:
```
$ sudo apt-get install intel-gpu-tools
```
* Clone repository and `cd` to it. Change the value `PERIOD` in `root/etc/intelpwm.conf` appropriate for your device (default value working good on ThinkPad X230) See more info at [ArchWiki](https://wiki.archlinux.org/index.php/Backlight#Backlight_PWM_modulation_frequency_.28Intel_i915_only.29).

* After configuration execute following command:
```
$ sudo cp -rn root/* /
```

## Dependencies
* intel-gpu-tools

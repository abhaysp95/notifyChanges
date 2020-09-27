# notifyChanges

Get the notifications for happening of different changes in your WM.

## Features:

Currently included:
* Notification for volume
* Notification for brightness
* Notification for battery status
	+ when battery is charged full
	+ when battery is charging
	+ when battery is discharging
	+ when battery is below critical level
* Notification for song changes(uses `mpc` as client and `mpd` as daemon)

## Screenshots

See the changes for yourself:

* **Volume:**

<!-- ![volume-change](sshots/vol-notify.png) -->
<p align="center">
<img width="720" alt="volume-change" src="sshots/vol-notify.png">
</p>

* **Brightness:**

<!--![bright-change](sshots/bright-notify.png)-->
<p align="center">
<img width="720" alt="bright-change" src="sshots/bright-notify.png">
</p>

* **Battery:**

<!--![battery-charge](sshots/battery_charging.png)-->
<p align="center">
<img width="720" alt="battery-charge" src="sshots/battery_charging.png">

<!--![battery_discharging](sshots/battery_discharging.png)-->
<p align="center">
<img width="720" alt="battery_discharge" src="sshots/battery_discharging.png">
</p>

* **Song:**

<!--![song-change](sshots/music-notify.png)-->
<p align="center">
<img width="720" alt="music-notify" src="sshots/music-notify.png">
</p>

## Usage:

* Use `alert_battery.sh` with some sort of auto-startup program.

You can also checkout my repo for more detailed and some more battery related scripts [here](https://github.com/coolabhays/battery-status)
* Use `getProgressString.sh` inside your desired script or tool to get your desired progress bar look. Checkout `--help` for detail
* Use `mpd_changes.sh` with some sort of auto-startup program like your _wm's config file_ or _.xprofile_ etc.
* Run `notifyChanges.sh --battery` with auto-startup utility same as above ones
* For _volume, brightness_ etc. bind `notifyChanges.sh` with the respected flags to keybinding.

Auto detection for these(volume, brightness etc.) may or may not be added


## Todo:

* Add notification for temprature alert(which tells that CPU is cranking up(atleast in my system))
* Notification for internet connectivity

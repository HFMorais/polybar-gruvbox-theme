# Polybar gruvbox theme


## Screenshots

Defalut view
![screenshot](./screenshots/1.png)

With i3 mode
![screenshot](./screenshots/2.png)


## Requirements
* polybar - 3.7.0 or above


## Install

Backup current config if exists

```sh
mv ~/.config/polybar ~/.config/polybar.backup
```

Download this config

```sh
git clone --depth=1 https://github.com/emgyrz/polybar-gruvbox-theme.git ~/.config/plobar
```

Install fonts
```sh
# JetBrains Mono
best_package_manager install jetbrains-mono 

# Material Icons (Round)
mkdir ~/.fonts && cp -R ~/.config/polybar/fonts/MaterialIcons ~/.fonts/

```


## Configuration

Read polybar [docs](https://github.com/polybar/polybar/wiki).

Update device names:

* `modules/backlight.ini`:`card` - see available cars in `/sys/class/backlight/`
* `modules/battery.ini`:`battery,adapter` - see `/sys/class/power_supply/`
* `modules/temperature.ini`:`zone-type` - see content of `/sys/class/thermal/thermal_zone*/type`
* `modules/wired.ini`:`interface` - net device name can be found with command like `ifconfig`, `ip link` etc
* `modules/wlan.ini`:`interface` - ^

Select visible blocks in `modules.ini`




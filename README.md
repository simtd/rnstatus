# rnstatus - modular POSIX statusbar script for window managers that use "xsetroot -name"

## Dependencies:

* xsetroot
* pkill, pgrep
* light (read backlight level, can be easily changed in rn-modules)
* pactl (read audio information)
* date

## Code structure:

* rnstatus: user interaction, start/stop and update special modules etc.
* rn-modules: functions that provide the actual status text
* rn-stream: runs in backround, handles data stream, updates certain modules on timer

## Output example

* ` Head 10% | Disp 10% | Discharging 35% | Thu 19 May 2022-W20 13:21:31 `

## Usage

```
Usage:
- Run the script: $ rnstatus [start/stop/restart]
- Update special modules: $ rnstatus [volume/backlight]
```
# klipper-config

This repo holds the Klipper configuration files for my Ender 3 Pro. My printer has the following mods:
 - BigTreeTech (BTT) SKR Mini E3 V2.0
 - BL Touch
 - BigTreeTech Smart Filament Sensor (not currently present in config)

## Organization

Files are purposely broken out by function. The `printer.cfg` file is the "entry point" for all others, as it references other files as-needed.


For example, the `skr-mini-e3-v2.cfg` file contains all prerequisite configurations needed to run the SKR Mini E3 V2.0 on an otherwise stock Ender 3 Pro. Likewise, the `bltouch.cfg` file contains everything needed to add a BL Touch sensor to the Ender 3.

The `macros.cfg` file contains a `G29` shim, which translates Marlin-style `G29` (bed leveling) GCode into what Klipper needs to make it run.

---

:warning: This project is a work in progress. Feel free to reference any files here, but know that I may not be able to help with any issues if your printer is substantially different than mine.

---

## TODO:

- [x] Remove bed chain holder
- [x] re-level bed
- [ ] get bl touch offset closer to 1mm if possible
- [ ] turn start up process into macro
- [ ] remove unneccessary travel during start up process
- [ ] measure accel for x axis
- [ ] measure accel for y axis
- [ ] consider voron stealthburner for direct drive w/ pla cooling fan (tbd: jan 2022)
- [ ] reprint mount for filament runout sensor
- [ ] calibrate filament runout sensor
- [x] dual z axis mod
- [ ] x-axis and y-axis belt tensioners
- [ ] x-axis linear rails
- [ ] y-axis linear rails
- [ ] z-axis linear rails
- [ ] z-axis stability/rigidity kit
- [x] hotend upgrade
- [x] noctua silent fan for electronics and hotend
- [x] silencer for part cooling fan?
- [ ] gcode --> script macros for git management of config
- [ ] create filler for wire harness cutout on bottom of chassis
- [ ] put in filament covers for the remaining segments of aluminum extrusion
- [x] consider reverting to older bed leveling knobs
- [ ] print bed leveling knob guide because I'm simply incapable of remembering which way to turn
- [ ] upgraded bl touch cover to better hide the red color because yikes
- [ ] find a way to cover any remaining non-black bits on the printer
- [ ] 3 point bed leveling???
- [ ] second hotend
- [ ] filament dry box out of the rest of the printer stand/frame
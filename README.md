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

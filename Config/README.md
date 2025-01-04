# Siboor Voron Trident 300mm AWD Config
This config is loosely orgonized by device.
Each device has it's own sub folder where hardware connect to each device is then configured.
Macros or other misc. configuration that applies generally to the printer as a whole is kept in the root.

## `Devices.cfg`
Pulls in config files for desired devices.
(Un)Comment devices as necessary.

### BTT Manta m8p v2
Printer main board responsible for:
* Bed heater
* Fans
  * AUX (`fan2`)
  * Fume Pack (`fan3`)
  * Skirt
  * Stepper Drivers
* Day Light LEDs
* Stepper Drivers
  * X0/1
  * Y0/1
  * Z0/1/2

### BTT EBB SB2209 (Siboor stock hw config)
* Standard BMG extruder
* Standard fan configuration
* Standard LED configuration
* Rapido 2 UHF

### Mellow Fly SHT36 v3
* Apus 2 extruder
  * Filament sensor WIP
* Rapido 2 UHF
* Fans
  * Hot end fan
  * Part cooling fan
* LED
  * Defined but commented out

### Cartographer
Includes `[bed mesh]` section.


## Other `.cfg` Files
| File | Description |
| ---- | ----------- |
| `helpers.cfg` | Helper macros |
| `motor_sync.cfg` | Motor Sync module configuration |
| `overrides.cfg` | Homing/Z-tilt overrides |
| `print_actions.cfg` | Contains start/stop/pause/resume/cancel/load/unload |
| `shake_tune.cfg` | Shake tune module configuration |

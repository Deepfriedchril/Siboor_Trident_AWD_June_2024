# Siboor Trident AWD June 2024 Mods

## Hardware Mods
### Add 2040 Corner Brackets
| Extra Parts: ✔ | Recommended: 💯 |
| -------------- | --------------- |

Simple addition that improves frame rigidity.
- [ ] 16x 2040 Brackets
- [ ] m4x10mm BHSC
- [ ] m4 roll-in 2020 nuts

### Flip Rear Motors Downwards
| Extra Parts: ❌ | Recommended: 💯 |
| -------------- | --------------- |

Helps with wiring and gives additional space for other mods.
- [ ] Install the motors upside-down from what is shown in the manual.
- [ ] **Invert** the motor step direction for x1 and y1

### Remove Cable Chain
| Extra Parts: ✔ | Recommended: 💯 |
| -------------- | --------------- |

Vastly improves input shaper graphs and allows for greater accelerations. In place of the cable change I used PG7 cable glands on both ends of the CAN bus cable.
  - [ ] [Bowden PTFE Tube Guide Arm and Can Bus Cable Support](https://www.printables.com/model/978123-voron-bowden-ptfe-tube-guide-arm-and-canbus-cable)
  - [ ] [SB2240 PG7 USB Strain Relief](https://www.printables.com/model/676208-sb2209-sb2240-pg7cnlinko-usb-strain-relief)
  - [ ] [2040 Bracket PG7 Mount](https://www.printables.com/model/1000097-2040-bracket-pg7-mount)
  - *Optional*
	  - [ ] Reprint Fume Pack with PTFE tube side exits
		  - *Note* The Fume Pack provided by Siboor has been modified so that both pan wires exit a _new_ hole in the bottom center instead of each fan wire exiting the port on each fan's side as in the source model. It's easy enough to use a drill and add this hole on to the reprinted part.

### Daylight On A Stick
| Extra Parts: ✔ | Recommended: 💯 |
| -------------- | --------------- |

Huge quality of life improvement to have built in lights that provide plenty of light on the build plate.
- [ ] [Daylight on a Stick](https://github.com/VoronDesign/Voron-Hardware/tree/master/Daylight)
	- There are various retailers that sell premade versions. You ideally want 1 for each side and optionally 1 for the front. 
- [ ] [Mounting Brackets](https://github.com/VoronDesign/Voron-Hardware/blob/master/Daylight/STL/Brackets_2020.stl)
- *Optional*
	- [ ] [Light Baffles](https://www.printables.com/model/315479-daylight-on-a-stick-mount)

### Flat Mesh Skirts
| Extra Parts: ✔ | Recommended: 👍 |
| -------------- | --------------- |

I did not order the decorative parts from Siboor and used the kit to print the rest of the parts once it was in a working state. I choose these skirts instead of the stock ones. Primary benefit is not having a bunch of large holes into the electronics bay.
- [ ] [Flat Mesh Skirts](https://github.com/livinhack/Flat_Mesh_Skirt_Remix_for_Siboor_Trident)

### Panel Clips
| Extra Parts: ✔ | Recommended: 🤷‍♂️ |
| -------------- | ------------------ |

These are an improvement over the standard Voron panel clips but can be a bit brittle with their filament hinges. Once enough break I'll likely try out [Annex clips](https://www.printables.com/model/410806-annex-modified-2020-enclosure-clip).
- [ ] [Filament Latch](https://www.printables.com/model/172368-voron-24-filament-latch-or-any-2020-extrusion)
	- Kit comes with 3mm panel and 3mm foam tape. Print a few test sizes before committing to a full set but the size I ended up on were 5.5mm

### Nozzle Brush
| Extra Parts: ✔ | Recommended: 👎 |
| -------------- | --------------- |

On paper a nozzle brush seems like a great idea however after installing one it seemed to make everything worse. This is likely due to me not using it right but I didn't want to spend any more time on trying to make it work after trying out the line purge from [KAMP](https://github.com/kyleisah/Klipper-Adaptive-Meshing-Purging/tree/main). 
- [ ] Bambu Lab A1 Silicon Brush
- [ ] [Nozzle Scrubber & Decontaminator](https://www.printables.com/model/796563-nozzle-scrubber-decontaminator-for-voron-24-using)
- [ ] [Nozzle Scrubber Arm Extension](https://www.printables.com/model/298565-nozzle-scrubber-arm-extension-voron-trident)

### Glass Panels
| Extra Parts: ✔ | Recommended: ❓ |
| -------------- | -------------- |

My top panel is already showing a bunch of scratches. At some point I'd like to see how replacing the top, sides, and maybe door panels with glass works out. I got a bunch of glass from a guy that redid windows on his house so these will need to be cut down to size and the edges ground down.  

## Software Changes

### Additional Plugins
- [ ] [Motors Sync](https://github.com/MRX8024/motors-sync/blob/main/wiki/EN.md)
	- This plug-in is ran prior to every print to get the motors synced as close as possible.
- [ ] [KAMP](https://github.com/kyleisah/Klipper-Adaptive-Meshing-Purging/tree/main)
	- I only use the adaptive line purge from this plug in.
- [ ] [Cartographer](https://docs.cartographer3d.com/)
	- This is included with the base kit however at the time [Survey Touch](https://docs.cartographer3d.com/cartographer-probe/survey-touch/settings-and-commands) was only in beta. Once fully released I flashed my cartographer with survey and use it at the start of every print.
- [ ] TMC Auto-tune

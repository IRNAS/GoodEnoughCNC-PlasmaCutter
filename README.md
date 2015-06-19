# GoodEnoughCNC-PlasmaCutter

**Good Enough CNC Plasma Cutter - very low cost and simple, suitable for everyone. **

** Work-in-progress, to be published soon.**

Industry in vast majority aims to use highest precision and reliability machines, to be capable of producing even the most complicated parts designers come up with. We are flipping such approach on its head, trading precision of manufacturing tools for simplicity and low cost of their construction, to reduce the entry barrier for using them in any environment. 

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/images/CNC_Plasma-2.jpg)

## Prototype Specifications
Every machine can be tailored to size.
The good enough CNC Plasma cutter is a parametric bootstrap machine. Dimensions depend on the length of the profiles (Parameter L) and profile sizes. The specification below applies for L=1200mm profiles. 


### Frame Metric
 * 40 mm steel tubes
 * 3 mm thickness
 * Frame Imperial
 * 1.5 inch steel tubes
 * 11 gauge

### Trolleys Metric
 * 100 mm steel tubes
 * 3 mm thicknes

### Trolleys Imperial
 * 4 inch steel tubes
 * 11 gauge

### Footprint
 * Width: L+220 mm 
 * Length: L

### Cutting area
 * Width: L-400 mm
 * Length: L-500 mm

### Z travel
 * Height: Z axis rod length - 170 mm

### XY Motion system
 * Timing belt and pulley (T5 or HTD5M or HTD3M or GT2[worst case])
 * Nema 23 motors

### Z Motion system
 * Threaded rod
 * Nema 17 motor

### Plasma
 * Low cost hand held plasma (BMF CUT 50M) or similar
 * THC (Torch height controller)
 * Compressor 30-100 l/min at 2-4 bar – effective 180 l/min

###CNC Controller
Any 4 channel CNC controller, tested:
 * Planet CNC MK3/4 USB Controller
 * Stepper drivers 2.5 A
 * 24 or 48 VDC Power supply





## Features

### Simplicity
Can be manufactured using a hand held drill and angle grinder. Non critical parts are 3D and can be made using other manufacturing processes

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/images/CNC_Plasma.jpg)

### Frame
Low cost Square tubes are used as structural components and linear rails for trolleys. The frame is kept in rectangular position using two turnbuckles. Removing the turnbuckles allows folding the frame for easy transport. 

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/images/Frame_Top_View.jpg)

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/images/Turnbuckles.jpg)

### Trolleys
Low cost square tubes with holes for motor, bearing positions and tightening. Tightening mechanisms compensate for loose tolerances in hole positioning. The result is a exact fit on the frame.

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/images/Trolley.jpg)

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/images/Trolley_inside.jpg)

### Z Axis
Lighter and simpler to manufacture, the Z axis mechanism does not require milled parts like conventional solutions. The torch holder tightly locks the the torch in place without having to modify the handle.

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/images/Z_Axis_CAD.jpg)
![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/images/Z_Axis.jpg)

### Plasma
The Chinese BMF CUT 50M plasma cutter packs more than enough punch to cleanly cut up to 5 mm sheet metal (10 mm max cut). Additionally a compressor and torch height controller is needed.

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/images/Plasma_and_Height_controller.jpg)

## Control system
A number of different CNC controller systems may be applied to this machine. Additionally we have developed an unique fibre optics based interface for the plasma cutter itself, reducing the cost of adding a Torch Height Controller with our custom design, enabling cutting of warped or corrugated surfaces.

## Copyright

Copyright Institute IRNAS Rače 2015. 

This documentation describes Open Hardware and is licensed under the CERN OHL v. 1.2.
You may redistribute and modify this documentation under the terms of the [CERN OHL v.1.2.](http://ohwr.org/cernohl). This documentation is distributed WITHOUT ANY EXPRESS OR IMPLIED  WARRANTY, INCLUDING OF MERCHANTABILITY, SATISFACTORY QUALITY AND FITNESS FOR A PARTICULAR PURPOSE. Please see the CERN  OHL  v.1.2 for applicable conditions.

Any firmware and software are licensed under [GNU General Public License](http://www.gnu.org/licenses/).

Any text and documentation are licensed under `Creative Commons BY-SA` [Attribution-ShareAlike](https://github.com/idleberg/Creative-Commons-Markdown/blob/spaces/4.0/by-sa.markdown)

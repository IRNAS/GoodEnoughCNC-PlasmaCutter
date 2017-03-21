# GoodEnoughCNC-Hybrid

#### ! PLEASE NOTE THAT WE NO LONGER ACTIVELY SUPPORT THIS PROJECT. 

**GoodEnoughCNC Hybrid - very low cost and simple, suitable for everyone. Can be mill, plasma or laser cutter.**

You can find out more on the project website - [goodenoughcnc.eu](http://goodenoughcnc.eu/). Step-by-step assembly instructions are available at [instructions.goodenoughcnc.eu](http://instructions.goodenoughcnc.eu/). 

**Technical files for the last, improved version are available in the folder [HybridCNC_v3](https://github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/tree/master/HybridCNC_v3). Please note that these improvements are not included in the [HybridCNC assembly instructions](http://instructions.goodenoughcnc.eu/).**

Industry in vast majority aims to use highest precision and reliability machines, to be capable of producing even the most complicated parts designers come up with. We are flipping such approach on its head, trading precision of manufacturing tools for simplicity and low cost of their construction, to reduce the entry barrier for using them in any environment. 

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/Images/plasma.jpg)

## Prototype Specifications
Every machine can be tailored to size.
The GoodEnoughCNC Hybrid is a parametric bootstrap machine. Dimensions depend on the length of the profiles (Parameter L) and profile sizes. The specification below applies for L=1200mm profiles. 


### Frame Metric
 * 40 mm steel tubes
 * 3 mm thickness
 

### Trolleys Metric
 * 100 mm steel tubes
 * 3 mm thicknes


### Footprint
 * Width: 1450 mm 
 * Length: 900 mm

### Cutting area
 * Width: L-900 mm
 * Length: L-900 mm

### Z travel
 * Height: Z axis rod length - 150 mm

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

### Frame
Low cost Square tubes are used as structural components and linear rails for trolleys. The frame is kept in rectangular position using two turnbuckles. Removing the turnbuckles allows folding the frame for easy transport. 

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/Images/Frame_Top_View.jpg)

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/Images/Turnbuckles.jpg)

### Trolleys
Low cost square tubes with holes for motor, bearing positions and tightening. Tightening mechanisms compensate for loose tolerances in hole positioning. The result is a exact fit on the frame.

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/Images/Trolley.jpg)

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/Images/Trolley_inside.jpg)

### Z Axis
Lighter and simpler to manufacture, the Z axis mechanism does not require milled parts like conventional solutions. The torch holder tightly locks the torch in place without having to modify the handle.

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/Images/z-axis.jpg)

### Plasma
The Chinese BMF CUT 50M plasma cutter packs more than enough punch to cleanly cut up to 5 mm sheet metal (10 mm max cut). Additionally a compressor and torch height controller is needed.

![GoodEnoughCNC-PlasmaCutter](https://raw.github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/master/Images/Plasma_and_Height_controller.jpg)

## Control system
A number of different CNC controller systems may be applied to this machine. Additionally we have developed an unique fibre optics based interface for the plasma cutter itself, reducing the cost of adding a Torch Height Controller with our custom design, enabling cutting of warped or corrugated surfaces.

### Configuration for CNC control systems
 * Steps per unit X, Y (steps/mm): 67.67 (using 1/16 microstepping by default)
 * Steps per unit Z (steps/mm): 2560 (using 1/16 microstepping by default)
 * Maximum speed X, Y(mm/min): 8000
 * Maximum speed Z (mm/min): 250
 * Acceleration X,Y (mm^2/min): 80
 * Acceleration Z (mm^2/min): 25
 
Setting file for PlanetCNC is [available](goodenoughcnc-hybrid-planetcnc.setting).

### Configuring Goodrive10 VFD inverter for 0.8kW watercooled spindle
Manufacturers [user manual for Goodrive10](http://www.invt.com/UploadFiles/en/Files/2013/9/Goodrive10%20Operation%20Manual(V1.3).pdf) documents well all the features. Spindle specific settings for 0.8kW spindle are, modified from defaults:
 * P00.03 400
 * P00.04 400
 * P02.02 400
 
With this the spindle should run at 24000rpm, note the display either shows 24000 in rpm or 400 in Hz, both representing the same speed.
 
 
## Q&A

[Here](https://github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/blob/master/Q%26A.md) you can read the answers to some frequently asked questions.

---

#### License

All our projects are as usefully open-source as possible.

Hardware including documentation is licensed under [CERN OHL v.1.2. license](http://www.ohwr.org/licenses/cern-ohl/v1.2)

Firmware and software originating from the project is licensed under [GNU GENERAL PUBLIC LICENSE v3](http://www.gnu.org/licenses/gpl-3.0.en.html).

Open data generated by our projects is licensed under [CC0](https://creativecommons.org/publicdomain/zero/1.0/legalcode).

All our websites and additional documentation are licensed under [Creative Commons Attribution-ShareAlike 4 .0 Unported License] (https://creativecommons.org/licenses/by-sa/4.0/legalcode).

What this means is that you can use hardware, firmware, software and documentation without paying a royalty and knowing that you'll be able to use your version forever. You are also free to make changes but if you share these changes then you have to do so on the same conditions that you enjoy.

Koruza, GoodEnoughCNC and IRNAS are all names and marks of Institut IRNAS Rače. 
You may use these names and terms only to attribute the appropriate entity as required by the Open Licences referred to above. You may not use them in any other way and in particular you may not use them to imply endorsement or authorization of any hardware that you design, make or sell.

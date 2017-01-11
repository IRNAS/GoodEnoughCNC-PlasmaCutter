#GoodEnoughCNC Q&A

Here you can read the answers to some frequently asked questions. Please get in touch via [chat](https://chat.irnas.eu/home), [forum](https://goodenoughcnc-hybrid-cnc.readme.io/discuss) or [email](mailto:info@irnas.eu) if you don't find what you're looking for below.

**1. What are the dimensions of GoodEnoughCNC?**

The default version of GoodeenoughCNC machine is 1.1 m x 1.1 m . We do not recommend exceeding the 2 m x 1.2 m dimensions for plasma operations. For milling it depends on your speed and precision requirements.

**2. Is the machining toolhead included in your GoodEnoughCNC kit?**

GoodEnoughCNC kit is the machine without the toolhead, you can mount a
number of different ones on it:

1) Mill : mechanical subtraction of material with a milling bit suitable for most materials ([0.8 kW watercooled spindle](http://fabrikor.eu/goodenoughcnc-hybrid/toolhead-milling-0.8-kw-spindle) available from our store).

2) Plasma: cutting metal with a conductive arc ([plasma cutting torch](http://fabrikor.eu/goodenoughcnc-hybrid/toolhead-plasma-cutting-41) available from our store).

3) Laser: cutting various materials, subject to laser power. We have no laser cutters in our offer at the moment.

**3. Can I cut or engrave MDF with the laser or plasma? The thickest MDF is 18 mm, can your Laser cut it at thoroughly in single pass at that depth?**

MDF you can cut only with a mill, laser cutting it may produce hazardous vapors. You can buy a number of different milling bits for different applications. The spindle we offer uses ER11 collets, meaning it can fit bits with shaft ranging from 1-7 mm.

**4. Can I use my own plasma cutter with GoodEnoughCNC?**

To use any plasma cutter with GoodenoughCNC machine one must 3D print a suitable torch mount, modify the plasma cutter such that cutting can be triggered from the control circuit (for example with GoodenoughCNC optical relay, to be released shortly) and optionally connect a Torch Height Controller unit to the plasma torch.

**5. What software is required to work with GoodEnoughCNC?**

The design and G-code generation is best done with [Autodesk Fusion 360](http://www.autodesk.com/products/fusion-360/overview), free and powerful. You also generally require a PC to run CNC software, you can either choose [Planet-CNC controller](http://fabrikor.eu/goodenoughcnc-hybrid/planet-cnc-usb-controller-mk3-4-4axis) that will be bundled with next generation of GoodenoughCNC Hybrid or use any open-source solution, like Arduino+GRBL and control it with one of many applications that exist, but neither really works that great. [GRBL-panel](https://github.com/gerritv/Grbl-Panel/wiki) seems to be one of the more working ones.

**6. What are configuration settings for CNC Control system?**

A number of different CNC controller systems may be applied to this machine. Additionally we have developed an unique fibre optics based interface for the plasma cutter itself, reducing the cost of adding a Torch Height Controller with our custom design, enabling cutting of warped or corrugated surfaces.

Configuration for CNC control systems
- Steps per unit X, Y (steps/mm): 67.67 (using 1/16 microstepping by default)
- Steps per unit Z (steps/mm): 2560 (using 1/16 microstepping by default)
- Maximum speed X, Y(mm/min): 8000
- Maximum speed Z (mm/min): 250
- Acceleration X,Y (mm^2/min): 80
- Acceleration Z (mm^2/min): 25

Setting file for PlanetCNC is available [here](https://github.com/IRNAS/GoodEnoughCNC-PlasmaCutter/blob/master/goodenoughcnc-hybrid-planetcnc.setting).

**7. We cannot configure the inverter for spindle. Do you have a manual or something so that we can change the rpm of the spindle?**

Configuring Goodrive10 VFD inverter for 0.8 kW watercooled spindle:

[Manufacturers user manual](www.invt.com/UploadFiles/en/Files/2013/9/Goodrive10%20Operation%20Manual(V1.3).pdf) for Goodrive10 documents well all the features. Spindle specific settings for 0.8kW spindle are, modified from defaults:
- P00.03 400
- P00.04 400
- P02.02 400

With this the spindle should run at 24000 rpm, note the display either shows 24000 in rpm or 400 in Hz, both representing the same speed.

**8. The collet falls from the spindle after some time. What can I do?**

Collet falls from spindle if it is rotating anti-clockwise, please check the rotation direction. You can change the direction by swapping the U and W wires on VFD. 

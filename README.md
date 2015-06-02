## A place to freely share Wings 3D Objects
### Electronics Parts for KiCAD 

## Examples
![](https://raw.githubusercontent.com/gruvin/wings3dbits/master/images/led_sm0805_red.jpg)
![](https://raw.githubusercontent.com/gruvin/wings3dbits/master/images/pin_array_2-54_4x1_90.jpg)
![](https://raw.githubusercontent.com/gruvin/wings3dbits/master/images/pin_array_2-54_6x2.jpg)
![](https://raw.githubusercontent.com/gruvin/wings3dbits/master/images/usb-b-smd-micro-socket.jpg)

## Become a Contributor

All Pull requests welcome!

## Conventions

### Dimensions in mm

KiCAD does everything in inches or 1/1000th's of an inch (mils) actually. **We/I do everything in metric**.

So, after exporting a Wings model to VRML format for use in KiCAD (swapping X an Y axis a that point too, is a good idea) you will need to specify a scaling factor of **0.3937** for all three X, Y and Z axis in KiCAD. (Actually, 0.39 will general do the job.)

Some parts will also require either -90 or +90 Z-axis rotation.

### File Naming

```
 primary[_more]_footprint-size_secondary_tertiary.wings
```
... meaning primary part identification, foot print size or designation
(eg. 2.54mm or sm0603 or sot89, etc) secondary or next most important
description, third most important feature.

Also, please be as general as makes sense.

A poor example might be an SOT89 packaged, NPN transistor with BCE
pin ordering ...

```
 transistor_sot89_npn_bce.wings
```

Whilst accurate, this is probably a poor example, because one would
not usually not label the pins on physical transistor or its 3D
graphical representation. Better might something like ...

```
 transistor_sot89.wings
```

An example using secondary and tertiary descriptors might be an
SMD 0805 packaged, blue LED with clear lens ...

```
 led_sm0805_blue_clear.wings
```

Whilst allowed, it is probably best to avoid dots (.) in file names.
Example: a 2.54mm pin pitched, 6 way, 2 row, 90-degree pin array ...

```
 pin_array_2-54mm_6x2_90.wings
```

One may argue that the size, "6x2" is more important than the pin pitch spacing. Let's just use whatever makes the best sense at the time. :-P

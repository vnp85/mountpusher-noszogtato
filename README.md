# Mountpusher - noszogtato

A desktop app to make the telescope follow the planets (or patterns) during recording, by using the ST4 autoguider port on the mount via an Arduino Nano board.

## Getting Started

This project aids the amateur astronomer in keeping the tube pointed to a planet or bright star, or to follow a certain pattern, even with a polar alignment being mediocre, and even with sidereal tracking applied to the Moon's surface details. It's based on the well known ST4 standard for the mount, and some preconditions about the camera: that it is oriented along ra-dec and that the software is preferably SharpCap with its light theme.

The project's desktop part is written in Lazarus, for Windows. The physical device part is based on an Arduino Nano, with the CH340 chip providing a serial interface.

Component TLazSerial from: https://github.com/JurassicPork/TLazSerial

The arduino nano based hardware is very similar to: https://github.com/kevinferrare/arduino-st4  

The desktop app makes distinct beeps to signal status and/or errors. It keeps beeping if expected to guide yet the image goes missing (clouds).

### Prerequisites

A mount with the ST4 guiding port. Cable.

An Arduino compatible device with proper wiring and RJ11/12 port connected to the ST4.

A serial over USB cable connection, the desktop app prefers the CH340 chip found on cheap boards.

A camera to acquire the high resolution images.

A windows laptop or desktop with preferably SharpCap, preferably light (default) theme.

The desktop app running on top of SharpCap.

### Installing

Build the hardware, provision it with the .ino code, install the desktop environment, compile and run the exe. 

Depending on the version, you may want to avoid other CH340 based com ports on the same system.

## Calibration

There is no autocalibration. You may calibrate using the hand controller's autoguiding speed, and by observing and checking the checkboxes: invert ra and/or dec.

## Versioning

I use the YYYY-MM-DD date as the version. Nothing fancy.

## Authors

The sources mention above aside, the sole author is Pal VARADI NAGY. csillagtura.ro

## License

Take it, use it *as is*. Don't sell it, help the others.

## Acknowledgments, other stuff

* My electrical engineer colleagues who helped out an ex-philologist to built such a thing
* The projects mentioned above
* Two decades of astronomy, lessons learnt the hard way



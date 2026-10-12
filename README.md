# Archean

A semi-modular synthesizer built around a Teensy 4.0, made by [Nakedboards](https://nakedboards.online).

Archean combines a monophonic digital voice (wavetable oscillator, software ADSR, LFO) with a
small set of patchable CV/gate I/O, so it behaves like a hybrid between a standalone synth and a
module you can drop into an existing modular rig.

This repository holds the hardware side of the project: schematics, panel/BOM info, and the stock
firmware the instrument ships with.

## Related repositories

Archean can also be driven by typing commands into a terminal instead of (or alongside) its
knobs -- a live-coding workflow built on a small language called Strata. Those live separately,
since both are meant to be reusable beyond this one instrument:

* [archean-live](https://github.com/nakedboards/archean-live) -- the alternate firmware that
  turns Archean into a live-codable instrument.
* [strata](https://github.com/nakedboards/strata) -- the language itself, with no
  Archean-specific code in it, documented on its own.

## What's here

* `firmware/` -- the stock Archean firmware (Arduino/Teensyduino).
* Schematics and panel/BOM files (see the repository's contents -- being filled in).

## Flashing

Archean runs on a Teensy 4.0. To build and flash the stock firmware:

1. Install the [Arduino IDE](https://www.arduino.cc/en/software) and the
   [Teensyduino](https://www.pjrc.com/teensy/teensyduino.html) add-on.
2. Open the `.ino` file under `firmware/` in the Arduino IDE.
3. Select **Tools > Board > Teensy 4.0**.
4. Connect Archean over USB and hit Upload.

To try live coding instead, flash [archean-live](https://github.com/nakedboards/archean-live)
in the same way and see its README.

## About

Archean is designed and built by [Nakedboards](https://nakedboards.online), based in Cebu City,
Philippines. Questions, demos, and updates are posted on
[Instagram](https://instagram.com/nakedboards) and this GitHub account.

## License

MIT.

# Archean

An open-source, monophonic, semi-modular patchable synthesizer built around a Teensy 4.0, made by
[Nakedboards](https://nakedboards.online). Its design is inspired by the Archean eon, an early
period of Earth's development -- it's meant to be a platform for exploration and learning as much
as a musical instrument.

* **Sound engine** -- a single patchable voice covering about seven octaves (16 Hz to 2093 Hz),
  with three waveform modes (randomly generated "landscapes," smoothly evolving terrain, and a
  classic triangle wave), a built-in filter, LFO, ADSR envelope, voltage-controlled delay, and
  numerous patch points for modulation and sound design.
* **Controls** -- a 22-key touch-sensitive keyboard with mineral-shaped keys, and a distance
  sensor that outputs both CV and MIDI-CC for theremin-like expressive control.
* **Connectivity** -- USB-MIDI, MIDI In/Out via 3.5 mm TRS, CV/Gate inputs, line-level and
  Eurorack-level audio outputs, and Eurorack compatibility.
* **Open-source** -- firmware runs on a Teensy 4.0 and is programmable via the Arduino IDE;
  schematics are openly available so components can be replaced and features modified or added.

Full details, specs, and pricing (fully assembled or as a DIY kit) are on the
[product page](https://nakedboards.online/archean).

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

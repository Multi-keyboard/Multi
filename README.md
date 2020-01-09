<p align="center">
  <a href="https://github.com/Multi-keyboard/Multi">
    <img src="docs/resources/logo.png" width="40%">
  </a>
  <h1 align="center"">Main repository</h1>

  <p align="center">
    Main repository for the multifeatured diy keyboard
  </p>
</p>

## Table of contents

- [Table of contents](#table-of-contents)
- [What's that](#whats-that)
- [Structure](#structure)
- [Development process](#development-process)
- [Planned features](#planned-features)
- [Tools](#tools)
  - [Hardware](#hardware)
  - [Software](#software)
- [Quick start](#quick-start)

## What's that

Todo.

## Structure

The project is separated in 4 repositories:

- **[Multi](https://github.com/Multi-keyboard/Multi)**: Contains documentation, and the other 3 repositories as submodules
- **[Multi-software](https://github.com/Multi-keyboard/Multi-software)**: Contains the keyboard's firmware and desktop tools
- **[Multi-hardware](https://github.com/Multi-keyboard/Multi-hardware)**: Contains the keyboard's pcb, case and more
- **[Multi-tests](https://github.com/Multi-keyboard/Multi-tests)**: Preliminary tests for each feature of the keyboard (hardware, software)

## Development process

The goal is to separate the work into multiple, smaller features which can each be designed, built and tested separately to reduce the costs and complexity.

Preliminary development will happen in the `Multi-tests` repository for each feature. Once a first prototype of a feature is successfully built and tested, development will be moved over to the `Multi-software` or `Multi-hardware` repositories.

At some point when enough features have been added, a prototype keyboard will be built and tested.

## Planned features

- :black_medium_square::black_medium_square::black_medium_square: Full size keyboard (104 keys)
- :black_medium_square::black_medium_square::black_medium_square: RGB Backlighting
- :black_medium_square::black_medium_square::black_medium_square: A few modifier keys (FN1, FN2, FN3) to control functionnality
  - Right Windows and Menu buttons replaced by FN1 and FN2 buttons
- :black_medium_square::black_medium_square::black_medium_square: Detachable writst rest
- :black_medium_square::black_medium_square::black_medium_square: Macro GUI editor
- :black_medium_square::black_medium_square::white_medium_square: Key stabilizers for `space, shift, enter, backspace, +, 0`
- :black_medium_square::black_medium_square::white_medium_square: Media keys: play/pause, next
- :black_medium_square::black_medium_square::white_medium_square: Rotary knob to control volume
- :black_medium_square::black_medium_square::white_medium_square: USB 2.0 with Type-C receptacle
- :black_medium_square::black_medium_square::white_medium_square: USB dfu firmware updates
- :black_medium_square::black_medium_square::white_medium_square: USB Passthrough :
  - [USB hub](https://hackaday.io/project/160872-4-port-usb-hub-in-a-square-inch), verify bandwidth of keyboard while transferring files
  - USB2507 for High-Speed USB HUB
  - [TUSB8020B](http://www.ti.com/product/TUSB8020B/toolssoftware) for SuperSpeed USB (hand-solderable :smile:) + reference design
- :black_medium_square::white_medium_square::white_medium_square: On-keyboard macro recording
- :black_medium_square::white_medium_square::white_medium_square: RGB Underglow (if transparent case)
- :black_medium_square::white_medium_square::white_medium_square: Fader or [SliderBar](https://github.com/Haellsigh/SliderBar) on top
- :black_medium_square::white_medium_square::white_medium_square: Cable (either):
  - Custom braided cable (usb+usb+audio)
  - Normal USB Type-C detachable cable (with usb hub on keyboard)
- :black_medium_square::white_medium_square::white_medium_square: Aluminum plate for rigidity
- :black_medium_square::white_medium_square::white_medium_square: Oled display
- :white_medium_square::white_medium_square::white_medium_square: Audio passthrough
- :white_medium_square::white_medium_square::white_medium_square: Hot-swappable switches

## Tools

### Hardware

- **[KiCad](https://kicad-pcb.org/)**: Open-source EDA software
- **[STM32](https://www.st.com/en/microcontrollers-microprocessors/stm32-32-bit-arm-cortex-mcus.html)**: Main microcontroller
- **Cherry MX Brown**: Keyboard switches
- **WS2813 or APA-109B or other**: Fast, addressable LEDs

### Software

- **[VSCode](https://code.visualstudio.com/)**: Code editor for the firmware
- **[PlatformIO](https://platformio.org/)**: VSCode plugin for embedded development
- **[uGFX](https://ugfx.io/)**: Oled display
- **[Docsify](https://docsify.js.org/)**: Documentation
- **[libusb](https://libusb.info/)**: USB communication

## Quick start

Todo.

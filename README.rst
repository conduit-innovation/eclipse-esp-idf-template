==============================
Eclipse IDE & ESP-IDF Template
==============================

This is a template project for Eclipse IDE, supporting the ESP-IDF framework. It's a derivative of `Espressif\'s ESP-IDF template`_.

**Please Note: Windows is not supported by this project at the moment**. Follow `Espressif\'s guide for Windows`_ if you're stuck. Or even better, fire up a Linux VM.

Prerequisites
=============

- `Eclipse`_ CDT (Tested on Oxygen)
- `ESP-IDF`_
- `Xtensa ESP32 Toolchain`_

Getting Started
===============

- Install and set up the above prerequisites
- Ensure that `$IDF_PATH` is set correctly, and the Xtensa toolchain is included in your `$PATH`
- Download or clone this repo
- Run `make menuconfig` from the terminal inside the cloned directory
- Configure your serial programmer, and any other settings. Then save and exit.
- Open Eclipse
- File > Open projects from file system, and select the downloaded directory

That's it. Hopefully building will just work, and you can flash by running the 'flash' target from inside Eclipse (or you can just `make flash` from the command line).

If not, check the paths under Project > Properties > C / C++ Build > Environment. Specifically the IDF_PATH and PATH values. Remember, the bin directory for the Xtensa toolchain needs to be accessible on your PATH.

Code in this repository is Copyright (C) 2016 Espressif Systems, licensed under the Apache License 2.0 as described in the file LICENSE.

.. _ESP-IDF: https://github.com/espressif/esp-idf
.. _Espressif\'s ESP-IDF template: https://github.com/espressif/esp-idf-template
.. _Espressif\'s guide for Windows: http://esp-idf.readthedocs.io/en/latest/get-started/eclipse-setup-windows.html#eclipse-windows-setup
.. _`Xtensa ESP32 Toolchain`: http://esp-idf.readthedocs.io/en/latest/get-started/index.html#setup-toolchain
.. _`Eclipse`: http://www.eclipse.org/downloads/packages/eclipse-ide-cc-developers/oxygen1a

# Compiling Sinclair related tools and programs for macOS Silicon
Short HOW TO's for compiling Sinclair related programs for macOS on Silicon

In general [Homebrew](https://brew.sh/) and XCode is required for being able to compile.

* libspectrum
* Fuse (ZX Spectrum Emulator)
* Fuse-utils
* sz81 (ZX81 Emulator)
* sjamsplus (Assembler)
* pasmo (Assembler)
* tzxtools (suite of TZX tools)


## libspectrum
A library required by a few tools, such as Fuse and Fuse-utils

* Clone the source code from [GITHUB](https://github.com/speccytools/libspectrum) - `git clone https://github.com/speccytools/libspectrum`
* Change to folder with code and configure the build - `cd libspectrum && autoreconf -i && ./configure`
* Build the code - `make`
* Install required files globally (requires root access) - `sudo make install`

## Fuse - the Free Unix Spectrum Emulator
For compiling the X11/GTK version of Fuse for macOS:

## Fuse-utils

## zxsp - ZX Spectrum emulator for macos

## sz81 (ZX81 Emulator)

## sjamsplus (Assembler)

## pasmo (Assembler)

## tzxtools (suite of TZX tools)

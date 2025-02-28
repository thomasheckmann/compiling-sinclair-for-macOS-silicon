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

* Jump to a folder where you will keep the project - `cd <my code folder>`
* Clone the source code from [GITHUB](https://github.com/speccytools/libspectrum) - `git clone https://github.com/speccytools/libspectrum`
* Change to folder with code and configure the build - `cd libspectrum && autoreconf -i && ./configure`
* Build the code - `make`
* Install required files globally (requires root access) - `sudo make install`

## Fuse - the Free Unix Spectrum Emulator
For compiling the X11/GTK version of Fuse for macOS:

Requires:
* X11 (XQuartz on macOS)
* GTK
* libspectrum (see above)

Build:
* Jump to a folder where you will keep the project - `cd <my code folder>`
* Downloads source code for [Fuse-1.6.0](https://sourceforge.net/projects/fuse-emulator/files/fuse/1.6.0/fuse-1.6.0.tar.gz/download)
* Unpack archive - `tar zxvf fuse-1.6.0.tar.gz`
* Change to folder with code and configure the build - `cd fuse-1.6.0 && ./configure`
* Build the code - `make`
* Test by launching fuse - `./fuse`


## Fuse-utils

Requires:
* libspectrum (see above)

Build:
* Jump to a folder where you will keep the project - `cd <my code folder>`
* Downloads source for [Fuse-utils-1.4.3](https://sourceforge.net/projects/fuse-emulator/files/fuse-utils/1.4.3/fuse-utils-1.4.3.tar.gz/download)
* Unpack archive - `tar zxvf fuse-utils-1.4.3.tar.gz`
* Change to folder with code and configure the build - `cd fuse-utils-1.4.3 && ./configure`
* Build the code - `make`


## zxsp - ZX Spectrum emulator for macos

## sz81 (ZX81 Emulator)

## sjamsplus (Assembler)

## pasmo (Assembler)

## tzxtools (suite of TZX tools)

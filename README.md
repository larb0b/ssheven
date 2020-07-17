![ssheven box](http://www.cy384.com/media/img/ssheven_box_front_small.png)

ssheven
-------
A modern SSH client for Mac OS 7/8/9 on m68k and PPC machines.

Project status: as of 0.1.0 (see github releases), an actual SSH client, with a zero-features "vanilla" fixed-size terminal

* encryption libraries: ham-handedly ported and fairly functional
* console emulation: very basic, no escape codes or anything yet (to be implemented with libvterm soon)
* UI/UX: it quits when you click the close button! (i.e. basically nothing yet)

build
-----
More details to come as functionality is added.

Uses Retro68 and cmake.

Requires mbedtls and libssh2, see my (cy384's) ports of those libraries for details.  Note that you need to make/install them for both platforms if you want to build for both platforms.

* `mkdir build && cd build`
* `cmake .. -DCMAKE_TOOLCHAIN_FILE=/your/path/to/Retro68-build/toolchain/powerpc-apple-macos/cmake/retroppc.toolchain.cmake` or `cmake .. -DCMAKE_TOOLCHAIN_FILE=/your/path/to/Retro68-build/toolchain/m68k-apple-macos/cmake/retro68.toolchain.cmake`
* `make`

license
-------
Licensed under the BSD 2 clause license, see LICENSE file.


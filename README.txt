For msys2/mingw64 needed switch in linking -Wl,--allow-multiple-definition is required to build exe. Use make -f Makefile.mingw64
See: https://www.youtube.com/watch?v=l_yjcm5dihg for setup of build environment under w11.


MnvM_bld: README
Paul C. Pratt
www.gryphel.com
July 27, 2005


MnvM_bld is the build system for Mini vMac,
a miniature Macintosh emulator.

Further information may be found at
"http://minivmac.sourceforge.net/".


You can redistribute MnvM_bld and/or modify it under the terms
of version 2 of the GNU General Public License as published by
the Free Software Foundation.  See the included file COPYING.

MnvM_bld is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
license for more details.

---

What is MYSYS2?
MSYS2 is a collection of tools and libraries providing you with an easy-to-use environment for building, installing and running native Windows software.

What is SDL2?
Simple DirectMedia Layer is a cross-platform development library designed to provide low level access to audio, keyboard, mouse, joystick, and graphics hardware via OpenGL and Direct3D. It is used by video playback software, emulators, and popular games including Valve's award winning catalog and many Humble Bundle games. 

Get MSYS2:
https://www.msys2.org/

Get SDL2
https://libsdl.org/

Commands used in the above video:
pacman -Syu

pacman -S git mingw-w64-x86_64-gcc mingw-w64-x86_64-toolchain mingw64/mingw-w64-x86_64-SDL2 mingw64/mingw-w64-x86_64-SDL2_mixer mingw64/mingw-w64-x86_64-SDL2_image mingw64/mingw-w64-x86_64-SDL2_ttf mingw64/mingw-w64-x86_64-SDL2_net mingw64/mingw-w64-x86_64-cmake make

gcc "name of file".c -o "executable name".exe $(pkg-config --cflags --libs sdl2)

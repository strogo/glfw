# GLFW

## Introduction

GLFW is a free, Open Source, multi-platform library for OpenGL and OpenGL ES
application development.  It provides a simple, platform-independent API for
creating windows and contexts, reading input, handling events, etc.

Version 3.1 is *not yet described*.

If you are new to GLFW, you may find the
[introductory tutorial](http://www.glfw.org/docs/latest/quick.html) for GLFW
3 useful.  If you have used GLFW 2 in the past, there is a
[transition guide](http://www.glfw.org/docs/latest/moving.html) for moving to
the GLFW 3 API.


## Compiling GLFW

See the [Compiling GLFW](http://www.glfw.org/docs/latest/compile.html) guide in
the GLFW documentation.


## Using GLFW

See the
[Building programs that use GLFW](http://www.glfw.org/docs/latest/build.html)
guide in the GLFW documentation.


## Dependencies

GLFW bundles a number of dependencies in the `deps/` directory.

The following dependencies are needed by GLFW:

 - [Khronos extension headers](https://www.opengl.org/registry/)

The following dependencies are needed by the examples and test programs:

 - [getopt\_port](https://github.com/kimgr/getopt_port/) for getopt
 - [TinyCThread](https://gitorious.org/tinythread/tinycthread/) for threading
 - An OpenGL loader generated by [glad](https://github.com/Dav1dde/glad)


## Changelog

 - Added native monitor handle access to native API
 - Added `glfwSetDropCallback` and `GLFWdropfun` for receiving dropped files
 - Bugfix: The debug context attribute was set from `GL_ARB_debug_output` even
           when a debug context had not been requested
 - Bugfix: The particles example was not linked against the threading library
 - [Cocoa] Added `_GLFW_USE_RETINA` to control whether windows will use the full
           resolution on Retina displays
 - [Cocoa] Bugfix: Using a 1x1 cursor for hidden mode caused some screen
                   recorders to fail
 - [Cocoa] Bugfix: Some Core Foundation objects were leaked during joystick
                   enumeration
 - [Win32] Enabled generation of pkg-config file for MinGW
 - [Win32] Bugfix: Failure to load winmm or its functions was not reported to
                   the error callback
 - [X11] Made GLX 1.3 the minimum supported version
 - [X11] Bugfix: The case of finding no usable CRTCs was not detected
 - [X11] Bugfix: Detection of broken Nvidia RandR gamma support did not verify
                 that at least one CRTC was present
 - [X11] Bugfix: A stale `_NET_SUPPORTING_WM_CHECK` root window property would
                 cause an uncaught `BadWindow` error
 - [X11] Bugfix: No check was made for the presence GLX 1.3 when
                 `GLX_SGIX_fbconfig` was unavailable
 - [X11] Bugfix: The message type of ICCCM protocol events was not checked


## Contact

The official website for GLFW is [glfw.org](http://www.glfw.org/).  There you
can find the latest version of GLFW, as well as news, documentation and other
information about the project.

If you have questions related to the use of GLFW, we have a
[support forum](https://sourceforge.net/p/glfw/discussion/247562/), and the IRC
channel `#glfw` on [Freenode](http://freenode.net/).

If you have a bug to report, a patch to submit or a feature you'd like to
request, please file it in the
[issue tracker](https://github.com/glfw/glfw/issues) on GitHub.

Finally, if you're interested in helping out with the development of GLFW or
porting it to your favorite platform, we have an occasionally active
[developer's mailing list](https://lists.stacken.kth.se/mailman/listinfo/glfw-dev),
or you could join us on `#glfw`.


## Acknowledgements

GLFW exists because people around the world donated their time and lent their
skills.

 - Bobyshev Alexander
 - artblanc
 - arturo
 - Matt Arsenault
 - Keith Bauer
 - John Bartholomew
 - Niklas Behrens
 - Niklas Bergström
 - Doug Binks
 - blanco
 - Lambert Clara
 - Andrew Corrigan
 - Noel Cower
 - Jarrod Davis
 - Olivier Delannoy
 - Paul R. Deppe
 - Michael Dickens
 - Jonathan Dummer
 - Ralph Eastwood
 - Michael Fogleman
 - Gerald Franz
 - GeO4d
 - Marcus Geelnard
 - Stefan Gustavson
 - Sylvain Hellegouarch
 - heromyth
 - Paul Holden
 - Toni Jovanoski
 - Osman Keskin
 - Cameron King
 - Peter Knut
 - Robin Leffmann
 - Glenn Lewis
 - Shane Liesegang
 - Дмитри Малышев
 - Martins Mozeiko
 - Tristam MacDonald
 - Hans Mackowiak
 - Kyle McDonald
 - David Medlock
 - Jonathan Mercier
 - Marcel Metz
 - Kenneth Miller
 - Bruce Mitchener
 - Jack Moffitt
 - Jeff Molofee
 - Jon Morton
 - Pierre Moulon
 - Julian Møller
 - Kamil Nowakowski
 - Ozzy
 - Andri Pálsson
 - Peoro
 - Braden Pellett
 - Arturo J. Pérez
 - Pieroman
 - Jorge Rodriguez
 - Ed Ropple
 - Riku Salminen
 - Sebastian Schuberth
 - Matt Sealey
 - SephiRok
 - Steve Sexton
 - Systemcluster
 - Dmitri Shuralyov
 - Daniel Skorupski
 - Bradley Smith
 - Julian Squires
 - Johannes Stein
 - Justin Stoecker
 - Nathan Sweet
 - TTK-Bandit
 - Sergey Tikhomirov
 - Samuli Tuomola
 - urraka
 - Jari Vetoniemi
 - Simon Voordouw
 - Torsten Walluhn
 - Jay Weisskopf
 - Frank Wille
 - yuriks
 - Santi Zupancic
 - Lasse Öörni
 - All the unmentioned and anonymous contributors in the GLFW community, for bug
   reports, patches, feedback, testing and encouragement


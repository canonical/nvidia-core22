# Nvidia and Mesa libraries for core22 snaps

A content snap providing the Nvidia and Mesa userspace libraries and
drivers for `base: core22` snaps.

This supplies the graphics-core22 content interface:

Path|Description|Use
--|--|--
bin/graphics-core22-provider-wrapper|Sets up all the environment|Run your application through it
||
drirc.d|App-specific workarounds|Layout to /usr/share/drirc.d
libdrm|Needed by mesa on AMD GPUs|Layout to /usr/share/libdrm
X11|X11 locales etc|Layout to /usr/share/X11
||
mir-quirks|(optional)Mir configuration|Mir specific

----

For more information about the `graphics-core22` interface, see: [The graphics-core22 snap interface](https://mir-server.io/docs/the-graphics-core22-snap-interface) documentation.

The repository license is GPL v3 with copyright Canonical LTD 2023,
however the license of the actual content snap is mixed license
(proprietary NVIDIA for NVIDIA libraries, and various open source
licenses for all other libraries). Installing this snap implies
accepting NVIDIA license terms.

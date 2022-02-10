# nvidia and mesa libraries for core22 snaps

A content snap providing the nvidia and mesa userspace libraries and
drivers for core22

This supplies the graphics-core22 content interface:

    .../lib contains the mesa shared libraries (add to LD_LIBRARY_PATH)
    .../dri contains the mesa drivers (set LIBGL_DRIVERS_PATH/LIBVA_DRIVERS_PATH to this)
    .../glvnd/egl_vendor.d contains the mesa ICD (set __EGL_VENDOR_LIBRARY_DIRS to this)
    .../etc/mir-quirks contains any Mir configuration for driver support (none for mesa)
    .../libdrm contains mesa configuration for driver support (layout to /usr/share/libdrm) 
    .../drirc.d contains mesa app-specific workarounds (layout to /usr/share/drirc.d) 

----

For details on how to get NVIDIA drivers see
[NVIDIA-assemble](https://github.com/xnox/nvidia-assemble) snap.

For details of the graphics-core22 content interface see:

https://discourse.ubuntu.com/t/the-graphics-core20-snap-interface/23000

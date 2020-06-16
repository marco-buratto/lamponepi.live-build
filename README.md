# Lampone Pi, live building

Lampone Pi is a live Debian arm64 port for the Raspberry Pi.

Here are the instructions on how to build the live image compatible with a Raspberry Pi. 
A Debian arm64 host is required (use qemu).

**\
\
Live build: create the ISO**

Clone or download this GitHub repository and change the current directory to it.

A patched live-build program is needed for a correct live-building. 
The .deb package of live-build patched by our Team must be installed as the first step:

    dpkg -i live-build2019031131_all.deb
    apt install -fy

Live building is now trivial:

    cd live-build
    
    lb config
    lb build

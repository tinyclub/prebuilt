
# ARM toolchain

This is downloaded from http://newos.org/toolchains/arm-eabi-5.3.0-Linux-x86_64.tar.xz

## Decompress

    tar Jxf arm-eabi-5.3.0-Linux-x86_64.tar.xz -C /opt

## Setting up environment in ~/.bashrc:

    export PATH=/opt/arm-eabi-5.3.0-Linux-x86_64/bin:$PATH
    export LD_LIBRARY_PATH=/opt/arm-eabi-5.3.0-Linux-x86_64/lib:$LD_LIBRARY_PATH

## Download, build and boot little kernel

    git clone https://github.com/littlekernel/lk
    cd lk
    ./scripts/do-qemuarm

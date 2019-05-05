
# ARM toolchain

https://releases.linaro.org/components/toolchain/binaries/

## Download & Decompress

    $ make toolchain

## Configure and use it

    $ vim boards/virt/Makefile
    CCVER ?= 8.3-2019.03
    CCPATH ?= $(PREBUILT_TOOLCHAINS)/$(XARCH)/gcc-arm-$(CCVER)-x86_64-aarch64-linux-gnu/bin/ 

## Use it

    $ make kernel-defconfig
    $ make kernel

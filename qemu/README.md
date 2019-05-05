
For prebuilt qemu, linaro ppa is another choice (only for ARM/ARM64):

<https://wiki.linaro.org/WorkingGroups/ToolChain/QEMU>

Install them, for example:

    sudo add-apt-repository -y ppa:linaro-maintainers/tools
    sudo apt-get -y update
    sudo apt-get install qemu-system-arm

but it also depends on Ubuntu version, so, to get newer qemu version, we may
must compile it ourselves.

    $ make emulator-download
    $ make emulator-defconfig
    $ make emulator
    $ make emulator-save

The self-compiled qemu files will be stored in prebuilt/qemu/XARCH/QEMU/ by
default, the qemu-system-XARCH is stored in prebuilt/qemu/XARCH/QEMU/bin

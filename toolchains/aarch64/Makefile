VERSION ?= 8.3-2019.03

#VERSION=7.4-2019.02
#SUBVERSION=7.4.1-2019.02
#LINARO_BASE=gcc-linaro-$(SUBVERSION)-x86_64_aarch64-linux-gnu
#LINARO_URL=https://releases.linaro.org/components/toolchain/binaries/$(VERSION)/aarch64-linux-gnu/$(LINARO_BASE).tar.xz

ARM_BASE=gcc-arm-$(VERSION)-x86_64-aarch64-linux-gnu
ARM_URL=https://developer.arm.com/-/media/Files/downloads/gnu-a/$(VERSION)/binrel/$(ARM_BASE).tar.xz

TOOLCHAIN=$(ARM_URL)

all:
	wget -c $(TOOLCHAIN)
	tar Jxvf $(shell basename $(TOOLCHAIN))

clean:
	rm -rf $(TOOLCHAIN)

TOOLCHAIN=gcc-8

all:
	add-apt-repository -y ppa:ubuntu-toolchain-r/test
	apt-get -y update
	apt-get install -y --force-yes $(TOOLCHAIN)
	update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-8 46

clean:
	apt-get remove $(TOOLCHAIN)

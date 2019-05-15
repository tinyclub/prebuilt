
# Docker images for full rootfs

list available docker images containing a full root with package management tool.

## ARM

* ARM32 / arm
  - Ubuntu
    - arm32v7/ubuntu (18.04)
    - tinylab/arm32v7-ubuntu (18.04)
  - Busybox
    - arm32v7/busybox

* ARM64 / aarch64
  - Ubuntu
    - arm64v8/ubuntu (18.04)
  - Busybox
    - arm32v7/busybox

## MIPS

* MIPS32 / mipsel
  - aoqi/debian-mipsel

* MIPS64 / mips64el
  - aoqi/debian-mips64el

## PPC

* PPC64 / ppc64sel
  - ppc64le/ubuntu

## X86

* X86_32 / i386
  - i386/ubuntu

* X86_64 / x86_64
  - ubuntu

## More

Search more from docker images repository:

    $ docker search ppc | grep ubuntu

Extrat one:

    $ tools/rootfs/docker/extra.sh arm64v8/ubuntu aarch64

Run with docker:

    $ tools/rootfs/docker/run.sh arm64v8/ubuntu aarch64

Run with chroot:

    $ tools/rootfs/docker/chroot.sh arm64v8/ubuntu

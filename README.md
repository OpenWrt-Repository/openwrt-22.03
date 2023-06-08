## OpenWrt 22.03 with support for Arcadyan/Astoria Easybox 904 xDSL (VGV952CJW33-E-IR)
[![Openwrt](https://img.shields.io/badge/os-OpenWrt-<COLOR>.svg)](https://github.com/OpenWrt-Repository/) [![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://github.com/OpenWrt-Repository/openwrt#license)

## Kernel 5.10 compilation error - work in progress!
```
drivers/net/phy/mdio_bus.c: redefinition of 'mdio_find_bus'
```

### Requirements

You need the following tools to compile OpenWrt, the package names vary between
distributions. A complete list with distribution specific packages is found in
the [Build System Setup](https://openwrt.org/docs/guide-developer/build-system/install-buildsystem)
documentation.

```
gcc binutils bzip2 flex python3 perl make find grep diff unzip gawk getopt
subversion libz-dev libc-dev rsync which
```

### Quickstart

1. Run `./scripts/feeds update -a` to obtain all the latest package definitions
   defined in feeds.conf / feeds.conf.default

2. Run `./scripts/feeds install -f` and `./scripts/feeds install -a` to install symlinks for all obtained
   packages into package/feeds/

3. Run `make menuconfig` to select your preferred configuration for the
   toolchain, target system & firmware packages.

4. Run `make V=sc` to build your firmware. 
   
### Other

* [Firmware Recovery with GUI](https://github.com/zuzia-dev/Easybox-904xDSL)
* [Repository of compiled images and packages](https://github.com/zuzia-dev/Easybox-904xDSL-repo-source)
* [The official OpenWrt forum](https://forum.openwrt.org/t/lantiq-xrx200-easybox-904xdsl-and-speedport-w-921v-build/77105)

## License

OpenWrt is licensed under GPL-2.0
> It based on https://github.com/Plonkbong/openwrt/tree/xrx200-21.02.2


The celerate openwrt firmware builder.

What the prepare script does:

1. Downloads OpenWRT

2. Patches OpenWRT.

# Usage

## Requirements

The openwrt wiki has some examples of requirements per distro:
http://wiki.openwrt.org/doc/howto/buildroot.exigence#examples.of.package.installations

Their example for ubuntu 64-bit is:
    sudo apt-get install build-essential subversion libncurses5-dev zlib1g-dev gawk gcc-multilib flex git-core gettext quilt ccache libssl-dev xsltproc

## Build All

Build firmware and all packages from scratch:

    git clone https://github.com/denovo/celerate-openwrt-firmware.git
    cd sudowrt-firmware
    ./prepare
    ./build

Something magical will appear, this is the firmware, under e.g. `built_firmware/ar71xx/bin/`

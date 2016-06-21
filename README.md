# Lab7 Systems Ubuntu/Debian packaging

This repository contains the Debian/Ubuntu packaging sources used to create the
packages in the
"[chenghlee/lab7io](https://launchpad.net/~chenghlee/+archive/ubuntu/lab7io)"
personal package archive (PPA). [Lab7 Systems](https://www.lab7.io) uses these
packages to support various internal development projects but is making them
publicly available in hopes others will also find them useful.

**NOTE**: this repository contains only those files needed to generate `.deb`
packages from upstream sources (i.e., the files in the `debian` subdirectory).
It does *not* contain the upstream sources nor the `.deb` packages (i.e., this
cannot be used as an apt repository).

To actually make use of the packages on an Ubuntu system, you will need to run
the following:
```bash
sudo apt-get install software-properties-common   # if not already installed
sudo add-apt-repository ppa:chenghlee/lab7io
```
The signing key for the PPA is [1024R/D35D1042](http://keyserver.ubuntu.com:11371/pks/lookup?fingerprint=on&op=index&search=0x8EBDBFE661B6ABEFE1395D73B1503307D35D1042), created on 2012-09-05.

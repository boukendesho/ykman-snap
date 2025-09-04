## ykman-snap
[![ykman](https://snapcraft.io/ykman/badge.svg)](https://snapcraft.io/ykman)
 
[![ykman](https://img.shields.io/github/v/release/Yubico/yubikey-manager?logo=github)](https://github.com/Yubico/yubikey-manager)

Configure your YubiKey via the command line.

### Known issues: Pcscd: Communication protocol mismatch!

> Ykman warnnings:
> WARNING: PC/SC not available. Smart card (CCID) protocols will not function.
> ERROR: Unable to list devices for connection

Ubuntu 24.10  above or pcscd > 2.3.0 version will  likely encounter this problem.
Details: https://github.com/Yubico/yubioath-flutter/issues/1725

Please try the edge channel build.

```bash
$ sudo snap refresh ykman --edge
```

### Authors

This snap is maintained by me, and is not necessarily endorsed or officially maintained by the upstream developers. If you encounter any issues, please kindly report it here.

Caution: you will need `pcscd` installed and running . 

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/ykman)

## Requirements

[Snap installed](https://snapcraft.io/docs/installing-snapd)

## Install

```bash
$ sudo apt install pcscd # Must have, otherwise smartcard functions will not work.
$ sudo snap install ykman
```

## Usage

see: [Official Docs](https://docs.yubico.com/software/yubikey/tools/ykman/Using_the_ykman_CLI.html)


## Data & Config file location

Due to the packaging with Snap, the default paths are different.

- Default config directory: /home/$USER/snap/ykman/current/



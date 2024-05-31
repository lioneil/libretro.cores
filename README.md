# libretro.cores/aarch64

A repository for pre-built 64-bit linux (arm64 or aarch64) RetroArch Libretro Cores. These cores are ideal for arm-based linux builds typically for retro handhelds (e.g. Anbernic RG ARC-S or ARC-D).

## Supported Cores

All supported cores can be downloaded from the [Releases](https://github.com/lioneil/libretro.cores/releases) section or directly from the table below.

| Core | Nightly builds |
| :--- | :------------- |
| FBNeo | [![FBNeo libretro Linux aarch64](https://github.com/lioneil/libretro.cores/actions/workflows/fbneo-libretro.yml/badge.svg?branch=main)](https://github.com/lioneil/libretro.cores/releases/download/Linux_aarch64/fbneo_libretro.so.zip) |
| Flycast | [![Flycast libretro Linux aarch64](https://github.com/lioneil/libretro.cores/actions/workflows/flycast-libretro.yml/badge.svg?branch=main)](https://github.com/lioneil/libretro.cores/releases/download/Linux_aarch64/flycast_libretro.so.zip) |

## RetroArch Core Settings

Optionally, you can make this repository your main source of cores.

In RetroArch, go to Online Updater > Updater Settings and change value for Buildbot Cores URL to:

```
https://github.com/lioneil/libretro.cores/releases/download/Linux_aarch64/
```

Or in `retroarch.cfg`, add/overwrite the key-value pair:

```cfg
core_updater_buildbot_cores_url = "https://github.com/lioneil/libretro.cores/releases/download/Linux_aarch64/"
```

# libretro.cores/aarch64

A repository for pre-built 64-bit linux (arm64 or aarch64) RetroArch Libretro Cores. These cores are ideal for arm-based linux builds typically for retro handhelds (e.g. Anbernic RG ARC-S or ARC-D).

## Supported Cores

All supported cores can be downloaded from the [Releases](https://github.com/lioneil/libretro.cores/releases) section or directly from the table below.

| Core | Nightly builds |
| :--- | :------------- |
| FBNeo | [![FBNeo libretro Linux aarch64](https://github.com/lioneil/libretro.cores/actions/workflows/fbneo-libretro.yml/badge.svg?branch=main)](https://github.com/lioneil/libretro.cores/releases/download/Linux_aarch64/fbneo_libretro.so.zip) |
| Flycast | [![Flycast libretro Linux aarch64](https://github.com/lioneil/libretro.cores/actions/workflows/flycast-libretro.yml/badge.svg?branch=main)](https://github.com/lioneil/libretro.cores/releases/download/Linux_aarch64/flycast_libretro.so.zip) |

## Installation and Download

Download the nightly builds from the above table or from the [Releases](https://github.com/lioneil/libretro.cores/releases) section.

Then from your Retro Pie or console or wherever you need the build, simply copy it into the libretro cores folder of your system.

For example, in RetroArch I can go the the RetroArch GUI application Settings > Directory > Cores, and it will provide me the path, something like:

```
/home/[username]/.config/retroarch/cores
```

Simply unzip and copy the file(s) over in the directory and restart retroarch.

## RetroArch Core Settings

While not recommended, you can make this repository your main source of cores.

> ⚠️ Note: The cores in this repository are incomplete and limited to cater to a curated selection of supported systems for a retro handheld device.

In RetroArch, go to Online Updater > Updater Settings and change value for Buildbot Cores URL to:

```
https://github.com/lioneil/libretro.cores/releases/download/Linux_aarch64/
```

Or in `retroarch.cfg`, add/overwrite the key-value pair:

```cfg
core_updater_buildbot_cores_url = "https://github.com/lioneil/libretro.cores/releases/download/Linux_aarch64/"
```

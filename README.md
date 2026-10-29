# libretro.cores/aarch64

A repository for pre-built 64-bit linux (arm64 or aarch64) RetroArch Libretro Cores. These cores are ideal for arm-based linux builds typically for retro handhelds (e.g. Anbernic RG ARC-S or ARC-D).

## Supported Cores

All supported cores can be downloaded from the [Releases](https://github.com/lioneil/libretro.cores/releases) section or directly from the table below.

On the 1st of each month, GitHub Actions builds each core from the latest upstream source ([libretro/FBNeo](https://github.com/libretro/FBNeo), [flyinghead/flycast](https://github.com/flyinghead/flycast)) and replaces the previous build, so the release only has the newest build of each core.

The cores are cross-compiled on Ubuntu 22.04. Your device needs glibc 2.34 or newer and libstdc++ from GCC 12 or newer. Flycast also needs `libgomp`.

| Core | Monthly builds |
| :--- | :------------- |
| FBNeo | [![FBNeo libretro Linux aarch64](https://github.com/lioneil/libretro.cores/actions/workflows/fbneo-libretro.yml/badge.svg?branch=main)](https://github.com/lioneil/libretro.cores/releases/download/Linux_aarch64/fbneo_libretro.so.zip) |
| Flycast | [![Flycast libretro Linux aarch64](https://github.com/lioneil/libretro.cores/actions/workflows/flycast-libretro.yml/badge.svg?branch=main)](https://github.com/lioneil/libretro.cores/releases/download/Linux_aarch64/flycast_libretro.so.zip) |

## Installation and Download

Download the monthly builds from the above table or from the [Releases](https://github.com/lioneil/libretro.cores/releases) section.

Then from your Retro Pie or console or wherever you need the build, simply copy it into the libretro cores folder of your system.

For example, in RetroArch I can go to the RetroArch GUI application Settings > Directory > Cores, and it will provide me the path, something like:

```
/home/[username]/.config/retroarch/cores
```

Simply unzip and copy the file(s) over in the directory and restart retroarch.

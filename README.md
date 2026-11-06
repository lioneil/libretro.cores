# libretro.cores/aarch64

[![Build libretro cores Linux aarch64](https://github.com/lioneil/libretro.cores/actions/workflows/build-cores.yml/badge.svg?branch=main)](https://github.com/lioneil/libretro.cores/actions/workflows/build-cores.yml)

A repository for pre-built 64-bit linux (arm64 or aarch64) RetroArch Libretro Cores. These cores are ideal for arm-based linux builds typically for retro handhelds (e.g. Anbernic RG ARC-S or ARC-D) and single-board computers such as the Raspberry Pi.

## Supported Cores

All supported cores can be downloaded from the [Releases](https://github.com/lioneil/libretro.cores/releases) section or directly from the table below.

On the 1st of each month, GitHub Actions builds each core from the latest upstream source ([libretro/FBNeo](https://github.com/libretro/FBNeo), [flyinghead/flycast](https://github.com/flyinghead/flycast)) and each monthly build publishes a new release containing both cores. The release notes link the exact upstream commit each core was built from. The three most recent releases are kept.

GitHub pauses scheduled workflows in public repositories after 60 days without activity. Each build re-enables its own schedule to prevent this; if a month's release is ever missing, check that the workflow is enabled under the Actions tab.

The cores are cross-compiled on Ubuntu 22.04. Your device needs glibc 2.34 or newer and libstdc++ from GCC 12 or newer. Flycast also needs `libgomp`.

| Core | Latest build |
| :--- | :----------- |
| FBNeo | [Download fbneo_libretro.so.zip](https://github.com/lioneil/libretro.cores/releases/latest/download/fbneo_libretro.so.zip) |
| Flycast | [Download flycast_libretro.so.zip](https://github.com/lioneil/libretro.cores/releases/latest/download/flycast_libretro.so.zip) |

## Installation and Download

Download the monthly builds from the above table or from the [Releases](https://github.com/lioneil/libretro.cores/releases) section.

Each zip holds the core and its upstream licence file. Unzip it and copy the `.so` into the libretro cores folder of your system, and restart RetroArch.

In RetroArch, go to Settings > Directory > Cores to see the path. It is usually:

```
/home/[username]/.config/retroarch/cores
```

On RetroPie, cores are kept per emulator under `/opt/retropie/libretrocores/` (for example `/opt/retropie/libretrocores/lr-fbneo/`).

## License

The workflow and documentation in this repository are released under the [MIT License](LICENSE).

The cores themselves are built from third-party source and keep their upstream licences:

- FBNeo is distributed under the [FBNeo license](https://github.com/libretro/FBNeo/blob/master/src/license.txt), which forbids commercial use.
- Flycast is distributed under the [GNU General Public License v2](https://github.com/flyinghead/flycast/blob/master/LICENSE). The source for each build is the upstream commit linked in its release notes.

# CropsXP

CropsXP assigns experience drops when a survival player breaks supported crops and plants on an Axolotl-PM server.

[![Build](https://github.com/NhanAZ-Plugins/CropsXP/actions/workflows/build.yml/badge.svg)](https://github.com/NhanAZ-Plugins/CropsXP/actions/workflows/build.yml)
[![License](https://img.shields.io/github/license/NhanAZ-Plugins/CropsXP)](LICENSE)

## Behavior

The plugin handles `BlockBreakEvent` for wheat, beetroot, carrot, potato, melon, pumpkin, bamboo, cocoa, sugarcane, sweet berry bush, cactus, sea pickle and nether wart. Its XP range depends on crop maturity, sea pickle count and Silk Touch where relevant. Other blocks and players outside survival mode are left to the server's normal behavior.

The plugin has no commands, permissions or configuration file.

![CropsXP example](https://user-images.githubusercontent.com/60387689/212985194-8f3bfaad-7118-4434-9ee3-55d705ad30c5.jpg)

## Requirements and compatibility

- Axolotl-PM with plugin API `5.0.0`.
- PHP 8.1 or newer in the Axolotl-PM 5 toolchain.

The [Build workflow](.github/workflows/build.yml) pins the Axolotl-PM source revision used for PHPStan level max. The tested runtime is recorded in the release evidence. Compatibility with every Axolotl-PM 5.x release has not been established.

## Installation

Download `CropsXP.phar` from a verified [GitHub release](https://github.com/NhanAZ-Plugins/CropsXP/releases), place it in the server's `plugins/` directory and restart the server.

## Building and testing

The [build workflow](.github/workflows/build.yml) runs PHPStan level max, builds with [DevTools](https://github.com/NhanAZ/DevTools), and verifies the PHAR manifest, source, license and digest. The workflow pins the builder revision. A clean server startup check establishes that the PHAR loads. It does not replace an in-game harvest test with a player.

## License and support

The plugin source is licensed under [GPL-3.0](LICENSE). For help, use [NhanAZ Discord](https://discord.gg/j2X83ujT6c).

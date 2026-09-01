# Changelog

All notable changes to avocado-bsp-raspberrypi4 are documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.1]

### Added
- `kernel-module-cmac`: Bluetooth SMP needs cmac(aes); the board booted with
  `hci0: Unable to create CMAC crypto context`.
- `wireless-regdb-static`, so cfg80211 has a regulatory database (the board
  booted with `regulatory.db` missing and WiFi pinned to country 00).

## [0.1.0]

### Added
- Initial release: Board support for the Raspberry Pi 4.
- CI via the shared `avocado-linux/actions` reusable workflows: PR build check
  (`test.yml`) and tag-driven package + publish to the Avocado feed (`release.yml`).

> ⚠️ **EXPERIMENTAL FORK** — This is an **unofficial, experimental fork** of [flasher.meshcore.io](https://github.com/meshcore-dev/flasher.meshcore.io) maintained by [HermestoAizales](https://github.com/HermestoAizales) for testing purposes only.
> **Not affiliated with or endorsed by the official MeshCore project.**
> For the official web flasher, please visit [flasher.meshcore.io](https://flasher.meshcore.io).
> Use at your own risk.

---

## 🚀 Live Web Flasher

**[https://hermestoaizales.github.io/flasher.meshcore.io/](https://hermestoaizales.github.io/flasher.meshcore.io/)**

Flash experimental MeshCore firmware builds directly from your browser (Chrome/Edge).

## Firmware Variants

Each release provides **two variants** per device:

| Variant | Description | Filename Suffix |
|---------|-------------|-----------------|
| **Standard** | Normal firmware for daily use | *(none)* |
| **Observer** | With `MESH_PACKET_LOGGING=1` — logs all mesh packets (type, route, SNR, RSSI, hash) via Serial for debugging | `-obs` |

Observer builds are ideal for monitoring mesh traffic, debugging packet issues, or running a dedicated observer node.

## Changes vs Upstream

See the [MeshCore fork CHANGES.md](https://github.com/HermestoAizales/MeshCore/blob/main/CHANGES.md) for firmware modifications.

Webflasher-specific changes:
- **GitHub Pages subpath support**: Fixed asset loading (`history.pushState` base URL issue)
- **Observer firmware selection**: Each device role offers standard and observer builds
- **Auto-updated `releases.json`**: Populated automatically from GitHub Release assets via CI
- **Community firmware compatibility**: Devices with upstream `github` config are shown even when no upstream releases match (empty version list)

## Flasher Features

- ESP32 flashing via Web Serial (esptool.js)
- Custom nRF52 serial flashing based on adafruit-nrfutil
- Serial console
- Firmware download (direct from GitHub Release assets)

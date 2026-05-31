> ⚠️ **EXPERIMENTAL FORK** — This is an **unofficial, experimental fork** of [flasher.meshcore.io](https://github.com/meshcore-dev/flasher.meshcore.io) maintained by [HermestoAizales](https://github.com/HermestoAizales) for testing purposes only.
> **Not affiliated with or endorsed by the official MeshCore project.**
> For the official web flasher, please visit [flasher.meshcore.io](https://flasher.meshcore.io).
> Use at your own risk.

---

## 🚀 Live Web Flasher

**[https://hermestoaizales.github.io/flasher.meshcore.io/](https://hermestoaizales.github.io/flasher.meshcore.io/)**

Flash experimental MeshCore firmware builds directly from your browser (Chrome/Edge).

Currently available: **T-Beam SX1262/SX1276** companion BLE firmware (v1.15.0-hermes1)

### About This Fork

This fork hosts experimental firmware builds from the [HermestoAizales/MeshCore](https://github.com/HermestoAizales/MeshCore) fork, which includes:

- **ESP32 Blob Storage Optimization**: Replaces per-key files in `/bl/<hex>` with a single `/adv_blobs` file. Saves ~30 KB Flash on devices with 160 contacts.
- One-time migration of old `/bl/` files on first boot.

### Flasher Features

- ESP32 flashing via Web Serial (esptool.js)
- Custom nRF52 serial flashing based on adafruit-nrfutil
- Serial console

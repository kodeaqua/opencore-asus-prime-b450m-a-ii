# OpenCore Config: ASUS PRIME B450M-A-II, Ryzen 5 4500, RX Vega 56 8GB

Simple OpenCore configuration for AMD Ryzen build.

## Hardware Specs
- **Motherboard**: ASUS PRIME B450M-A-II
- **Processor**: Ryzen 5 4500 (6 Core / 12 Threads)
- **GPU**: Sapphire Pulse RX Vega 56 8GB (HDMI)
- **RAM**: Apacer NOX DDR4 32GB (2x16) @ 3600MHz (XMP) 18-22-22-38
- **NVME**: TeamGroup NVME PCIE 512GB
- **Audio**: Realtek ALC897 (Logitech Z120 via 3.5mm Jack)
- **LAN**: Realtek RTL8111/8168 Gigabit

## What's Working
- Almost everything (Graphics, Audio, LAN, Power Management, etc.)

## Configuration Details
- **SMBIOS**: `iMacPro1,1`
- **Audio Layout ID**: `11`
- **Bootloader**: OpenCore

## Notes
- This config is compatible with most 6-core Ryzen processors.
- Remember to generate your own Serial, Board Serial, and UUID.
- Ensure BIOS settings: Secure Boot (Other OS), Fast Boot (Disabled), CSM (Disabled), Above 4G Decoding (Enabled), Resizeable BAR (Auto).
- **Troubleshooting**: If you experience a bootloop during installation, set `SecureBootModel` to `Disabled` in your config. You can revert it to `j137` or `Default`.

---
*Credits to Acidanthera and AMD OS X team.*

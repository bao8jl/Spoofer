# Spoofer (Modded Version)

Hardware identifier spoofing tool for Windows.

## Features

- **HWID Spoofing** - Modify system UUID, motherboard serial
- **MAC Address Spoofing** - Change network adapter identifiers
- **EDID Spoofing** - Modify monitor serials
- **Trace Removal** - Clean registry, event logs, temp files
- **Backup & Restore** - Save and restore original hardware IDs

## Quick Start

### Installation

**Download Python** from the official website: https://www.python.org/downloads/

**Install dependencies** by running in terminal:
   ```bash
   pip install colorama requests pywin32
```

## Spoofing Modes

| Mode | Use Case | Changes |
|------|----------|---------|
| **Full Spoof** | Hard HWID ban | HWID + MAC + EDID + Traces |
| **Light Spoof** | Soft ban | MAC + EDID + Traces |
| **Recommended** | Continue cheating | Traces + MAC (no HWID) |
| **Reverse** | Undo changes | Restore from backup |

## Safety

The tool includes:
- System restore point creation before changes
- Hardware ID backup to JSON file
- HWID and EDID registry backup for reversal
- Preflight system checks

**Important:**
- HWID/EDID can be restored from backup (not just restore point)
- MAC addresses always reversible
- Create backup before first use

## Known Limitations

- **ASUS motherboards** may block HWID changes
- **WiFi adapters** often don't support MAC spoofing
- **Administrator rights** required for all operations
- **System reboot** needed after EDID changes

## Requirements

- Windows 10/11 (64-bit)
- Python 3.8+
- Administrator privileges

This is a modded version made by me. If you don't trust it, you can find the source here: dsc.gg/samtarbros

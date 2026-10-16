# Scopetta — Releases

Scopetta is a card game you can play on Android, Windows, or in your browser. This repository distributes the Android and Windows builds; it does not contain the application source code.

## Download

**[Get the latest release](https://github.com/diegoami/scopetta-releases/releases/latest)**, or [browse all releases](https://github.com/diegoami/scopetta-releases/releases).

| Platform | Release file | Notes |
| --- | --- | --- |
| Android | `Scopetta-<version>-android.apk` | APK installer |
| Windows (64-bit) | `Scopetta-<version>-windows-x64.exe` | Portable app; no installer required |
| Browser | [Play Scopetta online](https://scopetta.netlify.app/) | No download required |

Check the release notes for details about each version.

## Install

### Android

1. Download the Android APK from the release page and open it on your device.
2. If prompted, allow your browser or file manager to install apps from this source.
3. Follow the on-screen prompts to finish installation.

### Windows

1. Download the Windows x64 executable from the release page.
2. Run the `.exe` file. It is portable, so you can keep it in any folder; there is no installer.
3. Windows may show a **Windows protected your PC** warning because the app is not digitally signed. To continue, select **More info**, then **Run anyway**.

## Verify a download

The latest release includes a `SHA256SUMS.txt` file. Compare the downloaded file's SHA-256 hash with its entry in that file.

On Windows PowerShell:

```powershell
Get-FileHash .\Scopetta-<version>-windows-x64.exe -Algorithm SHA256
```

On Linux:

```sh
sha256sum Scopetta-<version>-android.apk
```

On macOS:

```sh
shasum -a 256 Scopetta-<version>-android.apk
```

Replace the example filename with the file you downloaded. The hash must match the corresponding entry in `SHA256SUMS.txt`.

## Privacy

The release notes state that Scopetta's match history stays on your device and is not sent elsewhere.

## Source

Application source code is maintained in [diegoami/Scopetta](https://github.com/diegoami/Scopetta). Release notes identify the source revision used for a build; this distribution repository contains the downloadable releases.

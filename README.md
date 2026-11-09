# QRMomen releases

QRMomen installers for Android, iOS, macOS, Windows and Linux, built from the QRMomen source repository. Each [release](https://github.com/indramahkota/qrmomen-releases/releases) contains every installer and `SHA256SUMS`.

| Platform | File | Minimum |
| --- | --- | --- |
| Android | [QRMomen-android.apk](https://github.com/indramahkota/qrmomen-releases/releases/latest/download/QRMomen-android.apk) | Android 10 |
| iOS | `QRMomen-ios-unsigned.ipa` in the [latest release](https://github.com/indramahkota/qrmomen-releases/releases/latest) | iOS 18.5 |
| macOS (Apple silicon) | [QRMomen-macos-arm64.dmg](https://github.com/indramahkota/qrmomen-releases/releases/latest/download/QRMomen-macos-arm64.dmg) | |
| macOS (Intel) | [QRMomen-macos-x64.dmg](https://github.com/indramahkota/qrmomen-releases/releases/latest/download/QRMomen-macos-x64.dmg) | |
| Windows | [QRMomen-windows-x64.msi](https://github.com/indramahkota/qrmomen-releases/releases/latest/download/QRMomen-windows-x64.msi), [QRMomen-windows-x64.exe](https://github.com/indramahkota/qrmomen-releases/releases/latest/download/QRMomen-windows-x64.exe) | Windows x64 |
| Debian, Ubuntu | [amd64](https://github.com/indramahkota/qrmomen-releases/releases/latest/download/qrmomen-linux-amd64.deb), [arm64](https://github.com/indramahkota/qrmomen-releases/releases/latest/download/qrmomen-linux-arm64.deb) | |
| Fedora, openSUSE | [x86_64](https://github.com/indramahkota/qrmomen-releases/releases/latest/download/qrmomen-linux-x86_64.rpm), [aarch64](https://github.com/indramahkota/qrmomen-releases/releases/latest/download/qrmomen-linux-aarch64.rpm) | |

`QRMomen-android.aab` is the bundle uploaded to Google Play. The APK in this repository is signed with a different key than the Google Play build, so it cannot update a Google Play installation, and the reverse.

## Notes

- The macOS DMG is not notarized. Open the app the first time with Control-click, Open.
- The IPA is unsigned. Sign it with your own Apple ID (for example with Sideloadly or AltStore) before installing.
- Windows and Linux builds do not sync over Bluetooth.

## Checksums

```bash
shasum -a 256 -c SHA256SUMS --ignore-missing
```

On Windows, compare the output of `Get-FileHash <file> -Algorithm SHA256` with the line for that file in `SHA256SUMS`.

# OpenClaw Codex Releases

This public repository contains **binary release assets only** for OpenClaw Codex clients.
The application source code is maintained in a separate private repository and is not published here.

## Latest stable release: v1.9.34

Download only from the [v1.9.34 Release](https://github.com/lei0620/openclaw-codex-releases/releases/tag/v1.9.34):

- Windows: `OpenClaw-Codex-1.9.34-Setup.exe`
- Android: `OpenClaw-Codex-1.9.34.apk`
- Checksums: `SHA256SUMS.txt`

### Android first production-signed release

Historical Android development builds used a debug certificate and cannot be upgraded in place to v1.9.34. Save the computer address, connection, and pairing information first; then uninstall the old debug app yourself, install the production APK, and pair again. The release process does not uninstall or operate apps on user phones.

### Windows publisher warning

The v1.9.34 Windows installer is **not Authenticode-signed**. Windows may show “Unknown publisher” or a Microsoft Defender SmartScreen warning. Download it only from this repository and verify its SHA-256 before running it.

### Verify SHA-256

Download `SHA256SUMS.txt` from the same Release. In PowerShell, run `Get-FileHash .\OpenClaw-Codex-1.9.34-Setup.exe -Algorithm SHA256` or `Get-FileHash .\OpenClaw-Codex-1.9.34.apk -Algorithm SHA256`, then compare the result with the matching line in the checksum file.
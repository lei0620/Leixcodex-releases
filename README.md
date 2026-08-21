# Leixcodex Releases

This public repository contains the official Android and Windows binary releases for Leixcodex.

## Latest stable release: v1.9.42

Download only from the [v1.9.42 Release](https://github.com/lei0620/Leixcodex-releases/releases/tag/v1.9.42):

- Android: `Leixcodex-v1.9.42-82-android.apk`
- Windows: `Leixcodex-v1.9.42-windows-x64-setup.exe`
- Checksums: `SHA256SUMS.txt`

v1.9.42 fixes public Windows installs that treated folders under `C:\Users\<username>` as projects. It now discovers the real Codex project catalog with no manual configuration, restores the matching desktop conversations, and migrates the affected v1.9.41 configuration during an in-place upgrade.

### Android signing

The Android APK uses the long-term production signing certificate and package name `com.aixm.leixcodex`. Users already running the production-signed app can update in place.

### Windows publisher warning

The Windows installer is signed with the `CtrlGJump Local Code Signing` certificate and a DigiCert timestamp. Because this is not a public commercial CA certificate, computers that do not trust it may still show SmartScreen, Smart App Control, or an unknown-publisher warning.

### Verify SHA-256

Download `SHA256SUMS.txt` from the same Release. In PowerShell, run:

```powershell
Get-FileHash .\Leixcodex-v1.9.42-82-android.apk -Algorithm SHA256
Get-FileHash .\Leixcodex-v1.9.42-windows-x64-setup.exe -Algorithm SHA256
```

Compare the results with the matching entries in `SHA256SUMS.txt` before installation.

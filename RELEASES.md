# Release asset contract

Tags use `vMAJOR.MINOR.PATCH`; prereleases add a SemVer suffix such as `v1.10.0-rc.1`.

Each complete release contains:

- `Leixcodex-vMAJOR.MINOR.PATCH-VERSION_CODE-android.apk`
- `Leixcodex-vMAJOR.MINOR.PATCH-windows-x64-setup.exe`
- `android-update.json`
- `SHA256SUMS.txt`

Stable and prerelease channels use GitHub's release metadata. A release is created as a draft, validated after every asset is uploaded, and only then may it be published.

`android-update.json` contains `versionCode`, `versionName`, `apkUrl`, `sha256`, `notes`, and `publishedAt`. The APK URL must point to the matching asset in the same GitHub Release.

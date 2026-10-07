# 三角洲口风琴 Android

此仓库提供应用的 Android 更新清单与安装包。

- [当前版本清单](android-version.json)
- [v0.7.7 安装包](apk/delta-melodica-android-v0.7.7-calibration.apk)
- [v0.7.7 更新说明](release-notes.md)
- [v0.7.6 安装包](apk/delta-melodica-android-v0.7.6-github-update.apk)

应用“设置 → 检查更新”读取 `main/android-version.json`，根据 `versionCode` 与设备上安装的版本比较。发现新版本时，点击“前往 GitHub 下载”会打开清单中的 `file` 链接。

发布下一版本时，先上传新的 APK，再更新 `android-version.json` 的 `version`、递增的 `versionCode`、`file` 和 `notes`。APK 应使用与当前应用相同的签名证书，才能覆盖安装并保留数据。

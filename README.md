# ScholarFetch

更新发布通道：更新清单 + Windows x64 下载包（ScholarFetch）。

- 当前版本：**1.1.0.2**（build 2）
- 最近更新：修复自动更新:当更新源缓存滞后时,老版本现在直接升级到最新版,不再逐级多次更新。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [ScholarFetch-1.1.0.2-win-x64-Setup.exe](https://github.com/xmuhl-tools/ScholarFetch-updates/releases/download/v1.1.0.2/ScholarFetch-1.1.0.2-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [ScholarFetch-1.1.0.2-win-x64.zip](https://github.com/xmuhl-tools/ScholarFetch-updates/releases/download/v1.1.0.2/ScholarFetch-1.1.0.2-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\ScholarFetch`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
ScholarFetch-1.1.0.2-win-x64.zip
  09bdee8011d5382e217dc914feb48f733833284a1dae37f84821339d5d554dd4
ScholarFetch-1.1.0.2-win-x64-Setup.exe
  330f401c8e7dfcb128a2f47ea1baa92c28f667b8299630bcb8767ff9c6daa13e
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-20），请勿手工改动。

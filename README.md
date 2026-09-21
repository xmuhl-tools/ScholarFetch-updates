# ScholarFetch

更新发布通道：更新清单 + Windows x64 下载包（ScholarFetch）。

- 当前版本：**1.1.0.5**（build 5）
- 最近更新：界面布局优化:「前往」按钮紧贴网址输入框(帮助/检查更新移至右角,不再隔开);五个下载选项勾选框独立成行,与操作按钮/AI设置分区更清晰;按钮与标签全中文化(前往/模型);使用手册勘误(附录工具说明与贴士措辞)随包更新。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [ScholarFetch-1.1.0.5-win-x64-Setup.exe](https://github.com/xmuhl-tools/ScholarFetch-updates/releases/download/v1.1.0.5/ScholarFetch-1.1.0.5-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [ScholarFetch-1.1.0.5-win-x64.zip](https://github.com/xmuhl-tools/ScholarFetch-updates/releases/download/v1.1.0.5/ScholarFetch-1.1.0.5-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\ScholarFetch`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
ScholarFetch-1.1.0.5-win-x64.zip
  a44fcb7fcb56114d50e8627e4d885af56860b4395dd7609f48f66ba0fbe4bffb
ScholarFetch-1.1.0.5-win-x64-Setup.exe
  4dccf754e8c7a9cb5b58a19e16dc1a131ec957acb7a9e38607728a5a3cdcfa6b
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-21），请勿手工改动。

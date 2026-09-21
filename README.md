# ScholarFetch

更新发布通道：更新清单 + Windows x64 下载包（ScholarFetch）。

- 当前版本：**1.1.0.4**（build 4）
- 最近更新：主界面右上角新增「帮助」(打开使用手册)与「检查更新」按钮;使用手册升级V1.3(安装章节改为安装包流程,卸载与常见提示说明);其他功能与1.1.0.3相同。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [ScholarFetch-1.1.0.4-win-x64-Setup.exe](https://github.com/xmuhl-tools/ScholarFetch-updates/releases/download/v1.1.0.4/ScholarFetch-1.1.0.4-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [ScholarFetch-1.1.0.4-win-x64.zip](https://github.com/xmuhl-tools/ScholarFetch-updates/releases/download/v1.1.0.4/ScholarFetch-1.1.0.4-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\ScholarFetch`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
ScholarFetch-1.1.0.4-win-x64.zip
  90041e3015ff3212e268890d51b76e3d78b78c18afefeb736d1cb6682665ac6f
ScholarFetch-1.1.0.4-win-x64-Setup.exe
  82d2ba9cd286bdfe14055ae1935d7620ccddbdc348ec0453c7b2b645c2a622f9
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-21），请勿手工改动。

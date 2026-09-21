# ScholarFetch

更新发布通道：更新清单 + Windows x64 下载包（ScholarFetch）。

- 当前版本：**1.1.0.7**（build 7）
- 最近更新：修复自动更新下载偶发挂死:下载停滞(代理低速拖曳)15秒无进展即自动换下一个下载源;下载过程显示源序号与实时进度,逐源尝试与失败原因写入日志。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [ScholarFetch-1.1.0.7-win-x64-Setup.exe](https://github.com/xmuhl-tools/ScholarFetch-updates/releases/download/v1.1.0.7/ScholarFetch-1.1.0.7-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [ScholarFetch-1.1.0.7-win-x64.zip](https://github.com/xmuhl-tools/ScholarFetch-updates/releases/download/v1.1.0.7/ScholarFetch-1.1.0.7-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\ScholarFetch`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
ScholarFetch-1.1.0.7-win-x64.zip
  c6d903bb1a0beb19981cd952ed3613c399a263860d4775920063294d5f3db59e
ScholarFetch-1.1.0.7-win-x64-Setup.exe
  49dde5b781e4c0e0435e6c24b93f49e25a1ce910d3bedd458b8a2c2f8938fb4c
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-21），请勿手工改动。

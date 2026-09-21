# ScholarFetch

更新发布通道：更新清单 + Windows x64 下载包（ScholarFetch）。

- 当前版本：**1.1.0.6**（build 6）
- 最近更新：窗口标题版本号改为完整四段(如V1.1.0.6),与更新弹窗、文件属性、安装包一致;其他与1.1.0.5相同。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [ScholarFetch-1.1.0.6-win-x64-Setup.exe](https://github.com/xmuhl-tools/ScholarFetch-updates/releases/download/v1.1.0.6/ScholarFetch-1.1.0.6-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [ScholarFetch-1.1.0.6-win-x64.zip](https://github.com/xmuhl-tools/ScholarFetch-updates/releases/download/v1.1.0.6/ScholarFetch-1.1.0.6-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\ScholarFetch`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
ScholarFetch-1.1.0.6-win-x64.zip
  cff9c30cd1ae87d2adbfe6178ae92fcfcaab97b5879d2b88dcd6552f9d4db767
ScholarFetch-1.1.0.6-win-x64-Setup.exe
  9ab62677d938b2bb4395f62c8b0b76a2a1918b59e9403a2f68e977ede86985df
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-21），请勿手工改动。

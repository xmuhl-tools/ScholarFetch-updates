# ScholarFetch

更新发布通道：更新清单 + Windows x64 下载包（ScholarFetch）。

- 当前版本：**1.1.0.1**（build 1）
- 最近更新：V1.1 用户体验升级：界面状态记忆（模式/主题/数量/选项跨启动接续）；任务运行中退出确认；完成弹窗部分成功分级警示与日志直达；核心布局自适应与高分屏机械量测保障；窗口标题与文件属性版本可识别；本版本起支持自动更新与完整性校验。手册 V1.1 增加数据与隐私说明。

## 下载

| 用途 | 文件 |
|---|---|
| 便携版 / 自动更新载荷 | [ScholarFetch-1.1.0.1-win-x64.zip](https://github.com/xmuhl-tools/ScholarFetch-updates/releases/download/v1.1.0.1/ScholarFetch-1.1.0.1-win-x64.zip) |

## 校验（sha256）

```text
ScholarFetch-1.1.0.1-win-x64.zip
  8eed99877043559d589275cfe31531673c9c0e43c68eb9630d8732a99cc0b2a0
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-17），请勿手工改动。

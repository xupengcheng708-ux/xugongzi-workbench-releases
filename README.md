# 许公子剪辑工作台

面向苹果 M 系列 Mac 的口播粗剪工作台，将本机素材整理为可继续编辑的剪映草稿。

当前版本：**0.17.0-preview.2（预览版）**。声音验收尚未完成，生成后请人工核对音频接续、字幕与内容取舍。

## 下载与安装

1. [下载当前安装包](https://github.com/xupengcheng708-ux/xugongzi-workbench-releases/releases/download/v0.17.0-preview.2/workbench-0.17.0-preview.2-macos-arm64.zip)，双击解压。
2. 在 Finder（访达）中进入个人文件夹，将“剪辑工作台.app”放入里面的 `Applications` 文件夹；没有该文件夹可以新建。使用个人应用目录便于后续更新。
3. 双击打开。此版本未使用 Apple 开发者账号，也未做 Apple 公证。如果 macOS 阻止打开，在确认文件来自本仓库后，按系统提示进入“系统设置 → 隐私与安全性 → 仍要打开”。不需要关闭系统安全保护。
4. 首次启动自动下载三个离线组件，总计约 3 GB。程序会检查下载摘要并保留组件；网络中断后重新打开可重试。建议首次准备前至少空出 10 GB 磁盘空间。
5. 使用自己的 Moonshot API Key（模型服务密钥）和余额；密钥保存在本机钥匙串。视频与音频留在本机，转写文字会发送到 Kimi 进行内容判断。生成前按应用提示核对费用。

## 系统要求与验证范围

- 苹果 M 系列芯片；macOS 15 或更高；已安装剪映。
- 当前在作者的 macOS 26 电脑完成运行和更新验证；macOS 15 的独立实机验收尚未完成。
- 原生外壳、转写/对齐运行环境随包或首次组件一起提供，不要求安装 Python 或 Homebrew。
- 当前仍为预览版，不将安装成功等同于陌生素材的剪辑质量验收。

## 后续更新

打开工作台，在左上角应用菜单选择“检查更新…”。有新版时，确认后下载、验证签名并安装重启；工作台正在处理任务时会暂缓更新。

程序、离线组件与任务数据分开存放。日常更新通常只下载约 194 MB 的程序包；离线组件版本未变化时继续复用。任务与设置保存在本机 Application Support 目录，更新不清空任务。

本仓库的 [预览更新通道](https://github.com/xupengcheng708-ux/xugongzi-workbench-releases/releases/tag/preview-channel) 提供固定版本列表；[离线组件](https://github.com/xupengcheng708-ux/xugongzi-workbench-releases/releases/tag/components-20261031) 使用固定版本地址。普通使用者只需下载安装包，无需手工处理这些文件。

## 发布文件

- [版本记录与安装包](https://github.com/xupengcheng708-ux/xugongzi-workbench-releases/releases/tag/v0.17.0-preview.2)
- [校验值](https://github.com/xupengcheng708-ux/xugongzi-workbench-releases/releases/download/v0.17.0-preview.2/SHA256SUMS.md)
- [第三方组件说明](https://github.com/xupengcheng708-ux/xugongzi-workbench-releases/releases/download/v0.17.0-preview.2/THIRD_PARTY_NOTICES.md)

安装包及更新列表由同一发布密钥签名；离线组件另有应用内固定的 SHA-256 校验。该机制用于验证发布来源和文件完整性，不代表 Apple 公证。

仓库公开，任何人均可下载；包内程序和剪辑规则也可查看。发行文件不含作者的任务素材、任务专属修复证据、API 密钥或更新私钥。

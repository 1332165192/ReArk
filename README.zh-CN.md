# ReArk

[English](README.md) | 简体中文

ReArk 是一款面向 HarmonyOS 和 Android 应用的桌面逆向与 AI 辅助分析工具。支持打开鸿蒙 `.hap`、`.app`、`.abc` 文件和 Android `.apk`、`.aab` 包，在同一个工作区中查看代码、资源、元数据及应用运行行为。

结合静态分析、真机交互和 ReArk Agent，可用于研究应用逻辑、安全分析和 CTF 解题。

## 安装与运行平台

请前往[最新发布页](https://github.com/lkimuk/ReArk/releases/latest)，下载适合电脑系统的安装包。历史版本和更新说明见[全部发布版本](https://github.com/lkimuk/ReArk/releases)。

| 系统 | 版本要求 | 点击直接下载 |
| :---: | --- | --- |
| <img src="https://raw.githubusercontent.com/devicons/devicon/v2.17.0/icons/windows8/windows8-original.svg" width="44" height="44" alt="Windows"><br>Windows | Windows 10+<br>x64 | [![Setup x64](https://img.shields.io/badge/Setup-x64-0078D4?style=flat-square)](https://github.com/lkimuk/ReArk/releases/download/v1.0.0/ReArk-1.0.0-windows-x64-setup.exe) |
| <img src="https://raw.githubusercontent.com/devicons/devicon/v2.17.0/icons/apple/apple-original.svg" width="44" height="44" alt="macOS"><br>macOS | macOS 14.0+<br>Apple Silicon | [![DMG Apple Silicon](https://img.shields.io/badge/DMG-Apple_Silicon-000000?style=flat-square&logo=apple&logoColor=white)](https://github.com/lkimuk/ReArk/releases/download/v1.0.0/ReArk-1.0.0-macos-arm64.dmg) |
| <img src="https://raw.githubusercontent.com/devicons/devicon/v2.17.0/icons/linux/linux-original.svg" width="44" height="44" alt="Linux"><br>Linux | x64<br>系统要求待公布 | 下个版本提供 |

## 功能亮点

**包体与静态分析**

- 支持 HarmonyOS HAP/APP/ABC 和 Android APK/AAB 文件
- 浏览包结构、模块、源码输出、资源和应用元数据
- 支持 ABC 反汇编、反编译，以及字符串、字面量、交叉引用和调用参数流分析
- 查看 Android Manifest、权限、组件、入口点、资源和应用图标
- 查看 Android 反汇编和类 Java 反编译结果
- 支持十六进制、格式化 JSON、XML、文本、图片和媒体资源预览，以及文件搜索和源码导航

**鸿蒙签名与打包**

- 检查签名、证书和签名有效期
- 配置签名材料，对鸿蒙应用进行重签名和重打包
- 将支持的应用包安装到连接的设备；Android 设备安装使用 APK 文件

**ReArk Agent**

- 围绕当前鸿蒙或 Android 包进行上下文问答
- 按需发现分析能力，读取包体文件、元数据、字符串、反汇编和反编译结果
- 附加参考文档，结合自己的资料补充包体分析证据
- 支持多种模型服务，包括 OpenAI 兼容接口和本地 Ollama 模型
- 串联静态分析与真机工作流；宿主命令、Python 执行和设备操作遵循相应的授权流程

**真机连接与操纵**

- 通过 HDC 发现鸿蒙设备，通过 ADB 发现 Android 设备
- 安装和启动应用、截屏、检查 UI 节点、读取设备日志
- 实时投屏，通过鼠标和键盘操纵设备
- 根据设备和运行时支持情况，使用录屏、音频、剪贴板和设备控制功能
- 支持全屏投屏和独立投屏窗口

具体分析视图和设备操作取决于包格式、系统版本及设备能力。ABC 迹索工具和鸿蒙重签名功能适用于鸿蒙包。

## 截图

| 工作区概览 | Ark 反汇编 |
| --- | --- |
| <img src="assets/screenshots/01-overview.png" alt="ReArk 工作区概览" width="420"> | <img src="assets/screenshots/02-disassembly.png" alt="Ark 字节码反汇编" width="420"> |

| ABC / Hex 检查 | 字符串 |
| --- | --- |
| <img src="assets/screenshots/03-abc-hex-view.png" alt="ABC 和 Hex 检查" width="420"> | <img src="assets/screenshots/04-strings.png" alt="ABC 字符串视图" width="420"> |

| ReArk Agent | Agent 分析 |
| --- | --- |
| <img src="assets/screenshots/05-ReArk-agent.png" alt="ReArk Agent 工作区" width="420"> | <img src="assets/screenshots/06-ReArk-agent-analysis.png" alt="ReArk Agent 分析结果" width="420"> |

| 设备运行态 | ABC 迹索视图 |
| --- | --- |
| <img src="assets/screenshots/07-device-runtime.png" alt="HarmonyOS 设备运行态工作区" width="420"> | <img src="assets/screenshots/08-abc-evidance.png" alt="ABC 迹索视图" width="420"> |


## 安全与隐私

ReArk 仅应用于合法授权的逆向工程、互操作研究、恶意样本分析和安全研究。

使用 ReArk Agent 连接远程模型服务时，请避免提交密钥、证书、用户数据、商业秘密或其他敏感内容。

## 许可

ReArk 使用 Apache License 2.0 许可。详情见 [LICENSE](LICENSE)。

第三方声明见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。

## 支持

- 问题反馈：[GitHub Issues](https://github.com/lkimuk/ReArk/issues)
- 使用指南：[cppmore.com/ReArk](https://www.cppmore.com/category/ReArk/)

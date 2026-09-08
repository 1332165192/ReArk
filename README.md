# ReArk

English | [简体中文](README.zh-CN.md)

ReArk is a desktop reverse engineering and AI-assisted analysis tool for HarmonyOS and Android applications. Open HarmonyOS `.hap`, `.app`, and `.abc` files or Android `.apk` and `.aab` packages to inspect code, resources, metadata, and application behavior in one workspace.

Combine static analysis with connected-device inspection and ReArk Agent to investigate application logic, review security, and work through CTF challenges.

## Installation and platforms

Download the installer for your computer from [Latest release](https://github.com/lkimuk/ReArk/releases/latest). See [All releases](https://github.com/lkimuk/ReArk/releases) for version history and release notes.

| Desktop platform | Availability |
| --- | --- |
| Windows x64 | Setup installer available in v1.0.0 |
| macOS Apple Silicon | DMG available in v1.0.0 |
| Linux | Source build and packaging configuration; no installer in v1.0.0 |

## Feature Highlights

**Package and static analysis**

- Analyze HarmonyOS HAP/APP/ABC and Android APK/AAB files
- Browse package structure, modules, source output, resources, and application metadata
- Disassemble and decompile ABC bytecode; explore strings, literals, cross-references, and call argument flows
- Inspect Android manifests, permissions, components, entry points, resources, and application icons
- Read Android disassembly and Java-like decompiled output
- View hex data, formatted JSON, XML, text, images, and media resources; search files and navigate source output

**HarmonyOS signing and packaging**

- Inspect signatures, certificates, and signing validity
- Configure signing materials, re-sign, and repackage HarmonyOS applications
- Install supported application packages on connected devices; Android device installation uses APK files

**ReArk Agent**

- Ask contextual questions about the current HarmonyOS or Android package
- Discover analysis capabilities and retrieve package files, metadata, strings, disassembly, and decompiled output as needed
- Attach reference documents to supplement package evidence with your own materials
- Use supported model providers, including OpenAI-compatible endpoints and local Ollama models
- Combine static analysis with device workflows; host commands, Python execution, and device operations use the applicable approval flows

**Connected devices**

- Discover HarmonyOS devices through HDC and Android devices through ADB
- Install and launch applications, capture screenshots, inspect UI nodes, and read device logs
- Mirror device screens in real time and control devices using mouse and keyboard
- Use screen recording, audio, clipboard, and device controls where supported by the device and runtime
- Work with fullscreen or detached mirroring windows

Available analysis views and device actions depend on the package format, operating system version, and device capabilities. ABC evidence tools and HarmonyOS re-signing are specific to HarmonyOS packages.

## Screenshots

| Workspace overview | Ark disassembly |
| --- | --- |
| <img src="assets/screenshots/01-overview.png" alt="ReArk workspace overview" width="420"> | <img src="assets/screenshots/02-disassembly.png" alt="Ark bytecode disassembly" width="420"> |

| ABC / Hex inspection | Strings |
| --- | --- |
| <img src="assets/screenshots/03-abc-hex-view.png" alt="ABC and Hex inspection" width="420"> | <img src="assets/screenshots/04-strings.png" alt="ABC strings view" width="420"> |

| ReArk Agent | Agent analysis |
| --- | --- |
| <img src="assets/screenshots/05-ReArk-agent.png" alt="ReArk Agent workspace" width="420"> | <img src="assets/screenshots/06-ReArk-agent-analysis.png" alt="ReArk Agent analysis result" width="420"> |

| Device runtime | ABC trace view |
| --- | --- |
| <img src="assets/screenshots/07-device-runtime.png" alt="HarmonyOS device runtime workspace" width="420"> | <img src="assets/screenshots/08-abc-evidance.png" alt="ABC trace view" width="420"> |

## Safety and Privacy

Use ReArk only for legally authorized reverse engineering, interoperability research, malware analysis, and security research.

When using ReArk Agent with remote model providers, avoid submitting secrets, certificates, user data, trade secrets, or other sensitive content.

## License

ReArk is licensed under the Apache License 2.0. See [LICENSE](LICENSE) for details.

Third-party notices are listed in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

## Support

- Issues: [GitHub Issues](https://github.com/lkimuk/ReArk/issues)
- User guide: [cppmore.com/ReArk](https://www.cppmore.com/category/ReArk/)

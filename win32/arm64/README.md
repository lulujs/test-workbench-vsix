# VSIX 插件仓库

本仓库用于存放 TSCode 离线插件包 (`.vsix`)，按照平台相关性进行目录组织。

## 目录结构

```
├── *.vsix                  # 平台无关的插件（不区分操作系统）
├── darwin/
│   ├── arm64/              # macOS ARM64 (Apple Silicon) 插件
│   └── x64/                # macOS x64 (Intel) 插件
├── linux/                  # Linux 插件
└── win32/
    ├── arm64/              # Windows ARM64 插件
    └── x64/                # Windows x64 插件
```

## 说明

- **根目录**: 存放平台无关的插件（不区分操作系统），例如语言包、主题等通用插件。
- **平台目录**: `darwin/`、`linux/`、`win32/` 分别对应 macOS、Linux、Windows 三个平台。各平台目录下可按 CPU 架构进一步细分（如 `arm64/`、`x64/`），放置仅在该平台/架构下运行的插件。

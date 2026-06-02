# Anything Analyzer v3.6.27

## 修复

- **发布工作流 Actions 运行时兼容性** — 升级 Build & Release 中的核心 Actions 主版本，避免继续触发 Node 20 运行时迁移注解
  - Checkout、pnpm、Node.js、artifact 上传/下载和 Release 创建步骤均使用 Node 24 运行时兼容的 Actions 主版本
  - 新增发布工作流回归测试，防止核心 Actions 配置回退到旧主版本

## 下载

| 平台 | 文件 |
|------|------|
| Windows | Anything-Analyzer-Setup-3.6.27.exe |
| macOS (Apple Silicon) | Anything-Analyzer-3.6.27-arm64.dmg |
| macOS (Intel) | Anything-Analyzer-3.6.27-x64.dmg |
| Linux | Anything-Analyzer-3.6.27.AppImage |

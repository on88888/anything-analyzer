# Anything Analyzer v3.6.32

## 修复

- **Anthropic 工具调用空文本诊断** — 避免工具调用最终轮次缺少 `text` 内容时被误判为空成功结果
  - Anthropic/MiniMax 工具调用循环现在要求最终响应至少包含一个 `text` content block
  - 新增回归测试覆盖工具调用后返回非文本内容块的异常路径

## 下载

| 平台 | 文件 |
|------|------|
| Windows | Anything-Analyzer-Setup-3.6.32.exe |
| macOS (Apple Silicon) | Anything-Analyzer-3.6.32-arm64.dmg |
| macOS (Intel) | Anything-Analyzer-3.6.32-x64.dmg |
| Linux | Anything-Analyzer-3.6.32.AppImage |

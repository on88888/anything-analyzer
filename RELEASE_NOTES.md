# Anything Analyzer v3.6.48

## 修复

- **OpenAI 工具轮次响应校验** — 拒绝缺少 assistant message 的 OpenAI Chat Completions 工具调用响应
  - 工具调用轮次缺少 message 字段时不再退化为原生运行时异常
  - 现在会在入站协议边界返回明确的 LLM 响应格式异常

## 下载

| 平台 | 文件 |
|------|------|
| Windows | Anything-Analyzer-Setup-3.6.48.exe |
| macOS (Apple Silicon) | Anything-Analyzer-3.6.48-arm64.dmg |
| macOS (Intel) | Anything-Analyzer-3.6.48-x64.dmg |
| Linux | Anything-Analyzer-3.6.48.AppImage |

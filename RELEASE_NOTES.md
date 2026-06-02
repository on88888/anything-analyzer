# Anything Analyzer v3.6.36

## 修复

- **Anthropic/MiniMax 非流式文本格式校验** — 避免 text content 不是字符串时被拼成 `[object Object]`
  - 普通请求和工具调用最终轮次复用同一段 Anthropic 文本块校验逻辑
  - 新增回归测试覆盖非字符串 text content 的异常路径

## 下载

| 平台 | 文件 |
|------|------|
| Windows | Anything-Analyzer-Setup-3.6.36.exe |
| macOS (Apple Silicon) | Anything-Analyzer-3.6.36-arm64.dmg |
| macOS (Intel) | Anything-Analyzer-3.6.36-x64.dmg |
| Linux | Anything-Analyzer-3.6.36.AppImage |

# Anything Analyzer v3.6.21

## 修复

- **LLM 分析取消立即生效** — 修复分析任务取消后底层 LLM 请求仍继续执行的问题
  - 普通补全和工具调用补全现在都会把 `AbortSignal` 传递到底层 `fetch`
  - 取消请求时统一返回 `LLM 请求已取消`，避免被误判为网络故障

## 下载

| 平台 | 文件 |
|------|------|
| Windows | Anything-Analyzer-Setup-3.6.21.exe |
| macOS (Apple Silicon) | Anything-Analyzer-3.6.21-arm64.dmg |
| macOS (Intel) | Anything-Analyzer-3.6.21-x64.dmg |
| Linux | Anything-Analyzer-3.6.21.AppImage |

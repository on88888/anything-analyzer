# Anything Analyzer v3.6.40

## 修复

- **OpenAI 工具调用字段校验** — 避免缺失 id/name 的畸形 tool_call 进入工具执行轮次
  - 工具调用入站阶段直接拒绝缺少 id 或 function.name 的响应
  - 新增回归测试覆盖 OpenAI tool_call 必要字段缺失路径

## 下载

| 平台 | 文件 |
|------|------|
| Windows | Anything-Analyzer-Setup-3.6.40.exe |
| macOS (Apple Silicon) | Anything-Analyzer-3.6.40-arm64.dmg |
| macOS (Intel) | Anything-Analyzer-3.6.40-x64.dmg |
| Linux | Anything-Analyzer-3.6.40.AppImage |

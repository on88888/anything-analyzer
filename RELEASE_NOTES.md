# Anything Analyzer v3.6.14

## 修复

- **Responses API 流式末尾事件不再丢失** — 修复 SSE 响应没有尾随换行时最后一行 `data:` 未被解析，导致末尾文本块、usage 或错误事件被忽略的问题
  - 在流结束后补处理剩余 buffer，保留原有逐行解析行为
  - 增加无尾随换行 SSE 回归测试，确保最后文本块会进入增量回调和最终内容
- **macOS 发布工作流支持无签名 secrets 打包** — 修复 GitHub Actions 中空 `CSC_LINK` 被 electron-builder 当成签名文件路径，导致 macOS 打包失败的问题
  - 仅在 `CSC_LINK` 存在时向构建环境注入签名变量
  - 缺失签名配置时跳过 codesign 校验，保留未签名 macOS 产物构建
- **Responses API 流式失败事件不再被吞掉** — 修复 `response.failed` / `error` SSE 事件被 JSON 容错逻辑吞掉，导致上层误判为空成功响应的问题
  - 将 SSE JSON 解析容错和 API 失败事件处理分离
  - 增加流式失败事件回归测试，确保失败信息会向调用方抛出

## 下载

| 平台 | 文件 |
|------|------|
| Windows | Anything-Analyzer-Setup-3.6.14.exe |
| macOS (Apple Silicon) | Anything-Analyzer-3.6.14-arm64.dmg |
| macOS (Intel) | Anything-Analyzer-3.6.14-x64.dmg |
| Linux | Anything-Analyzer-3.6.14.AppImage |

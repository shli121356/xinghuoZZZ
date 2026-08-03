# 星火 API 中转站使用文档

## 1. 获取 API Key

打开 [控制台](https://zz.ncriscs.com/dashboard)，登录后创建 API Key。建议按项目或环境区分生产、测试密钥，并定期轮换。

## 2. 配置 Base URL

将客户端的 Base URL 设置为：

```text
https://zz.ncriscs.com
```

保留原有模型名称和请求参数。兼容 OpenAI 风格接口的客户端通常只需要替换 Base URL 和 Authorization。

## 3. 发起请求

在请求头中携带 Bearer Token：

```bash
curl https://zz.ncriscs.com/v1/chat/completions \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "gpt-4o-mini",
    "messages": [
      { "role": "user", "content": "点燃一个稳定的 AI 请求" }
    ]
  }'
```

## 4. 常用入口

- [控制台](https://zz.ncriscs.com/dashboard)：创建密钥和管理调用配置。
- [模型列表](https://zz.ncriscs.com/available-channels)：查看当前可用模型和渠道。
- [节点状态](https://zz.ncriscs.com/monitor)：查看模型节点可用性、延迟和历史状态。
- [飞书使用文档](https://fcn7al09nyc3.feishu.cn/wiki/D358wpMNyiHnflkvtTjcD9VGnJg)：查看完整平台说明。

## 安全注意事项

- 只在服务端保存 API Key，不要暴露给浏览器、移动端或公开仓库。
- 发现密钥泄露后，立即在控制台禁用并重新创建。
- 上线前通过节点状态页确认可用区和延迟。
- 生产环境建议配置超时、重试和日志脱敏。

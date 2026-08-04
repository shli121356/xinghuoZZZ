# 星火中转站

**Spark Relay**  
节点已点燃 · Ready

![星火中转站首页预览](http://localhost:8000/spark-relay-home-preview.png)

## 把星火稳稳接住，让火种燃通 AI 长路

星火 API 中转站：**多集群**保障链路稳定，**全链路加密**保护数据，**阶梯平价计费**，**极速转发**各类大模型请求。

## 快捷入口

- <a href="https://zz.ncriscs.com/dashboard" target="_blank" rel="noopener noreferrer">进入控制台</a>
- <a href="https://zz.ncriscs.com/available-channels" target="_blank" rel="noopener noreferrer">模型列表</a>
- <a href="https://fcn7al09nyc3.feishu.cn/wiki/D358wpMNyiHnflkvtTjcD9VGnJg" target="_blank" rel="noopener noreferrer">使用文档</a>
- <a href="https://zz.ncriscs.com/monitor" target="_blank" rel="noopener noreferrer">节点状态</a>

## 稳定接力

服务地址：`https://zz.ncriscs.com`

智能分配火种节点，让每次请求都稳稳抵达。

### 核心能力

- 透明计费
- 高并发
- 高稳定性
- 广泛支持
- 极速转发

## 服务特性

### 星火长燃

多节点冗余负载均衡，星火链路持续在线，高并发场景调用稳定不掉线。

### 星火安燃

数据全程加密隔离，精细化权限管控，每一次火种调用隐私不泄露。

### 星火优燃

透明阶梯低价计费，无隐形扣费，用更低成本点燃你的 AI 业务。

## 使用说明

星火中转站用于把业务侧请求稳定转发到大模型服务。准备好密钥后，将 Base URL 设置为 `https://zz.ncriscs.com`，即可接入统一鉴权、计费和节点状态能力。

### 1. 获取 API Key

进入控制台创建访问密钥，并按项目或环境区分生产、测试调用。

### 2. 配置转发地址

将客户端 Base URL 设置为 `https://zz.ncriscs.com`，保留兼容的模型名称与请求参数。

### 3. 发起模型请求

在请求头携带 Bearer Token，即可通过稳定节点转发对话、补全或多模态请求。

## 接口调用示例

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

建议在服务端保存密钥，不要把 API Key 暴露到浏览器前端；上线前可先打开<a href="https://zz.ncriscs.com/monitor" target="_blank" rel="noopener noreferrer">节点状态页</a>确认可用区与延迟。

## 首页预览

[打开完整首页](http://localhost:8000/spark-relay-home.html?logo=56)

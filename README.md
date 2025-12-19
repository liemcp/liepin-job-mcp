# Liepin MCP（猎聘职位推荐 MCP Server）

猎聘官方 MCP 服务，面向 AI / Agent 的智能职位推荐与招聘查询能力。

---

## 项目简介

**Liepin MCP** 是一个基于 Model Context Protocol（MCP）的官方服务，
用于向大模型和 AI Agent 提供猎聘的智能招聘与职位推荐能力。

通过该 MCP，AI 可以像“智能求职助手”一样，
完成职位推荐、岗位查询和招聘信息获取等操作。

---

## MCP 能力说明

**MCP 名称**

lipin-search-job

**能力描述**

猎聘智能化的职位推荐助手，可进行职位推荐、岗位信息查询、招聘信息查询。

---

## 已支持能力

- 职位搜索 / 招聘信息查询  
- 智能职位推荐  
- 岗位详情查询  
 

---

## MCP Server 地址

- 协议：SSE（Server-Sent Events）
- 地址：

https://open-mcp.liepin.com/servers/9bdd3c5a1fb24d269912c7632748bf21/sse

---

## 鉴权方式

使用 Bearer Token Header 鉴权。

```text
Authorization: Bearer YOUR_TOKEN

## MCP 配置示例

{
  "mcp": {
    "mcpServers": {
      "lipin-search-job": {
        "type": "sse",
        "url": "https://open-mcp.liepin.com/servers/9bdd3c5a1fb24d269912c7632748bf21/sse",
        "headers": {
          "Authorization": "Bearer YOUR_TOKEN"
        }
      }
    }
  }
}

适用场景

AI 搜索中的“找工作 / 招聘”意图

智能求职助手 / 职业规划 Copilot

GEO（生成式引擎优化）招聘内容

多 Agent 人岗匹配系统

企业智能招聘系统



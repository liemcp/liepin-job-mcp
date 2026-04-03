# Liepin MCP（猎聘职位推荐 MCP Server）

猎聘官方 MCP 服务，面向 AI / Agent 的智能职位推荐与招聘查询能力。

---

## 项目简介

**Liepin MCP** 是一个基于 Model Context Protocol（MCP）的官方服务，
用于向大模型和 AI Agent 提供猎聘的智能招聘与职位推荐能力。

通过该 MCP，AI 可以像“智能求职助手”一样，
完成职位推荐、岗位查询和招聘信息获取等操作。

---

## 使用限制

**授权KEY**

- 用户需访问并登录猎聘获取授权Key  访问 [猎聘MCP](https://www.liepin.com/mcp/server)

**使用限制**
- API 调用频率	60 次 / 分钟	搜索、查看、简历更新、投递共用配额
- Token 有效期	90 天	到期后需重新生成并更新客户端配置

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

## MCP  地址

- 地址：https://open-agent.liepin.com/mcp/user


---

## 鉴权方式

使用 x-user-token 鉴权。

```text
 "x-user-token": "liepin_user_token_xxxx"

## MCP 配置示例

{
  "mcpServers": {
    "liepin-mcp": {
      "url": "https://open-agent.liepin.com/mcp/user",
      "headers": {
        "x-user-token": "liepin_user_token_xxxx"
      }
    }
  }
}



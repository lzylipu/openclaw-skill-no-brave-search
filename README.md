# 🔍 No Brave Search Skill / 强制禁用 Brave 搜索中转器

> 🌐 English | [简体中文](./README.md)
> Restrict web searches to Google/Bing, preventing fallback requests to Brave Search API.
> 强制截获并封禁 Brave Search API 触发，只允许调用谷歌和必应进行免 API 网络检索。

## ❓ 为什么需要？ / Why?

- 没有 Brave Search API 密钥 / No Brave API key
- 每次搜索都触发 Brave 错误 / Every search triggers Brave errors
- 想要完全控制搜索引擎 / Full search engine control

## ✨ 功能特性 / Features

- 🚫 **Brave Block / 彻底拦截**: zero Brave Search API calls
- 🌐 **Multi-engine / 多引擎**: Bing, Google, DuckDuckGo
- 💸 **No API Key / 免 API**: all engines work without keys
- 📅 **Time filter / 时间筛选**: past 24h/week/month support

## 🚀 安装 / Installation

```bash
cp -r no-brave-search /path/to/openclaw/skills/
```

```json
{ "defaultEngine": "bing" }
```

## 🔧 支持的搜索引擎 / Supported Engines

| 引擎 / Engine | 优点 / Pros | 场景 / Use Case |
|------|------|------|
| **必应 / Bing** | 稳定、中文好 / stable, good Chinese | 日常搜索 / daily |
| **谷歌 / Google** | 质量高 / high quality | 专业搜索 / professional |
| **DuckDuckGo** | 隐私友好 / privacy-friendly | 备用 / fallback |

## 📁 目录结构 / Structure

```
no-brave-search/
├── SKILL.md      # 技能定义
├── README.md     # 本文件
└── search.js     # 重定向拦截逻辑
```

## ⚠️ 注意事项 / Notes

- 优先级最高 / highest priority in search chain
- 确保系统永不回退到 Brave Search

## 📄 许可证 / License

MIT

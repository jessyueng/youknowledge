# Competitive Landscape

**Last Updated:** 2026-02-03

## Overview

| 竞品 | 定位 | Changelog URL |
|------|------|---------------|
| **YouWare** | AI Vibe Coding + YouBase 后端 | [youware.app](https://youware.app) |
| **Lovable** | AI web app builder | [changelog](https://docs.lovable.dev/changelog) |
| **Bolt** | AI full-stack builder | [release notes](https://support.bolt.new/release-notes) |
| **v0** | Vercel's AI UI generator | [changelog](https://v0.app/changelog) |
| **Replit** | AI coding + cloud IDE | [updates](https://docs.replit.com/updates/) |
| **Trickle** | AI no-code builder | [changelog](https://feedback.trickle.so/changelog) |
| **Base44** | AI app builder | [changelog](https://base44.com/changelog) |
| **Rocket** | AI web builder | [changelog](https://docs.rocket.new/inspiration-and-help/changelog) |

> 💡 使用 **"sync competitive"** 指令可自动爬取上述 changelog 页面更新竞品数据

## Quick Comparison

| 维度 | YouWare | Lovable | Bolt | v0 | Replit |
|------|---------|---------|------|-----|--------|
| **内置后端** | YouBase | Lovable Cloud | Bolt Database | ❌ (需 Supabase) | Replit DB |
| **Coview 录屏** | ✅ | ❌ | ❌ | ❌ | ❌ |
| **积分退款** | ✅ Credit Care | ❌ | ❌ | ❌ | ❌ |
| **可视化编辑** | ✅ | ✅ | ✅ | ❌ | ❌ |
| **MCP 集成** | ✅ | ❌ | ❌ | ❌ | ❌ |
| **移动端 App** | ✅ iOS/Android | ❌ | ❌ | ❌ | ✅ |
| **定价模式** | 积分制 | 订阅+积分 | 订阅 | 订阅 | 订阅 |

## Differentiation

### YouWare 独有优势

1. **Coview** - 录屏+语音描述需求，解决"AI 是瞎子"问题
2. **Credit Care** - 不满意自动退款，降低用户心理门槛
3. **YouBase** - 真正零配置的内置后端
4. **Tab Tab 补全** - 智能 prompt 建议

### 各竞品特点

| 竞品 | 核心卖点 | 短板 |
|------|----------|------|
| **Lovable** | Design-first，UI 美观 | 后端依赖 Supabase |
| **Bolt** | 速度快，功能全 | 无积分退款机制 |
| **v0** | Vercel 生态，部署方便 | 只做前端，无后端 |
| **Replit** | 完整 IDE，多语言 | 学习曲线陡峭 |
| **Trickle** | 中文友好 | 功能相对简单 |

---

## Data Source

竞品 changelog 数据存储在 `_data/storage/*.json`，包含：
- 功能更新记录
- 发布时间
- 功能标签分类

使用 `sync competitive` 指令更新数据。

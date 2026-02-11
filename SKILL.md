---
name: youknowledge
description: "YouWare official documentation and community tutorials. Use when explaining YouWare features, pricing, capabilities, YouBase backend, Coview screen recording, or integrations. Triggers on: what is YouWare, YouWare docs, YouWare features, YouWare pricing, YouWare plans, Pro plan, Ultra plan, credits system, YouBase database, YouBase backend, Coview, screen recording, visual editing tool, publish app, deploy app, custom domain, Figma to code, GitHub integration, Notion integration, remix app, AI code generation, no-code platform, low-code builder, Tab Tab completion, boost feature, how to use YouWare, Vibe Coding tutorials, YouWare use cases."
---

# YouWare Knowledge Base

**Last Synced:** 2026-02-03

## Auto-Sync Reminder

When this skill is loaded, check if `Last Synced` date is older than 14 days from today.

If outdated, **before answering the user's question**, say:

> 📢 YouWare 文档已超过 14 天未更新。要先同步最新文档吗？（输入 "sync" 更新，或继续当前问题）

If user says "sync" / "更新" / "yes", run the sync workflow below. Otherwise proceed with their question.

---

## Product Overview

### 核心定位（一句话精髓）

**YouWare = AI Vibe Coding + Production-Ready Backend**

用自然语言描述想法，30 秒生成完整应用，内置后端（YouBase）和独特的录屏交互（Coview）让非技术用户也能构建生产级应用。

---

### 与竞品的核心差异化

| 能力 | YouWare | Lovable/Bolt/v0 |
|------|---------|-----------------|
| **后端集成** | YouBase 零配置内置 | 需要 Supabase/额外付费 |
| **交互方式** | Coview 录屏+语音 | 纯文字描述 |
| **风险控制** | Credit Care 不满意退款 | 无退款机制 |
| **移动端** | iOS/Android 原生 App | 仅 Web |
| **MCP 生态** | 7+ 官方集成（Figma/Notion/GitHub） | 有限或无 |

**独特卖点速记：**
1. **Coview** - 解决"AI 是瞎子"问题，指着屏幕说需求
2. **Credit Care** - 只为满意结果付费，降低心理门槛
3. **YouBase** - $20 搞定后端，vs $5000 雇人成本

---

### 目标用户 & 痛点映射

| 用户类型 | 核心痛点 | YouWare 解决方案 | 典型场景 |
|----------|----------|------------------|----------|
| **SMB 创始人** | 没钱雇人，不懂技术 | $20/月 Pro 计划，内置后端 | MVP 验证、内部工具 |
| **设计师** | 不会写代码，依赖开发 | Figma to Code + Visual Editing | 作品集、客户 Demo |
| **开发者** | 重复性工作浪费时间 | AI 快速原型 + Code Editor | 快速验证、Side Project |
| **内容创作者** | 不懂技术，想要变现 | Remix 社区项目 + 自定义 | 会员站、课程平台 |
| **竞品用户** | Lovable Cloud 额外收费 | 后端包含在订阅内，不收"云税" | 迁移成本低 |

---

### 使用场景决策树

#### 场景 1：从零开始新项目
```
描述需求 → 选择 AI 模型（快速原型用 Gemini，复杂逻辑用 Sonnet）
         → 生成后先用 Visual Editing 微调样式（省 Credits）
         → 需要后端？升级 Pro 启用 YouBase
         → 发布到 youware.app 或自定义域名
```

#### 场景 2：改进现有项目
```
难以文字描述？用 Coview 录屏指出问题
                → AI 自动识别并修复
简单样式调整？直接 Visual Editing（最省 Credits）
复杂功能？Chat 模式或 Code Editor 手动编辑（Pro/Ultra）
```

#### 场景 3：基于社区项目快速启动
```
Remix 现有项目（复制免费）→ 三个预设按钮：换内容/换主题/加功能
                            → 只有 AI 修改才消耗 Credits
                            → 自动归因原作者
```

#### 场景 4：需要后端服务
```
Pro/Ultra 用户 → 描述需求时提到"需要登录/数据库/文件上传"
               → AI 自动配置 YouBase（Database/Auth/Storage/Secrets）
               → 零配置，Production-Ready
               → 时光机功能可回溯数据（Ultra）
```

---

### 功能速查表（场景化）

| 你想要... | 推荐使用 | Credits 消耗 | 注意事项 |
|-----------|----------|--------------|----------|
| 快速生成 MVP | AI Generation（Gemini 低成本） | 中等 | 先构建核心链路，别追求完美 |
| 改样式/颜色/间距 | Visual Editing | 极低 | 优先用这个，最省钱 |
| 说不清楚问题 | Coview 录屏 | 中等 | 30 秒内，聚焦单一问题 |
| 复制设计稿 | Figma Connection | 中等 | 分段导入，别一次整个页面 |
| 添加复杂功能 | Chat Mode（Sonnet） | 高 | 逻辑复杂用 Sonnet，样式用 Gemini |
| 需要数据库/登录 | YouBase（Pro/Ultra） | - | 零配置，描述需求即可 |
| 发布上线 | One-Click Publish | 免费 | 免费域名 youware.app |
| 集成外部服务 | MCP Tools | 低-中 | Notion/GitHub/YouTube 等 |
| 不满意结果 | Credit Care 退款 | 退还 | 月度额度内可退 |

---

### 关键限制和常见误区

#### ❌ 什么是 YouWare **不能**做的

1. **不支持移动端原生开发** - 只能做 Web 应用（PWA 可用）
2. **YouBase 不能手动编辑数据** - 数据库是"查看为主"，不能像 Supabase 那样直接改表
3. **Remix 项目不能下载源码** - 只能在线修改
4. **Free 计划不能用 YouBase** - 后端功能需要 Pro/Ultra
5. **不能像传统 IDE 那样调试** - 主要靠 AI 修复，不支持断点调试

#### ⚠️ 常见误区纠正

| 误区 | 正确理解 |
|------|----------|
| "AI 一次就能做对" | 需要迭代，"干中学"比一开始追求完美更高效 |
| "Credits 很快用完" | Visual Editing 极低消耗，先用它微调再用 AI |
| "后端需要额外配置" | YouBase 零配置，描述需求时提到即可自动开启 |
| "不满意就浪费 Credits" | Credit Care 可退款（月度额度内） |
| "必须详细描述需求" | Coview 录屏比文字描述更高效 |

---

### 推荐工作流（最佳实践）

#### 完整项目流程（0→1）

```
1. 需求阶段
   ├─ 别直接说功能，先让 AI 生成需求文档
   └─ 明确核心链路（MVP），别贪多

2. 生成阶段
   ├─ 选模型：快速原型用 Gemini，复杂逻辑用 Sonnet
   ├─ 提示词：先描述情绪/氛围，再说功能（参考 Prompting 102）
   └─ 需要后端？直接说"需要用户登录和数据库"

3. 调优阶段
   ├─ 先用 Visual Editing 改样式（省 Credits）
   ├─ 说不清楚？Coview 录屏指出问题
   ├─ 复杂修改？Chat Mode 对话式调整
   └─ 不满意？History 回滚 + Credit Care 退款

4. 集成阶段（可选）
   ├─ 内容从 Notion 同步
   ├─ 设计稿从 Figma 导入
   └─ 代码托管到 GitHub

5. 发布阶段
   ├─ 免费域名：youware.app
   ├─ 自定义域名：Pro/Ultra（配置 CNAME）
   └─ 私密访问：设置密码（Pro/Ultra）
```

#### 日常使用建议

- **每次只改一个问题** - 不要一次提 10 个需求
- **先用 Tab Tab 补全** - 智能提示比自己想更准确
- **善用 Boost** - 一键优化比手动调整快
- **从自用工具开始** - 小规模试错，边用边学

---

### 定价速查

| Plan | 价格 | Credits/月 | 项目数 | 适合人群 |
|------|------|------------|--------|----------|
| **Free** | $0 | 试用额度 | 5 | 体验产品 |
| **Pro** | $20/月 | 3,000 | 100 | 个人开发者、SMB、设计师 |
| **Ultra** | $200/月 | 36,000 | 无限 | 重度用户、商业项目 |

**Credits 系统：**
- 不同 AI 模型价格不同（Gemini < Sonnet）
- Visual Editing 极低消耗
- Credits 有效期 2 年，月度滚动
- Credit Care：不满意可退款（月度额度：Free 1 次 / Pro 30 次 / Ultra 150 次）

---

### 快速决策指南

#### 问：用户问"YouWare 能做 XXX 吗？"如何判断？

**判断逻辑：**
1. 是 Web 应用？✅  移动原生 App？❌
2. 需要后端？Pro/Ultra ✅，Free ❌
3. 需要手动改数据库？❌（YouBase 设计如此）
4. 需要复杂权限控制？基础够用 ✅，企业级 IAM ❌
5. 需要实时通信？WebSocket 可用 ✅

#### 问：用户抱怨"AI 生成的不对"怎么办？

**解决路径：**
1. 先问：有没有用 Coview 录屏？→ 比文字描述准确 10 倍
2. 再问：是样式问题还是逻辑问题？
   - 样式 → Visual Editing 直接改（省 Credits）
   - 逻辑 → Chat Mode 详细描述
3. 提醒：不满意可以 History 回滚 + Credit Care 退款

#### 问：用户在 Lovable/Bolt 和 YouWare 之间犹豫？

**推荐话术：**
- 需要后端？YouWare 包含 YouBase，Lovable 额外收费
- 不会描述需求？YouWare 有 Coview 录屏
- 担心浪费钱？YouWare 有 Credit Care 退款机制
- 移动端办公？YouWare 有原生 App

---

## Quick Reference

| 需求 | 资源 |
|------|------|
| 回答功能问题 | `docs/*.md` |
| 查看实战案例 | `references/tutorials/*.md` |
| 查看术语/最佳实践 | `references/*.md` |
| 竞品对比 | `competitive/*.md` |
| GTM 策划/产品定位 | `gtm/*.md` |
| 添加新教程 | 新建 `references/tutorials/XX-name.md` |

## Official Documentation

### Product Overview
- [docs/PRODUCT-OVERVIEW.md](docs/PRODUCT-OVERVIEW.md) - **Complete product description**: What YouWare is, core features, YouBase backend, MCP connections, prompting best practices, terminology

### Getting Started
- [docs/GETTING-STARTED.md](docs/GETTING-STARTED.md) - Quick start guide, first project workflow

### Features
- [docs/FEATURES.md](docs/FEATURES.md) - Visual editing, Boost, Code View, Tab Tab, History

### Pricing
- [docs/PLANS.md](docs/PLANS.md) - Free, Pro, Ultra plans, credit system, Credit Care

### Backend
- [docs/YOUBASE.md](docs/YOUBASE.md) - Database, Users & Auth, Storage, Secrets

### Integrations
- [docs/INTEGRATIONS.md](docs/INTEGRATIONS.md) - MCP tools, Figma, Notion, GitHub, Supabase, Google Maps

### Mobile
- [docs/MOBILE.md](docs/MOBILE.md) - iOS/Android apps, push notifications, cross-device sync

## Competitive Intelligence

**Data Updated:** 2026-02-03 (Web Sync)

| 文档 | 内容 |
|------|------|
| [competitive/landscape.md](competitive/landscape.md) | 竞品全景对比 |
| [competitive/feature-matrix.md](competitive/feature-matrix.md) | 功能矩阵 |
| [competitive/_data/](competitive/_data/) | 原始 changelog 数据 (JSON) |

### 竞品列表
YouWare, Lovable, Bolt, v0, Replit, Trickle, Base44, Rocket

### 功能分类 (18个)
AI Model, Agent, Media, Editor, Backend, Integration, Deployment, Auth, Team, UI/UX, Performance, Billing, Framework, Analytics, Community, File, Security, Others

## Community Tutorials & Knowledge Base

### Reference Files
- [references/index.md](references/index.md) - Overview and tutorial index
- [references/terminology.md](references/terminology.md) - Key terms glossary
- [references/best-practices.md](references/best-practices.md) - Best practices
- [references/url-map.md](references/url-map.md) - Documentation URL mapping

### Tutorials (11 total)
| File | Topic |
|------|-------|
| [tutorials/01-vibe-diary.md](references/tutorials/01-vibe-diary.md) | Vibe Coding 全平台应用指南 |
| [tutorials/02-coview-fuli.md](references/tutorials/02-coview-fuli.md) | CoView 实战 - 乔木福利社 |
| [tutorials/03-art-museum.md](references/tutorials/03-art-museum.md) | 3小时在线艺术博物馆 |
| [tutorials/04-membership-ja.md](references/tutorials/04-membership-ja.md) | 会员服务自制 (日文) |
| [tutorials/05-sales-management.md](references/tutorials/05-sales-management.md) | 销售库存客户管理 |
| [tutorials/06-5min-website.md](references/tutorials/06-5min-website.md) | 5分钟创建网站 |
| [tutorials/07-rpg-game.md](references/tutorials/07-rpg-game.md) | Web 游戏存档功能 |
| [tutorials/08-prompt-tool.md](references/tutorials/08-prompt-tool.md) | AI 绘图提示词工具 |
| [tutorials/09-couple-app.md](references/tutorials/09-couple-app.md) | 二人专属应用 + Remix |
| [tutorials/10-shorts-breakdown.md](references/tutorials/10-shorts-breakdown.md) | YouTube Shorts 拆解 |
| [tutorials/11-sponsored-video.md](references/tutorials/11-sponsored-video.md) | YouTube 赞助视频拆解 |

## GTM (Go-to-Market) 资料

| 文档 | 内容 |
|------|------|
| [gtm/index.md](gtm/index.md) | GTM 资料索引和速查 |
| [gtm/youbase-launch.md](gtm/youbase-launch.md) | YouBase 发布策划 |
| [gtm/coview-launch.md](gtm/coview-launch.md) | CoView 发布策划 |

---

## Sync Official Docs

When user says **"sync youware docs"** or **"更新 youware 文档"**, follow this workflow:

### Step 1: Fetch Sitemap

```
WebFetch: https://docs.youware.com/sitemap.xml
Prompt: "Extract all documentation URLs from this sitemap"
```

### Step 2: Fetch Each Section

Fetch these key pages and extract content:

| Section | URL |
|---------|-----|
| Quick Start | https://docs.youware.com/introduction/quickstartguide |
| Plans & Pricing | https://docs.youware.com/introduction/plans-and-pricing |
| FAQ | https://docs.youware.com/introduction/faq |
| Boost | https://docs.youware.com/features/boost |
| Visual Editing | https://docs.youware.com/features/visual-editing |
| Tab Tab | https://docs.youware.com/features/tab-tab-completion |
| Remix | https://docs.youware.com/features/remix |
| Custom Domain | https://docs.youware.com/features/custom-domain |
| YouBase Intro | https://docs.youware.com/youbase/introduction |
| Database | https://docs.youware.com/youbase/database |
| Users & Auth | https://docs.youware.com/youbase/users-authentication |
| Storage | https://docs.youware.com/youbase/storage |
| Secrets | https://docs.youware.com/youbase/secrets |
| Figma | https://docs.youware.com/connections/figma-connection |
| GitHub | https://docs.youware.com/connections/github-connection |
| Notion | https://docs.youware.com/connections/notion-connection |

### Step 3: Update Local Docs

For each fetched page:
1. Compare with existing `docs/*.md` content
2. Update if there are changes
3. Note what changed

### Step 4: Update Metadata

1. Update `Last Synced` date in this file
2. Update `references/index.md` timestamp
3. Report changes to user

### Sync Output Format

```
## Sync Complete

**Date:** YYYY-MM-DD
**Pages Checked:** X
**Pages Updated:** Y

### Changes:
- FEATURES.md: Added new Boost options
- PLANS.md: Updated Ultra plan pricing
- (etc.)
```

---

## Adding New Tutorials

When user provides tutorial links or pastes content:

1. **Fetch content** - Use WebFetch; if blocked, ask user to paste
2. **Extract key info** - Title, case study, workflows, tips, prompts
3. **Create new file** - `references/tutorials/NN-name.md`
4. **Update index** - Add entry to `references/index.md`

### Tutorial Template

```markdown
# Tutorial N: {Title}

**来源:** {Source}
**核心案例:** {Product Name} ({URL})

## 案例产品功能
| 功能 | 描述 |
...

## {Key Sections}
...
```

---

## Sync Competitive Data

When user says **"sync competitive"** or **"更新竞品数据"**, follow this workflow:

### Method 1: Web Crawling (推荐)

直接从竞品官网爬取最新 changelog：

#### Competitor Changelog URLs

| 竞品 | Changelog URL |
|------|---------------|
| v0 | https://v0.app/changelog |
| Replit | https://docs.replit.com/updates/ |
| Lovable | https://docs.lovable.dev/changelog |
| Trickle | https://feedback.trickle.so/changelog |
| Base44 | https://base44.com/changelog |
| Bolt | https://support.bolt.new/release-notes |
| Rocket | https://docs.rocket.new/inspiration-and-help/changelog |

#### Crawl Workflow

1. **Fetch each changelog page**:
```
WebFetch: {changelog_url}
Prompt: "Extract all feature updates with dates. For each update, include: date, title, description, and categorize into tags (AI Model, Agent, Media, Editor, Backend, Integration, Deployment, Auth, Team, UI/UX, Performance, Billing, Framework, Analytics, Community, File, Security, Others)"
```

2. **Compare with existing data** in `_data/storage/{competitor}.json`

3. **Append new entries** to JSON files:
```json
{
  "time": "YYYY-MM-DD",
  "title": "Feature Name",
  "content": "Description...",
  "tag": "Category",
  "subtag": "Subcategory"
}
```

4. **Update summary docs**:
   - `landscape.md` - 如有新竞品定位变化
   - `feature-matrix.md` - 如有新功能需要对比

5. **Update timestamps**:
   - 本文件的 `Data Updated` 日期
   - `landscape.md` 的 `Last Updated` 日期
   - `feature-matrix.md` 的 `Last Updated` 日期

### Method 2: Local Data Import

如果用户提供新的数据文件夹路径：

```bash
cp -r {新数据路径}/* ~/.claude/skills/youknowledge/competitive/_data/
```

然后执行同样的更新流程。

### Update Checklist

- [ ] 爬取/导入新数据
- [ ] 检查各竞品最新日期
- [ ] 更新 landscape.md（如有变化）
- [ ] 更新 feature-matrix.md（如有新功能）
- [ ] 更新所有 `Last Updated` / `Data Updated` 日期

### Competitive Query Examples

用户可能问：
- "Lovable 最近更新了什么？" → 读 `_data/storage/lovable.json`
- "谁先有了 MCP 集成？" → 搜索各 JSON 中 "MCP" 标签
- "YouWare vs Bolt 后端对比" → 读 `feature-matrix.md` Backend 部分

### Sync Output Format

```
## Competitive Sync Complete

**Date:** YYYY-MM-DD
**Competitors Checked:** 7
**New Updates Found:** X

### New Features by Competitor:
- **Lovable**: Added XYZ feature (2026-01-XX)
- **Bolt**: Updated ABC (2026-01-XX)
- (etc.)

### Feature Matrix Updates:
- Added row for "New Feature X"
- Updated Lovable column for "Backend"
```

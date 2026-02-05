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

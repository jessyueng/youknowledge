# YouWare Product Overview

**Last Updated:** 2026-02-11

This document contains comprehensive information about YouWare, providing a complete understanding of what YouWare is and what it can do.

---

## What is YouWare?

YouWare is an AI-powered platform for building web applications without coding. Users describe their ideas in natural language, and AI builds complete projects in approximately 30 seconds. The platform provides editing, customization, and publishing capabilities within an integrated workspace.

**Core Value Proposition:** Transform ideas into functional websites and web applications through natural language descriptions, with AI handling the technical implementation.

**Target Users:**
- Non-technical users who want to build websites
- Designers who want to convert designs to code
- Developers who want rapid prototyping
- Creators who want to monetize their work

---

## Core Features

### Project Creation

#### Build from Scratch
- Describe idea in natural language in the Creative Command Center
- AI generates complete project in ~30 seconds
- Specific feature descriptions yield better results

#### Remix
- Copy and modify existing community projects
- Three preset buttons: Replace Content, Change Theme, Add Section
- Original project remains unchanged
- Remixed projects cannot be downloaded as source code
- Only pay credits when requesting AI modifications; copying is free

#### Upload Code
- Import existing project files
- Automatic tech stack detection
- Supports: React, Vue, Angular, Next.js, HTML/CSS/JS, Node.js, Python, PHP
- Preserves git history and project structure

### Editing Tools

#### Chat with AI
- Conversational editing with context awareness
- Complex changes through natural language
- Maintains project context across conversations

#### Visual Editing
- Click elements directly in preview to modify
- Text: font size, color, styling, alignment, padding, margin, hyperlinks
- Images: replace (PNG, JPG, SVG, WEBP, GIF), corner radius, padding, margin, hyperlinks
- Other elements: styling, corner radius, background color, remove
- Minimal credit consumption compared to AI-driven edits

#### Code View
- Browse HTML, CSS, JavaScript files
- View project file organization
- Subscribers can edit and save directly with real-time preview
- Free users can view but not edit

#### Boost
- One-click AI optimization
- Analyzes: page structure, content quality, user experience
- Preserves original design intent
- No configuration required

#### History
- Automatic version saving with timestamps
- Preview any version before restoring
- Captures: code, visual edits, AI updates, manual edits
- **Warning:** Restoring deletes all versions after restoration point
- Credits not refunded on restore (use Credit Care instead)

#### Tab Tab Completion
- AI-powered prompt auto-completion
- Press Tab to accept suggestions
- Context-aware based on project and task
- Works on creation page and throughout editor

### Publishing & Sharing

#### One-Click Publishing
- Instant deployment to YouWare domain (abc.youware.app)
- Customize project title and cover image
- Generate shareable links

#### Privacy Controls (Paid Plans)
- Private Projects: 4-character password protection
- Remix Permissions: Toggle to allow/disable copying
- Remove YouWare badge

#### Custom Domains (Pro/Ultra)
- Requires TXT record for verification (`_youware-verify`)
- Requires CNAME record for traffic routing
- Root domains need Cloudflare or subdomain workaround
- Supports private access with passcode

#### Creator Studio
- Track total views and credits consumed
- Per-project metrics: Credits Spent, Times Used, Views, Built On/Saves
- Earnings management with $50 minimum withdrawal
- Transaction history updated daily

### Multi-Model Switching

Five AI models available:
- OpenAI
- Anthropic (Claude)
- Moonshot
- Z.ai
- GLM

Click model name (bottom-right of input) to switch. Each model shows speed, intelligence, cost, and capabilities.

### Mobile App

**Key Features:**
- Voice Input: Describe ideas verbally
- Photo Integration: Snap photos for AI reference
- Task Notifications: Background processing with push alerts
- Code Editing: Full Code View with syntax highlighting
- Cross-Device Sync: Continue projects on any device

**Availability:** iOS App Store, Google Play (search "YouWare")

### IDE Extension

- Supports VS Code and Cursor
- Publish projects directly from editor
- Instant deployment and shareable links
- No command-line or server configuration needed

---

## YouBase Backend Services

YouBase is YouWare's built-in cloud backend infrastructure. Available on **Pro and Ultra plans only**.

### Key Capabilities
- Data Storage: Complete database functionality
- User Authentication: Enterprise-level access controls
- File Management: Cloud-based storage
- Server-side Logic: Computational processing
- Automatic Scaling: From prototypes to millions of users
- Zero-configuration setup through natural language

### Database Module
- View all tables with row counts
- Browse records with pagination (25/50/100 rows)
- Export full database or individual tables as ZIP
- Time Travel with bookmarks (System/Manual/Restore)
- **Cannot** manually add, edit, or delete rows (by design)
- Pro: 14-day history (no restore)
- Ultra: Full restore and bookmark creation

### Users & Authentication
- **Email Login:** Traditional email/password with verification
- **Google OAuth:** One-click login
- **Temporary Accounts:** Anonymous access for trials
- User operations: Add, Delete, Block, Unblock
- Email security: verification, password reset codes, device logout
- Immutable user IDs for data association

### Storage
- User-uploaded files in the cloud
- Single file or ZIP bundle downloads
- No file preview or deletion (by design)
- Pro/Ultra only

### Secrets
- Secure API key storage with enterprise-grade encryption
- Server-side only (never reaches frontend)
- Up to 64 secrets per project
- Common uses: third-party API keys, AI model credentials, service tokens

---

## MCP Connections

MCP Tools (Model Context Protocol) are pre-built connections that extend project capabilities like plugins.

### Built-in Tools (no setup required)
- Animation Library
- Icon Library
- Image Generator
- Unsplash

### Highly Recommended

**Figma Connection:** Convert designs to pixel-perfect, responsive code
- Requires Personal Access Token with file_content:read, file_dev_resources:read, projects:read scopes
- Convert section-by-section for best results

### Other Connections

**GitHub**
- Repository sync, version control, code backup
- AI learns your codebase structure and coding style
- Requires Personal Access Token

**Supabase**
- External database integration
- AI reads schema for data-aware code generation
- Requires Service Role Key (not Anon Key)

**Notion**
- Use Notion as CMS for your website
- Auto-sync content changes
- Requires Internal Integration Secret

**YouTube**
- Live video galleries, channel profiles, analytics dashboards
- No API key required
- Pulls real-time metadata: titles, thumbnails, view counts

**Google Maps**
- Location data, reviews, ratings, map embeds
- No API key required
- Best for: travel guides, store locators, real estate

**arXiv**
- Academic paper integration
- No authentication required
- Best with category tags (cs.CL, cs.AI) or keywords

### Usage Notes
- More enabled tools = longer generation time
- Enable only necessary tools initially
- Add more tools later as needed

---

## Credit Care

Credit Care allows users to recover credits when AI results don't meet expectations.

### How It Works
1. Create with AI
2. Not satisfied? Click "Rewind to previous version"
3. Select "Rewind & refund Credits"
4. Project reverts; Credits refund instantly

### Monthly Limits
| Plan | Credit Restores/Month |
|------|----------------------|
| Free | 1 |
| Pro | 30 |
| Ultra | 150 |

### Important Notes
- Restoring is **permanent** - loses all versions after rewind point
- 0-credit commits (manual edits) don't consume monthly allowance

---

## Prompting Best Practices

### Three Golden Rules

1. **Lead with Emotion, Not Mechanics**
   - Describe the desired feeling or atmosphere
   - Instead of "header, three-column layout, footer"
   - Say "cozy, rainy-day bookstore vibe—warm and nostalgic"

2. **Structure as Narrative**
   - Chapter 1 (Hook): Capture attention
   - Chapter 2 (Why): Value proposition
   - Chapter 3 (Proof): Credibility
   - Chapter 4 (Invitation): Call to action

3. **Refine Iteratively**
   - Treat outputs as "first lump of clay"
   - Provide conversational feedback
   - Focus on one element at a time

### Key Insight
"Your idea is the masterpiece. Your words are the direction." Act as art director, not machine operator.

---

## Key Terminology

| Term | Definition |
|------|------------|
| Credits | Usage-based currency for AI generation and services |
| Credit Care | Monthly credit restores for failed AI attempts |
| Remix | Starting from existing project and customizing it |
| Boost | One-click AI enhancement for pages |
| Tab Tab | AI-powered prompt auto-completion (press Tab) |
| YouBase | Built-in cloud backend infrastructure |
| MCP Tools | Model Context Protocol integrations (plugins) |
| Creator Studio | Analytics and monetization dashboard |
| Visual Editing | Point-and-click UI modifications |
| Code View | Full source editor with syntax highlighting |
| History | Version control with restore capability |
| Coview | Screen recording feature for showing AI what to build |

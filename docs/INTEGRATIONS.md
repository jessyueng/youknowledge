# YouWare Integrations & MCP Tools

Guide to YouWare's Model Context Protocol (MCP) tools and external service integrations.

## MCP Tools Overview

MCP (Model Context Protocol) tools extend YouWare's AI capabilities by connecting to external services and resources.

---

## Built-in Tools (No Setup Required)

These tools work automatically without configuration.

### Animation Library

Add professional animations to your projects.

**Features:**
- Pre-built animation presets
- Entrance, exit, and attention animations
- Scroll-triggered effects
- Hover animations
- Customizable timing and easing

### Icon Library

Access thousands of icons for your designs.

**Features:**
- Multiple icon sets
- Customizable colors and sizes
- SVG format for scalability
- Search by keyword

### Image Generator

AI-powered image creation.

**Features:**
- Generate images from text descriptions
- Multiple style options
- Various aspect ratios
- Direct integration with projects

### Unsplash

Access millions of free stock photos.

**Features:**
- High-quality professional photography
- Search by keyword or category
- Free for commercial use
- Automatic attribution handling

---

## External Integrations

Connect external services for enhanced capabilities.

### Figma

Convert Figma designs to pixel-perfect web code.

**Best For:**
- Portfolio sites from designs
- Product landing pages
- MVP development
- Designer-to-developer handoff

**Setup Requirements:**
- Personal Access Token with scopes:
  - `file_content:read`
  - `file_dev_resources:read`
  - `projects:read`

**How to Use:**
1. Open your Figma design
2. Select the component or section
3. Copy link to selection
4. Paste in YouWare chat
5. AI generates matching code

**Best Practice:** Convert section-by-section for better accuracy rather than entire pages at once.

---

### Notion

Use Notion as a CMS for YouWare projects.

**Best For:**
- Content-driven blogs
- Product catalogs
- Team directories
- Documentation sites

**Setup Requirements:**
- Internal Integration Secret from Notion
- Share relevant pages with the integration

**Features:**
- Content-first development
- Automatic updates when Notion changes
- Database support for structured content
- Real-time sync

---

### GitHub

Connect to GitHub for version control and collaboration.

**Best For:**
- Open-source documentation
- Code consistency across projects
- Team-based development
- Full version history

**Setup Requirements:**
- Personal Access Token with public repository access

**Features:**
- Version control integration
- AI reads existing code for context
- Team collaboration via Pull Requests
- Full rollback capability
- Automatic backup

---

### Supabase

Connect to Supabase for external database and backend.

**Best For:**
- Analytics dashboards
- Real-time inventory trackers
- Data-driven applications
- Complex database needs

**Setup Requirements:**
- Service Role Key from Supabase project

**Features:**
- Data-aware code generation
- Real-time database connectivity
- Full-stack cohesion
- Edge Functions support
- Row Level Security integration

**When to Choose Supabase vs YouBase:**

| Need | Choose |
|------|--------|
| Simple, quick setup | YouBase |
| Existing Supabase project | Supabase |
| Advanced PostgreSQL features | Supabase |
| Zero configuration | YouBase |
| Real-time subscriptions | Supabase |

---

### Google Maps

Pull live location data, reviews, and map embeds.

**Best For:**
- Travel guides
- Store locators
- Competitor research
- Real estate landing pages
- City portals

**Data Available:**
- Business names and categories
- Ratings and reviews
- Operating hours
- Addresses and coordinates
- Photos
- Navigation links

**Features:**
- Location directories
- Interactive landing pages
- Competitor dashboards
- Embedded maps

---

### YouTube

Integrate YouTube content into your projects.

**Best For:**
- Video portfolios
- Course platforms
- Content creator sites
- Product demos

**Features:**
- Embed videos
- Pull channel data
- Video galleries
- Playlist integration

---

### arXiv

Access research papers for content generation.

**Best For:**
- Research-driven projects
- Academic content
- Technical documentation
- Scientific applications

**Features:**
- Search research papers
- Pull paper metadata
- Generate content summaries
- Reference management

---

## MCP Market

Discover and install MCP tools from the marketplace.

**Features:**
- Browse tools by category
- One-click installation
- Tool management (enable/disable/remove)
- Setup guides for authorized tools

**How to Access:**
1. Open project settings
2. Navigate to "MCP Tools" or "Connections"
3. Browse available tools
4. Click to install and configure

---

## Integration Selection Guide

| Need | Recommended Tool |
|------|------------------|
| Design to code | Figma |
| Data storage (simple) | YouBase |
| Data storage (advanced) | Supabase |
| Dynamic content | Notion |
| Version control | GitHub |
| Location data | Google Maps |
| Video content | YouTube |
| Research content | arXiv |
| Stock images | Unsplash |
| Icons | Icon Library |
| Animations | Animation Library |
| AI images | Image Generator |

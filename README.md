# Snapchat Ads MCP Server by Insightful Pipe

[![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)](https://insightfulpipe.com/mcp-servers/snapchat-ads)
[![Insightful Pipe](https://img.shields.io/badge/Insightful_Pipe-MCP_Servers-purple)](https://insightfulpipe.com/mcp-servers)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Connect Snapchat Ads to AI assistants for Gen-Z marketing analytics and AR advertising insights.**

Part of the [Insightful Pipe MCP Server Collection](https://insightfulpipe.com/mcp-servers) — The Snapchat Ads MCP server enables Claude, ChatGPT, Cursor, and other AI assistants to analyze your Snapchat advertising campaigns. Reach Gen-Z audiences, optimize creatives, and get AI-powered recommendations.

[![Explore All MCP Servers](https://img.shields.io/badge/Explore_All-MCP_Servers-blue?style=for-the-badge)](https://insightfulpipe.com/mcp-servers)

![Snapchat Ads MCP Server](https://insightfulpipe.com/images/snapchat.svg)

## MCP Server URL

```
https://snapchat-ads.insightfulmcp.com/
```

## What is Snapchat Ads MCP?

Snapchat Ads MCP is a **remote Model Context Protocol server** that connects your Snapchat Ads Manager to AI assistants. This Gen-Z focused integration allows you to:

- Query Snapchat ad performance using natural language
- Analyze Story Ads and creative engagement
- Track swipe-up rates and conversion metrics
- Access media assets and audience segments
- Get AI recommendations for optimization

## Installation

### Claude

1. Copy the MCP Server URL: `https://snapchat-ads.insightfulmcp.com/`
2. Open [Claude Connectors Settings](https://claude.ai/settings/connectors)
3. Scroll to the bottom and click **Add custom connector**
4. Paste the URL and click **Add**
5. Click **Connect** on the connector to start authorization
6. Click **Authorize access** in the browser to complete the connection

### ChatGPT

Custom MCP servers are added through ChatGPT's **Developer mode**. Availability depends on your ChatGPT plan, and workspace admins may need to allow it.

1. Turn on **Developer mode** in ChatGPT settings
2. Create a new app for a remote MCP server and paste the URL: `https://snapchat-ads.insightfulmcp.com/`
3. Authorize with your InsightfulPipe account

See OpenAI's guide: [Developer mode and MCP apps in ChatGPT](https://help.openai.com/en/articles/12584461-developer-mode-and-mcp-apps-in-chatgpt)

### Claude Code

```bash
claude mcp add --transport http snapchat-ads https://snapchat-ads.insightfulmcp.com/
```

### Cursor

Add the server to `~/.cursor/mcp.json` (all projects) or `.cursor/mcp.json` (one project):

```json
{
  "mcpServers": {
    "snapchat-ads": {
      "url": "https://snapchat-ads.insightfulmcp.com/"
    }
  }
}
```

Then authorize the connection when Cursor prompts you.

## Available Actions

32 actions: 24 read, 8 write.

### Read Actions (24)

| Action | Description |
|--------|-------------|
| `get_ad` | Fetch a single ad, e.g. to read its current values before updating it |
| `get_ad_stats` | Retrieve performance statistics for a specific ad |
| `get_adaccount` | Fetch details for a single ad account |
| `get_adaccount_stats` | Retrieve performance statistics for an ad account |
| `get_adaccounts_by_organization` | List ad accounts for a specific organization |
| `get_ads` | List ads for an ad account |
| `get_ads_by_adsquad` | List the ads inside one ad squad |
| `get_ads_by_campaign` | List the ads inside one campaign |
| `get_adsquad` | Fetch a single ad squad, e.g. to read its current values before updating it |
| `get_adsquad_stats` | Retrieve performance statistics for a specific ad squad |
| `get_adsquads` | List ad squads for an ad account |
| `get_adsquads_by_campaign` | List the ad squads inside one campaign |
| `get_campaign` | Fetch a single campaign, e.g. to read its current values before updating it |
| `get_campaign_stats` | Retrieve performance statistics for a specific campaign |
| `get_campaigns` | List campaigns for an ad account |
| `get_creative` | Fetch a single creative, e.g. to read its current values before updating it |
| `get_creatives` | List creatives for an ad account |
| `get_media` | List media assets for an ad account |
| `get_media_detail` | Fetch metadata for a single media asset |
| `get_media_preview` | Retrieve a preview URL for a media asset |
| `get_media_thumbnail` | Retrieve a thumbnail URL for a media asset |
| `get_organization` | Fetch details for a single organization |
| `get_organizations` | List organizations the authenticated user can access |
| `get_segments` | List audience segments for an ad account |

### Write Actions (8)

| Action | Description |
|--------|-------------|
| `create_ad` | Create an ad within an ad squad |
| `create_adsquad` | Create an ad squad within a campaign |
| `create_campaign` | Create a campaign within an ad account |
| `create_creative` | Create a creative within an ad account |
| `update_ad` | Update one ad |
| `update_adsquad` | Update one ad squad |
| `update_campaign` | Update one campaign |
| `update_creative` | Update one creative |

## Usage Examples

### Campaign Performance

```
"How are my Snapchat campaigns performing this week?"
```

### Ad Squad Analysis

```
"Which ad squads have the highest swipe-up rate?"
```

### Creative Performance

```
"Show me my top performing Snapchat creatives"
```

### Media Assets

```
"List all my media assets and their thumbnails"
```

### Audience Segments

```
"What audience segments do I have available?"
```

## Supported Metrics

| Metric | Description |
|--------|-------------|
| Impressions | Total ad views |
| Swipe Ups | Users who swiped up |
| Swipe Up Rate | Swipes / impressions |
| Video Views | Video ad views |
| Completion Rate | Users who watched full video |
| Screen Time | Average ad viewing time |
| Shares | Content shares |
| Conversions | Pixel-tracked conversions |

## Why Snapchat Ads MCP?

### For Gen-Z Focused Brands
- **Youth engagement** - Reach 13-34 demographic
- **Creative insights** - Understand what resonates
- **Cultural relevance** - Stay connected to trends

### For App Marketers
- **App install tracking** - Mobile app campaigns
- **Deep linking** - In-app conversion data
- **Re-engagement** - App retargeting metrics

### For Agencies
- **Multi-account management** - Handle brand accounts
- **Creative benchmarking** - Compare ad performance
- **Automated reporting** - Client-ready insights

## Security & Privacy

- **Official Snapchat Marketing API** - Direct integration with Snap's API
- **OAuth 2.0** - Secure authentication

## Explore More MCP Servers by Insightful Pipe

Visit **[insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)** to discover our full collection of MCP servers for marketing and analytics.

### Gen-Z & Social MCP Servers
- [TikTok Ads MCP](https://insightfulpipe.com/mcp-servers/tiktok-ads) - Gen-Z video advertising
- [Instagram MCP](https://insightfulpipe.com/mcp-servers/instagram) - Visual social analytics
- [Pinterest Ads MCP](https://insightfulpipe.com/mcp-servers/pinterest-ads) - Visual discovery advertising

### Advertising MCP Servers
- [Facebook Ads MCP](https://insightfulpipe.com/mcp-servers/facebook-ads) - Social advertising
- [Google Ads MCP](https://insightfulpipe.com/mcp-servers/google-ads) - Search advertising

**[View All MCP Servers →](https://insightfulpipe.com/mcp-servers)**

## Resources

- [Documentation](https://insightfulpipe.com/docs/connectors-snapchat-ads)
- [Video Tutorial](https://www.youtube.com/playlist?list=PLJNzvjxzI5Xwe__BJJLAelSF0ewO3mEFk)
- [InsightfulPipe Blog](https://insightfulpipe.com/blog)

## Support

- **Documentation**: [insightfulpipe.com/docs](https://insightfulpipe.com/docs)
- **All MCP Servers**: [insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)
- **Email**: support@insightfulpipe.com

---

**[Insightful Pipe](https://insightfulpipe.com)** — AI-powered marketing analytics through MCP servers. [Explore all integrations →](https://insightfulpipe.com/mcp-servers)

## License

MIT License - see [LICENSE](LICENSE) for details.

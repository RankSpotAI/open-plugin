# SEO with RankSpot: AI SEO, GEO and AI visibility for Cursor

<img src="assets/logo.png" alt="SEO with RankSpot" width="96" />

Do SEO, AI SEO and GEO (generative engine optimization) without leaving Cursor. Connect the agent to your [RankSpot](https://www.rankspot.ai) workspaces to track your AI visibility in ChatGPT, Perplexity and Google AI answers, research keywords and competitors, and write and publish SEO articles, all in plain English from the agent chat.

This plugin adds the hosted RankSpot MCP server (`https://mcp.rankspot.ai`, Streamable HTTP). There is nothing to install or run locally.

## What your agent can do

- **AI visibility (GEO / AEO)**: see how ChatGPT, Perplexity and Google AI answers describe your brand, which pages they cite, and which searches they run.
- **Keyword research**: track keywords, read search volume and competition, and pull the semantic cluster around any seed term.
- **Competitors and backlinks**: track competitor domains and find sites linking to them but not to you.
- **Content**: plan work as actions, generate publish-ready articles, edit them, restore earlier revisions, and publish to your connected site.
- **Search Console**: read clicks, impressions, CTR and position, check whether a page is indexed, and request indexing.
- **Live research**: run a live Google search or fetch any public page as clean markdown.
- **Outreach**: find the right contact on a site and send link-building emails from your connected mailbox, then track replies.

## Setup

1. Create a RankSpot account at [rankspot.ai](https://www.rankspot.ai) and finish your workspace setup.
2. Install the plugin from the Cursor Marketplace.
3. The first time the agent calls a RankSpot tool, Cursor opens a RankSpot sign-in page. Log in, review the organizations and workspaces the app will reach, and approve.

Cursor stores and refreshes the tokens for you. Revoke access any time under **Account settings → Connected Apps** in RankSpot.

### Using an API key instead

If you prefer an API key, skip the plugin and add the server to `~/.cursor/mcp.json` yourself. Create a key under **Account settings → API Keys**:

```json
{
  "mcpServers": {
    "rankspot": {
      "url": "https://mcp.rankspot.ai",
      "headers": {
        "Authorization": "Bearer YOUR_RANKSPOT_API_KEY"
      }
    }
  }
}
```

## Example prompts

- "How often is my brand mentioned in AI answers this month, and which competitors show up more?"
- "Which Search Console queries are close to page one, and what should I do about them?"
- "Find three content gaps against my competitors and plan an article for each."

## Notes

- Search Console tools need a connected Search Console property, publishing needs a connected website, and outreach needs a connected mailbox.
- Article generation and some research tools use your usage allowance.
- Publishing, sending email and deleting happen only when you ask, and deletes require explicit confirmation.

## Links

- [RankSpot MCP](https://www.rankspot.ai/mcp)
- [Privacy policy](https://www.rankspot.ai/privacy)
- [Terms of service](https://www.rankspot.ai/terms)
- [Support](https://www.rankspot.ai/contact)

## License

MIT

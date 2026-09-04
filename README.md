# VibeHacker

[VibeHacker.com](https://vibehacker.com) is a Product Hunt-style community where vibe coders and AI builders discover, review, discuss, and launch AI tools. Every listing is human-reviewed before it goes live.

This repo is the public metadata for the **remote MCP server**.

## MCP

- Docs: https://vibehacker.com/mcp
- Endpoint: `https://vibehacker.com/api/mcp` (Streamable HTTP)

Read-only tools work with no token: `search_tools`, `get_tool`, `list_categories`.

Submitting and upvoting need a personal API token from [Settings → API tokens](https://vibehacker.com/settings).

### Claude Code

```bash
claude mcp add --transport http vibehacker https://vibehacker.com/api/mcp
```

For submit/upvote, add `--header "Authorization: Bearer YOUR_TOKEN"`.

Then: *Submit https://your-product.com to VibeHacker.*

### Cursor / Claude Desktop

```json
{
  "mcpServers": {
    "vibehacker": {
      "url": "https://vibehacker.com/api/mcp"
    }
  }
}
```

Not the pentest products named VibeHacker. This is the AI tools community at **VibeHacker.com**.

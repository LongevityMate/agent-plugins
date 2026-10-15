# LongevityMate plugins

Connect your assistant to the public LongevityMate educational library.

## LongevityMate Library

Search reviewed English guides, read their complete educational text and safety context, and follow their sources. No LongevityMate account or sign-in is needed.

This plugin does not read personal lab results, wearable data or plans, upload documents, change goals, or provide individual diagnosis or treatment. Use general topic phrases, without personal records or identifiers.

## Install in Codex

With a current Codex CLI that supports plugins:

```sh
codex plugin marketplace add LongevityMate/agent-plugins
codex plugin add longevitymate-library@longevitymate
```

Open a new chat after installation. If the desktop app does not show the new source yet, restart it and choose **LongevityMate** in the Plugins directory.

This is a direct marketplace installation. It does not mean the plugin has been reviewed or listed in OpenAI's public directory.

## Connect another MCP client

Use Streamable HTTP with no authentication:

```text
https://longevitymate.com/api/mcp/library
```

The server exposes two read-only tools: `search_library` and `get_library_item`. Client compatibility must be tested in the chosen product; support for MCP alone is not proof of a completed installation.

## Sources and privacy

The plugin returns public source links and publication dates. Preserve relevant cautions and evidence limits when using its results. A new article edition may be temporarily unavailable until its library audience review is complete.

Only public topic queries and article identifiers are needed. Do not send private documents, account details or personal health values. The server does not store tool payloads in an account or log query and result bodies. Hosting providers may process request metadata for operation and security. Your assistant provider's own privacy terms also apply.

[Library](https://longevitymate.com/learn) · [Privacy](https://longevitymate.com/privacy) · [Terms](https://longevitymate.com/terms) · [Support](mailto:hello@longevitymate.com)

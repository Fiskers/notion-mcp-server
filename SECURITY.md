# Security Policy

## Project status

This repository is a fork of the local Notion MCP server. The upstream project prioritizes the remote Notion MCP service and may not actively support this local server. Security reports must identify the affected repository and commit.

## Reporting a vulnerability

Do not disclose vulnerabilities, Notion tokens, MCP configuration, page content, database content, request headers, or logs in public issues or pull requests.

Report issues affecting this fork privately through:

https://github.com/Fiskers/notion-mcp-server/security/advisories/new

If the issue also affects the upstream project, follow Notion's official security reporting process.

Include reproduction steps, the affected commit or package version, impact, and a minimal proof of concept with secrets and personal data removed.

## Credentials and workspace access

Treat `NOTION_TOKEN`, `OPENAPI_MCP_HEADERS`, authorization headers, and MCP client configuration as secrets.

- Never commit real tokens or headers.
- Grant integrations access only to required pages.
- Prefer read-only capabilities when write access is unnecessary.
- Revoke and replace credentials that may have been exposed.
- Review tool calls before allowing an AI client to modify workspace data.

## Supported versions

Only the latest commit on this fork's default branch is considered for reports. No guarantee of production support is provided.

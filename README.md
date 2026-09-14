# ai

Agent Skills, MCP servers and Claude Code plugins.

```
skills/    one directory each - SKILL.md + optional scripts/ references/ assets/
mcp/       one server.json each
plugins/   only when the unit is MORE than a skill
```

## Standards

| Layer | Spec | Validator |
|---|---|---|
| skills | [agentskills.io](https://agentskills.io) | `skills-ref validate ./<skill>` |
| MCP servers | [MCP registry `server.json`](https://github.com/modelcontextprotocol/registry/blob/main/docs/reference/server-json/draft/server.schema.json) | `check-jsonschema` |
| plugins | [Claude Code marketplaces](https://code.claude.com/docs/en/plugin-marketplaces) | `claude plugin validate` |

Add as a marketplace:

```
/plugin marketplace add ismailkattakath/ai
```

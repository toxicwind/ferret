# MCP

[README](../README.md)

ProjectDiscovery does not publish an MCP server. The community surface is [intelligent-ears/pd-tools-mcp](https://github.com/intelligent-ears/pd-tools-mcp). A Docker wrap of that server lives in [FuzzingLabs/mcp-security-hub](https://github.com/FuzzingLabs/mcp-security-hub/tree/master/reconnaissance/pd-tools-mcp). Nuclei alone is wrapped again as `web-security/nuclei-mcp` in that hub.

Those six tools are first-class here. `ferret pull` updates their bins. Ferret does not vendor the MCP server.

| MCP tool | Bin | Job |
|---|---|---|
| subfinder | subfinder | passive subdomains |
| dnsx | dnsx | DNS resolve |
| naabu | naabu | port scan |
| httpx | httpx | HTTP probe |
| katana | katana | crawl |
| nuclei | nuclei | template scan |

Nuclei templates are a second pull: `nuclei -update-templates`. That is not `pdtm -update-all`.

Re-pull the server itself:

```sh
git -C "$HOME/src/pd-tools-mcp" pull --ff-only
```

Clone once from https://github.com/intelligent-ears/pd-tools-mcp if that directory is missing.

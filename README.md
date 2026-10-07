# ferret

The ProjectDiscovery MCP we already wrote. It lived at `toxicwind/estate` `tools/pd-mcp`. This repo is that server.

stdio JSON-RPC, Content-Length framing. `initialize`, `tools/list`, `tools/call`. It wraps the PDTM bins in `PD_TOOLS_DIR` (default `/home/toxic/.pdtm/go/bin`). It runs on yote, where the bins live.

```sh
ferret pull
bun mcp/server.ts
```

`ferret pull` is `pdtm -update-all`. The server is `mcp/`. Docs for the server are `mcp/README.md` and `mcp/AGENTS.md`.

Salvage copies under `estate/salvage/origin-main-20261002/conflicts/tools/pd-mcp` are the old conflict. Do not edit those.

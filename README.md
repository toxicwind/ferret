# ferret

Re-pull surface for [ProjectDiscovery PDTM](https://github.com/projectdiscovery/pdtm). Not a fork of those tools. Not a furry rename of them.

Upstream owns the bins. Ferret's job is to get them again without remembering flags.

## What this is

`pdtm` downloads release binaries into `$HOME/.pdtm/go/bin`. Ferret calls that. `ferret pull` is `pdtm -update-all`. `ferret install` is `pdtm -install-all`. `ferret self` updates pdtm itself.

The den names in older notes were a chat convention. They are not the project.

## Install

```sh
go install github.com/projectdiscovery/pdtm/cmd/pdtm@latest
install -m 755 ferret "$HOME/.local/bin/ferret"
ferret install
```

## Re-pull

```sh
ferret pull
ferret self
```

`PDTM_BIN` overrides the bin directory. `PDTM` overrides the pdtm binary.

## Docs

- [docs/UPSTREAM.md](docs/UPSTREAM.md) — what pull hits, and what it does not
- Upstream usage: https://github.com/projectdiscovery/pdtm
- [docs/MCP.md](docs/MCP.md) — community PD MCP, six first-class tools

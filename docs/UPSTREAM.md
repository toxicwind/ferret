# Upstream

[README](../README.md)

pdtm installs by downloading published release binaries. It does not build the tools. A platform without a published binary cannot be installed. Default path is `$HOME/.pdtm/go/bin`, flag `-bp`.

| ferret | pdtm |
|---|---|
| pull | -update-all |
| install | -install-all |
| install dnsx nuclei | -install dnsx nuclei |
| remove nuclei | -remove nuclei |
| remove all | -remove-all |
| self | -self-update |

Pull updates bins already installed. It does not add tools that were never installed. First run is `ferret install`.

This repo does not vendor httpx, nuclei, dnsx, or the rest. Re-pull them from ProjectDiscovery.

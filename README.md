# ferret

Furry names over [ProjectDiscovery PDTM](https://github.com/projectdiscovery/pdtm) bins. The aliases are obfuscation. The tools are not.

`tman` is `pdtm`. Everything else is a two-line `exec` into `$PDTM_BIN` (default `$HOME/.pdtm/go/bin`). Ferret only dispatches.

## Install

```sh
go install -v github.com/projectdiscovery/pdtm/cmd/pdtm@latest
pdtm -install-all
cp -p bin/* "$HOME/.local/bin/"
chmod +x "$HOME/.local/bin/"/*
```

## Use

```sh
ferret list
ferret dns -silent -a -resp
ferret probe -silent -json
ferret sig -severity high,critical -jsonl
```

Short forms: `probe` `dns` `sub` `sig` `ports` `crawl` `tls` `alt` `db` `asn` `cdn` `cloud` `cidr` `tld` `serve` `notify` `chaos` `prox` `shuffle` `aix`.

## Map

| Den name | Short | PDTM bin |
|---|---|---|
| tman | | pdtm |
| webprobe | probe | httpx |
| dnsprobe | dns | dnsx |
| subprobe | sub | subfinder |
| sigscan | sig | nuclei |
| portprobe | ports | naabu |
| crawlprobe | crawl | katana |
| tlsprobe | tls | tlsx |
| altprobe | alt | alterx |
| dbprobe | db | uncover |
| asnprobe | asn | asnmap |
| cdnprobe | cdn | cdncheck |
| cloudprobe | cloud | cloudlist |
| cidrprobe | cidr | mapcidr |
| tldprobe | tld | tldfinder |
| httpserve | serve | simplehttpserver |
| notify | notify | notify |
| chaos | chaos | chaos |
| proxify | prox | proxify |
| shuffledns | shuffle | shuffledns |
| aix | aix | aix |

Upstream docs: [projectdiscovery.io/open-source](https://projectdiscovery.io/open-source). This repo does not vendor those binaries.

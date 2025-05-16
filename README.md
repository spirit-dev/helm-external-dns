# Welcome to external-dns

[![App Status](https://argocd-internal.spirit-dev.net/api/badge?name=external-dns-turingpi&revision=true&showAppName=true)](https://argocd-internal.spirit-dev.net/applications/external-dns-turingpi)

## Table of content

[[_TOC_]]

## Installation process

The installation is entirely managed by Argocd.

A `Makefile` is present here to ease the first and one-time deployment or in case of an issue.
The installation should be done in two steps:

```shell
#> make dry-run ENV=<ENV>
#> make install ENV=<ENV>
```

## Create OVH credentials

https://kubernetes-sigs.github.io/external-dns/v0.14.0/tutorials/ovh/#creating-a-zone-with-ovh-dns

## Extra resources

the following resources are extracted from DNS providers (OVH and Cloudflare). Files do not intent to be a backup but note that some of its config (mail especially) are critical for the wellness of the solution.

- [DNS zone bordat.me Cloudflare](doc/DNS-zone-CF-bordat.me-ori.txt)
- [DNS zone spirit-dev.net Cloudflare](doc/DNS-zone-CF-spirit-dev.net-ori.txt)
- [DNS zone spirit-dev.net OVH](doc/DNS-zone-OVH-spirit-dev.net-ori.txt)

# external-dns

<!-- More info: https://github.com/Ileriayo/markdown-badges -->
<!-- More info: https://shields.io/badges -->
<!-- More info: https://badgesgenerator.com/ -->

[![GitLab Sync](https://img.shields.io/badge/gitlab_sync-external_dns-blue?style=for-the-badge&logo=gitlab)](https://gitlab-internal.spirit-dev.net/github-mirror/helm-external-dns) <!-- markdownlint-disable MD041 -->
[![GitHub Mirror](https://img.shields.io/badge/github_mirror-external_dns-blue?style=for-the-badge&logo=github)](https://github.com/spirit-dev/helm-external-dns)
[![App Status](https://argocd-internal.spirit-dev.net/api/badge?name=external-dns-turingpi&revision=true&showAppName=true)](https://argocd-internal.spirit-dev.net/applications/external-dns-turingpi)

<!--TOC-->

- [Installation process](#installation-process)
- [Create OVH credentials](#create-ovh-credentials)
- [Extra resources](#extra-resources)

<!--TOC-->

## Installation process

The installation is entirely managed by Argocd.

A `Makefile` is present here to ease the first and one-time deployment or in case of an issue.
The installation should be done in two steps:

```shell
#> make dry-run ENV=<ENV>
#> make install ENV=<ENV>
```

## Create OVH credentials

[OVH Documentation](https://kubernetes-sigs.github.io/external-dns/v0.14.0/tutorials/ovh/#creating-a-zone-with-ovh-dns)

## Extra resources

the following resources are extracted from DNS providers (OVH and Cloudflare). Files do not intent to be a backup but note that some of its config (mail especially) are critical for the wellness of the solution.

- [DNS zone bordat.me Cloudflare](doc/DNS-zone-CF-bordat.me-ori.txt)
- [DNS zone spirit-dev.net Cloudflare](doc/DNS-zone-CF-spirit-dev.net-ori.txt)
- [DNS zone spirit-dev.net OVH](doc/DNS-zone-OVH-spirit-dev.net-ori.txt)

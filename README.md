# external-dns



<!--TOC-->

- [Installation process](#installation-process)
- [Create OVH credentials](#create-ovh-credentials)

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


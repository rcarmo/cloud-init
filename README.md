# cloud-init

This repository contains useful cloud-init samples that I use for various things.

## Using with `lxc`

```bash
lxc image list images: | grep fedora
lxc profile create <name>
lxc profile set <name> user.user-data="$(< <file>)"
lxc launch images:fedora/35/cloud <container> -p <name>
lxc launch ubuntu:22.04 <container> -p <name>
```
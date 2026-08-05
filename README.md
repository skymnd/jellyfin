# Jellyfin in a homelab

This repo is my personal configuration for using jellyfin
on my homelab.
Jellyfin is a free software media system.
The
[Jellyfin docs](https://jellyfin.org/docs/)
are pretty good and can explain a bit more about what that
means.

## PCI Passthrough

I've configured the VM that is running jellyfin to use
PCI passthrough for the GPU to help with transcoding.
See the [Proxmox docs](https://pve.proxmox.com/wiki/PCI_Passthrough)
and the [Jellyfin docs](https://jellyfin.org/docs/general/post-install/transcoding/hardware-acceleration/intel)
for how to set that up.

## Media Storage

I'm storing the assets on a mounted
NAS drive rather than on the VM.
The drives are mounted in the docker-compose as docker volumes.

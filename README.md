# Pi-Hole + Unbound on Docker + Build on Synology

Synology does not support Dockerfiles in subdirectories. Dockerfile moved, config updated accordingly.

Only for original repos one-container solution:
- [`one-container`](one-container/) (new) - Install Unbound directly into the Pi-Hole container
  - This configuration contacts the DNS root servers directly, please read the Pi-Hole docs on [Pi-hole as All-Around DNS Solution](https://docs.pi-hole.net/guides/unbound/) to understand what this means.
  - With this approach, we can also simplify our Docker networking since `macvlan` is no longer necessary.


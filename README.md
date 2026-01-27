## parzival-space's Pacman Repository
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/parzival-space/pacman-pkgs/build-repository.yaml?branch=development&style=for-the-badge&logo=github)

Repository for various custom packages that I maintain for Arch Linux.

### Repository Installation
Add the following code snippet to your `/etc/pacman.conf` file:

```
[parzival-space]
SigLevel = Optional TrustAll
Server = https://github.com/parzival-space/pacman-pkgs/releases/download/$arch
```

Then, run `sudo pacman -Sy` to update your package database.
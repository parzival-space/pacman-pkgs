## parzival-space's Arch Packages
![Repository Update](https://img.shields.io/github/actions/workflow/status/parzival-space/pacman-pkgs/build-repository.yaml?style=for-the-badge&logo=github&label=Repository%20Update)
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/parzival-space/pacman-pkgs/sync-aur.yaml?style=for-the-badge&logo=archlinux&label=AUR%20Sync&color=blue)


Package sources I maintain or co-maintain for the Arch User Repository (AUR) and some other non-AUR packages.

### Contributing
The package sources in this repository are maintained on a case-by-case basis.
If you find an outdated package, feel free to open an issue or a pull request with the updated PKGBUILD.

### Using the 'parzival-space' Repository
Prebuilt packages, including some packages not published to the AUR, are published to a custom Pacman repository.
The packages are built using GitHub Actions. You can read the workflow file [here](.github/workflows/build-repository.yaml) for more details.

To use the Pacman repository, add the following code snippet to your `/etc/pacman.conf` file:
```
[parzival-space]
SigLevel = Optional TrustAll
Server = https://github.com/parzival-space/pacman-pkgs/releases/download/repository
```
Then, run `sudo pacman -Sy` to update your package database.


# Yolks

A curated collection of core images that can be used with Pterodactyl's Egg system. Each image is rebuilt
periodically to ensure dependencies are always up-to-date.

Images are hosted on `ghcr.io` and exist under the `games`, `installers`, and `yolks` spaces. The following logic
is used when determining which space an image will live under:

* `oses` — base images containing core packages to get you started.
* `installers` — anything living within the `installers` directory. These images are used by install scripts for different
Eggs within Pterodactyl, not for actually running a game server. These images are only designed to reduce installation time
and network usage by pre-installing common installation dependencies such as `curl` and `wget`.
* `yolks` — these are more generic images that allow different types of games or scripts to run. They're generally just
a specific version of software and allow different Eggs within Pterodactyl to switch out the underlying implementation. An
example of this would be something like Java or Python which are used for running bots, Minecraft servers, etc.

## Available Images

* [`base oses`](hhttps://github.com/Cr0iX/yolks/tree/main/oses)
  * [`ubuntu23`](https://github.com/Cr0iX/yolks/tree/main/oses/ubuntu23)
    * `ghcr.io/cr0ix/yolks:ubuntu23`

## Installation Images

* [`ubuntu23`](https://github.com/Cr0iX/yolks/tree/main/installers/ubuntu23)
  * `ghcr.io/cr0ix/installers:ubuntu23`
<p align="center">
  <a href="https://opensource.org/license/mit"><img src="https://img.shields.io/badge/License-MIT-blue.svg?color=3F51B5&style=for-the-badge&label=License&logoColor=000000&labelColor=ececec" alt="License: GPLv3"></a>
</p>

<p align="center">
    <img src="https://raw.githubusercontent.com/onloc-app/onloc-ui/refs/heads/main/public/favicon.svg" height="120"/>
</p>

## Description

Onloc is a service that allows you to track and locate your devices. This repository contains files and instructions to install and setup Onloc.

> [!NOTE]
> You can find the other repositories here:
>
> - Front-end: https://github.com/onloc-app/onloc-ui
> - Back-end: https://github.com/onloc-app/onloc-api
> - Android: https://github.com/onloc-app/onloc-android

## Installation

> [!NOTE]
> **Docker** or **Podman** is **required** to install this project. They are currently the only install methods.

1. Create a new directory.

```
mkdir ./onloc-app
cd ./onloc-app
```

2. Install the necessary files from the latest release.

```
curl -L -O https://github.com/onloc-app/onloc-deployment/releases/latest/download/docker-compose.yml
curl -L -O https://github.com/onloc-app/onloc-deployment/releases/latest/download/Caddyfile
```

3. Start the containers.

Docker:
```
docker compose pull && docker compose up -d
```

Podman:
```
podman compose pull && podman compose up -d
```

Onloc is now running on port **6144**.

## Update

Docker:
```
docker compose pull && docker compose up -d
```

Podman:
```
podman compose pull && podman compose up -d
```

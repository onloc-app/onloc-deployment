<p align="center">
  <a href="https://opensource.org/license/gpl-3-0"><img src="https://img.shields.io/badge/License-GPL_v3-blue.svg?color=3F51B5&style=for-the-badge&label=License&logoColor=000000&labelColor=ececec" alt="License: GPLv3"></a>
</p>

<p align="center">
    <img src="https://raw.githubusercontent.com/Onloc-Code/onloc-ui/refs/heads/main/public/favicon.svg" height="120"/>
</p>

## Disclaimer
> [!WARNING]
> - The project is under **active** development.
> - Expect bugs and breaking changes.
> - **Do not use the app as the only way to locate your devices.**

## Description
Onloc is a service that allows you to track and locate your devices. This repository contains files and instructions to install and setup Onloc.

> [!NOTE]
> You can find the other repositories here:
> - Front-end: https://github.com/Onloc-Code/onloc-ui
> - Back-end: https://github.com/Onloc-Code/onloc-api
> - Android: https://github.com/Onloc-Code/onloc-android

## Installation
> [!NOTE]
> **Docker** is **required** to install this project. It is currently the only install method.

1. Create a new directory.
```
mkdir ./onloc-app
cd ./onloc-app
```

2. Install the necessary files from the latest release.
```
wget -O docker-compose.yml https://github.com/Onloc-Code/onloc-deployment/releases/latest/download/docker-compose.yml
wget -O nginx.conf https://github.com/Onloc-Code/onloc-deployment/releases/latest/download/nginx.conf
```

3. Start the containers.
```
docker compose pull && docker compose up -d
```

Onloc is now running on port **6144**.

## Update
```
docker compose pull && docker compose up -d
```

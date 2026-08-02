[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-blue?style=flat)](./LICENSE)
![Development: Prototyping](https://img.shields.io/badge/Development-Prototyping-orange?style=flat)
![Version](https://img.shields.io/badge/dynamic/json?label=Version&color=yellow&style=flat&url=https%3A%2F%2Fraw.githubusercontent.com%2Ftschebbischeff%2Fhabitat-den%2Frefs%2Fheads%2Fmain%2Fmetadata.json&query=%24.version)

# Habitat: Den

> [!CAUTION]
> **🚧 This project is currently under heavy development, any information may be subject to change. 🚧**

Habitat provides modular functionality for deployment on home lab devices. \
Each of the modules is designed as an opinionated docker stack that can be deployed on its own or together with other modules by sharing the same docker network.

You can check out all officially available modules [here](https://github.com/Tschebbischeff/habitat#officially-available-modules).

## Our Principles

![TODO](https://img.shields.io/badge/TODO-Coming_Soon_(TM)-red?style=flat)

## Module Features

[![RomM](https://img.shields.io/badge/RomM-_?style=flat&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbDpzcGFjZT0icHJlc2VydmUiIHdpZHRoPSIxMDI0IiBoZWlnaHQ9IjEwMjQiIHZpZXdCb3g9IjAgMCAyNzAuOTMzIDI3MC45MzMiPgogICAgPGRlZnM+CiAgICAgICAgPGNsaXBQYXRoIGlkPSJhIiBjbGlwUGF0aFVuaXRzPSJ1c2VyU3BhY2VPblVzZSI+CiAgICAgICAgICAgIDxlbGxpcHNlIGN4PSI1MTEuODc1IiBjeT0iNTEyLjU1MSIgcng9IjI1NS45NDYiIHJ5PSIyNTUuOTg0IiBzdHlsZT0iZmlsbDpub25lIi8+CiAgICAgICAgPC9jbGlwUGF0aD4KICAgICAgICA8Y2xpcFBhdGggaWQ9ImIiIGNsaXBQYXRoVW5pdHM9InVzZXJTcGFjZU9uVXNlIj4KICAgICAgICAgICAgPGVsbGlwc2UgY3g9IjEzNS40NTciIGN5PSIxMzUuNDcxIiByeD0iMTM1LjQzNiIgcnk9IjEzNS40NTYiIHN0eWxlPSJmaWxsOm5vbmUiLz4KICAgICAgICA8L2NsaXBQYXRoPgogICAgICAgIDxjbGlwUGF0aCBpZD0iYyIgY2xpcFBhdGhVbml0cz0idXNlclNwYWNlT25Vc2UiPgogICAgICAgICAgICA8ZWxsaXBzZSBjeD0iNTExLjg3NSIgY3k9IjUxMi41NTEiIHJ4PSIyNTUuOTQ2IiByeT0iMjU1Ljk4NCIgc3R5bGU9ImZpbGw6bm9uZSIvPgogICAgICAgIDwvY2xpcFBhdGg+CiAgICA8L2RlZnM+CiAgICA8cGF0aCBkPSJNMjU1LjkyOCAyNTYuNTY0SDc2Ny44MlY3NjguNTRIMjU1LjkyOFoiIGNsYXNzPSJiYWNrZ3JvdW5kLWxpZ2h0IiBjbGlwLXBhdGg9InVybCgjYSkiIHN0eWxlPSJmaWxsOiNlZGU1Zjg7ZmlsbC1vcGFjaXR5OjE7c3Ryb2tlLXdpZHRoOjAiIHRyYW5zZm9ybT0idHJhbnNsYXRlKC0xMzUuNDA3IC0xMzUuNzUpc2NhbGUoLjUyOTE2KSIvPgogICAgPHBhdGggZD0ibTcxNC4zNjYgMjU2LjU2NC00NTguNDQgNDU4LjQ0djUzLjUzNkg3NjcuODJWMjU2LjU2NFoiIGNsYXNzPSJiYWNrZ3JvdW5kLWRhcmsiIGNsaXAtcGF0aD0idXJsKCNhKSIgc3R5bGU9ImZpbGw6I2JlYTRlMTtmaWxsLW9wYWNpdHk6MTtzdHJva2Utd2lkdGg6MCIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoLTEzNS40MDcgLTEzNS43NSlzY2FsZSguNTI5MTYpIi8+CiAgICA8ZyBjbGlwLXBhdGg9InVybCgjYikiIHN0eWxlPSJkaXNwbGF5OmlubGluZSI+CiAgICAgICAgPHBhdGggZD0iTTYwMS45MSA3NjguNTRjLTIuNzM1LS4wNjYtNDMuMzctNDcuNzE3LTgzLjczNi03OS4yNjEtMi43ODQtMi4xNzYtNi42NS01LjItOC41OTMtNi43MjEtMy44ODYtMy4wNDUtMTAuNzg0LTcuMDYtMTEuNDc5LTcuNDYxLTEuMTktLjY4Ny0yLjM5My0xLjI3Mi02LjY2NS0zLjE1LTQuNTI0LTEuOTktMTMuNTY3LTQuNTQyLTE4Ljc3Mi01LjI5OC04LjQ5OC0xLjIzNi0zMy44NC0xLjYzOS05Ni4yNTEtMS41ODJsLTEyMC40ODYuMTFjLS4wMTYtODIuMTg0LS4wMS0yMzYuMDM2LS4wMTMtMzA1LjEwOGw4OC44MzEuMjMyYzM5LjAyOS4xMDEgNDAuODQ3LS4xODkgNDcuMTQ0LTMuMDA4IDEzLjQ0My02LjAxOSA2OC45MDYtNzYuNTMgODMuMTE0LTgyLjk3MyA3LjI1NC0zLjI5IDE2LjYwMy00LjcwMiAyMy45MTgtMy4yMDIgMS41ODEuMzI0IDYuNjI2IDEuMTU3IDExLjIxMiAxLjg1MiAxMC44OTUgMS42NSAxOC4yMTggMi43NTQgMzUuNDM0IDcuMzc2IDI4LjY3NiA3LjY5NyA1Ni42MzggMTkuMzg2IDU4LjY2IDIwLjMxIDExLjkzNyA1LjQ1MyAyNS40MTEgMTIuNDcyIDI5LjQzIDE2LjI3MSAxLjU5IDEuNTA0IDMuMjgyIDMuNTQyIDQuMDgzIDQuODUyIDMuNTI0IDUuNzY1IDExLjAzNCAxOS44NDUgMTEuNzU2IDIyLjMzMyA5LjE3NSAyMi4wMDcgMTcuMzU2IDQ0LjM4MSAyNS43MzMgNjYuNyAzLjk3OSAxMS40MTUgOC4zMzYgMjIuNTcgMTIuMjc2IDMzLjk0NSAzLjM1OCA5Ljc4NSAxMC42MTQgMzAuMTI4IDExLjA0NSAzMC45NjggNS42MDQgMTUuNzE3IDEwLjQxOSAzMS42NTUgMTUuMjA0IDQ3LjY0MyAyLjk4OSA5LjkzIDYuNjc0IDIyLjg2MiAxMC4yNTMgMzYuNjI2IDUuMzkgMTguMTE4IDEwLjkwOSAzNi4yMDUgMTQuMjI2IDU0Ljg4OS43MTggMy45NiAzLjI2NCAxOS44MDIgMy40NDUgMjEuMDUzLjQzNyAzLjAyNiAzLjI3NyAyNS44NjcgMy44NTEgMzEuMDczIDIuNjI2IDIzLjgxIDIuMTUgNjguNTQ1LTE3LjY3OCAxMDEuNTQtLjEuMTY3LTIuNjUuMDMxLTIuNzA3LjAzMi05LjA0Mi4wNjUtMzEuOTA3LS4wMy0zOS42NjQtLjA0My0xNS45NC0uMDI5LTgzLjUwMS4wMDUtODMuNTA4LjAwNXoiIGNsYXNzPSJsb2dvLXNlY29uZGFyeSIgc3R5bGU9ImZpbGw6IzM3MWY2OTtmaWxsLW9wYWNpdHk6MTtzdHJva2Utd2lkdGg6MDtzdHJva2UtZGFzaGFycmF5Om5vbmUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKC0xMzUuNDA3IC0xMzUuNzUpc2NhbGUoLjUyOTE2KSIvPgogICAgICAgIDxwYXRoIGQ9Ik0xMTUuODk0IDkuMjU2Yy03IDMuMTczLTM3LjQxNSA0MS4xOC00My45OTIgNDQuMTI1LTMuMzMxIDEuNDkyLTQuMjk0IDEuNjQ1LTI0Ljk0NyAxLjU5MWwtNDYuOTQtLjE4OWMwIDM2LjU1LS4wMDIgMTE3Ljk2My4wMDYgMTYxLjQ1bDI2LjQ1Ni0uMDIzTDIwNC4yNiAzOC4zNmMtLjc1LTEuMzg3LTEuODQtMy4wOTUtMi4zODgtMy45OS0uNDI0LS42OTQtMS4xOC0xLjYzMy0yLjAyMS0yLjQyOC0yLjEyNi0yLjAxLTkuMjU2LTUuNzI1LTE1LjU3My04LjYxLTEwLjE0NC00LjYzMy0yMC4yMDQtNy42OC0zMS4wNDEtMTAuNzQ4LTkuMTEtMi40NDYtMTcuMjQ5LTMuNjI2LTE4Ljc1Mi0zLjkwMy0yLjQxMy0uNDQ0LTUuMDMxLS44NC01LjkzMi0uOTgtLjY0MS0uMDk4LTYuNTI1LTEuMjI1LTEyLjY1OCAxLjU1NVoiIGNsYXNzPSJsb2dvLXByaW1hcnkiIHN0eWxlPSJmaWxsOiM1NTNlOTg7ZmlsbC1vcGFjaXR5OjE7c3Ryb2tlLXdpZHRoOjAiLz4KICAgIDwvZz4KICAgIDxnIGNsaXAtcGF0aD0idXJsKCNjKSIgc3R5bGU9ImRpc3BsYXk6aW5saW5lIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTM1LjQwNyAtMTM1Ljc1KXNjYWxlKC41MjkxNikiPgogICAgICAgIDxjaXJjbGUgY3g9IjUzMC41MzIiIGN5PSIzODEuODE3IiByPSIzMS41MjkiIGNsYXNzPSJkb3QtbGlnaHQiIHN0eWxlPSJmaWxsOiNlNmM3YTc7ZmlsbC1vcGFjaXR5OjE7c3Ryb2tlLXdpZHRoOjA7c3Ryb2tlLWxpbmVqb2luOmJldmVsO3N0cm9rZS1kYXNoYXJyYXk6bm9uZSIvPgogICAgICAgIDxjaXJjbGUgY3g9IjQ3MS41NjUiIGN5PSI0NDAuMzQ4IiByPSIzMS41MjkiIGNsYXNzPSJkb3QtbGlnaHQiIHN0eWxlPSJmaWxsOiNlNmM3YTc7ZmlsbC1vcGFjaXR5OjE7c3Ryb2tlLXdpZHRoOjA7c3Ryb2tlLWxpbmVqb2luOmJldmVsO3N0cm9rZS1kYXNoYXJyYXk6bm9uZSIvPgogICAgICAgIDxjaXJjbGUgY3g9IjU5MC42MDEiIGN5PSI0MzkuMjUyIiByPSIzMS41MjkiIGNsYXNzPSJkb3QtZGFyayIgc3R5bGU9ImZpbGw6I2UxYTM4ZDtmaWxsLW9wYWNpdHk6MTtzdHJva2Utd2lkdGg6MDtzdHJva2UtbGluZWpvaW46YmV2ZWw7c3Ryb2tlLWRhc2hhcnJheTpub25lIi8+CiAgICAgICAgPGNpcmNsZSBjeD0iNTMwLjQ0MSIgY3k9IjQ5OS45NDgiIHI9IjMxLjUyOSIgY2xhc3M9ImRvdC1kYXJrIiBzdHlsZT0iZmlsbDojZTFhMzhkO2ZpbGwtb3BhY2l0eToxO3N0cm9rZS13aWR0aDowO3N0cm9rZS1saW5lam9pbjpiZXZlbDtzdHJva2UtZGFzaGFycmF5Om5vbmUiLz4KICAgIDwvZz4KPC9zdmc+&logoColor=000000&color=gray&labelColor=gray)](https://romm.app/)

 - **Retro console ROM Manager** \
 Provides RomM as a platform to manage ROMs for retro consoles in a library.

### Planned

![No Features Planned](https://img.shields.io/badge/_-No_Planned_Features-green?style=flat)

## Getting Started

### Requirements

 - [![Habitat-Module: Path](https://img.shields.io/badge/Habitat--Module-Path-_?style=flat&color=gray&labelColor=gray)](https://github.com/Tschebbischeff/habitat-path)
 - [![Habitat-Module: Scent](https://img.shields.io/badge/Habitat--Module-Scent-_?style=flat&color=gray&labelColor=gray)](https://github.com/Tschebbischeff/habitat-scent)

### Configuration

> [!IMPORTANT]
> All habitat modules are designed to be controlled exclusively with environment variables and secrets. \
> Refer to the configuration section of each module for an overview of how to configure it. \
> **This section describes how to configure the module without the help of the [Habitat Deployment Service](https://github.com/Tschebbischeff/habitat). \
> It is highly recommended to use the deployment service for ease of use and skip to the lists of environment variables and secrets for this module.**

 - [List of environment variables](#environment-variables)
 - [List of secrets](#secrets)

#### Shell Exports

The existing [.env](./.env) file contains sane defaults for most necessary environment variables and is designed to let you overwrite any of those environment variables via exports from your shell before running the application.

*Example:*
```sh
export APP_HOST="my-habitat.example.com"
export APP_MODULES="path,scent,vista,chatter,hoard,vigil,sight,stash"
export APP_SESSION_ID="$(cat /proc/sys/kernel/random/uuid)"
export APP_NAME_LABEL="MyHabitat"
export TIMEZONE="Europe/London"
export SECRETS_DIR="/run/secrets"
docker compose up
```

#### Repository _.env File

You can also create the file `_.env` in the root directory of the cloned repository and instruct docker compose to use this file instead via the `--env-file` argument, i.e `docker compose --env-file "./_.env" up` ([Compose documentation](https://docs.docker.com/compose/how-tos/environment-variables/variable-interpolation/)).

> [!TIP]
> The file `_.env` is included in [.gitignore](./.gitignore) and is guaranteed to not interfere with future updates via `git pull`.

> [!IMPORTANT]
> *If this method is used you need to define **all** necessary environment variables from the [.env](./.env) file, as docker compose will not use that file as a fallback, it is therefore recommended to copy the current `.env` file and replace all variable values.*

*Example:* [See .env](./.env)

#### Local .env File

It is also possible to create a `.env` file in an unrelated directory ([Compose documentation](https://docs.docker.com/compose/how-tos/environment-variables/variable-interpolation/#local-env-file-versus-project-directory-env-file)).

> [!NOTE]
> In this case you need to set the additional variable `COMPOSE_FILE` to the path of the repository's compose file and all variables inside the [.env](./.env) file will be loaded as fallback, if your own `.env` file does not define them.

> [!NOTE]
> You do not need to instruct docker compose to use this file as long as you run `docker compose up` from the directory containing your `.env` file.

*Example:*
```sh
# /path/to/your/.env
COMPOSE_FILE="/path/to/repository/compose.yml"
APP_HOST="my-habitat.example.com"
APP_MODULES="path,scent,vista,chatter,hoard,vigil,sight,stash"
APP_SESSION_ID="$(cat /proc/sys/kernel/random/uuid)"
APP_NAME_LABEL="MyHabitat"
TIMEZONE="Europe/Madrid"
SECRETS_DIR="/run/secrets"
```

### Environment Variables

> [!TIP]
> Some environment variables are used commonly throughout all modules, you can check the list [here](https://github.com/Tschebbischeff/habitat#environment-variables-for-modules).

*This module does not require any additional environment variables.*

### Secrets

*This module does not require any secrets.*

<!--
> [!NOTE]
> All secrets are expected to be files within a single folder, each file containing the value of the secret. \
> This folder can be set via environment variable (`SECRETS_DIR`) itself and defaults to `./.secrets` (git-ignored folder). \
> All secrets must be present at run-time.

| (File) Name | Description | Documentation / How to Obtain |
| :-- | :-- | :-- |
|  | This module does not require any secrets |  |
-->

### Run the Application

 - Run `docker compose up` from the root directory of the repository or from the directory containing your `.env` file
 - Run `docker compose logs` and wait for the application to finish first-time setup and settle

## Acknowledgments and Licensing

This project is licensed under the [GNU Affero General Public License v3.0 (AGPL-3.0)](./LICENSE).

Copyright (c) 2026, [Tschebbischeff](https://github.com/Tschebbischeff). \
All rights reserved to the extent permitted by the AGPLv3.

For third-party license details and attribution, please see [Third-Party Licenses](./THIRD-PARTY-LICENSES.md).

With Icons from:
[![SimpleIcons](https://img.shields.io/badge/SimpleIcons-_?style=flat&logo=simpleicons&logoColor=111111&color=gray&labelColor=gray)](https://simpleicons.org/)
[![DashboardIcons](https://img.shields.io/badge/DashboardIcons-_?style=flat&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSI1MTIiIGhlaWdodD0iNTEyIiB2aWV3Qm94PSIwIDAgMjMyIDIzMiIgcm9sZT0iaW1nIiBhcmlhLWxhYmVsPSJkYXNoYm9hcmQtaWNvbnMgbG9nbyI+DQogIDxyZWN0IHg9IjQiIHk9IjQiIHdpZHRoPSIyMjQiIGhlaWdodD0iMjI0IiByeD0iMzIiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzAwMCIgc3Ryb2tlLXdpZHRoPSI4IiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiLz4NCiAgPGcgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjY2NjIiBzdHJva2Utd2lkdGg9IjQiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCI+DQogICAgPHJlY3QgeD0iMjQiIHk9IjI0IiB3aWR0aD0iNDgiIGhlaWdodD0iNDgiIHJ4PSI4IiBzdHJva2U9IiNGQjcxODUiLz4NCiAgICA8cmVjdCB4PSI5MiIgeT0iMjQiIHdpZHRoPSI0OCIgaGVpZ2h0PSI0OCIgcng9IjgiIGZpbGw9IiNGREJBNzQiLz4NCiAgICA8cmVjdCB4PSI5MiIgeT0iOTIiIHdpZHRoPSI0OCIgaGVpZ2h0PSI0OCIgcng9IjgiIHN0cm9rZT0iI0M0QjVGRCIvPg0KICAgIDxyZWN0IHg9IjE2MCIgeT0iOTIiIHdpZHRoPSI0OCIgaGVpZ2h0PSI0OCIgcng9IjgiLz4NCiAgICA8cmVjdCB4PSI5MiIgeT0iMTYwIiB3aWR0aD0iNDgiIGhlaWdodD0iNDgiIHJ4PSI4Ii8+DQogICAgPHJlY3QgeD0iMTYwIiB5PSIxNjAiIHdpZHRoPSI0OCIgaGVpZ2h0PSI0OCIgcng9IjgiIGZpbGw9IiM5M0M1RkQiLz4NCiAgPC9nPg0KICA8Y2lyY2xlIGN4PSIxODQiIGN5PSI0OCIgcj0iMjYiIGZpbGw9IiM4NkVGQUMiLz4NCiAgPGNpcmNsZSBjeD0iNDgiIGN5PSIxMTYiIHI9IjI2IiBmaWxsPSIjOTNDNUZEIi8+DQogIDxyZWN0IHg9IjI0IiB5PSIxNjAiIHdpZHRoPSI0OCIgaGVpZ2h0PSI0OCIgcng9IjgiIGZpbGw9IiNGREU2OEEiLz4NCjwvc3ZnPg==&logoColor=F56565&color=gray&labelColor=gray)](https://dashboardicons.com/)
[![Lucide](https://img.shields.io/badge/Lucide-_?style=flat&logo=lucide&logoColor=F56565&color=gray&labelColor=gray)](https://lucide.dev/)
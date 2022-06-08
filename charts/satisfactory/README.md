![version: 0.1.2](https://img.shields.io/badge/version-0.1.2-informational?style=flat-square) ![type: application](https://img.shields.io/badge/type-application-informational?style=flat-square) ![app version: v1.2.4](https://img.shields.io/badge/app%20version-v1.2.4-informational?style=flat-square) [![artifact hub](https://img.shields.io/badge/artifact%20hub-satisfactory-informational?style=flat-square)](https://artifacthub.io/packages/helm/jess-v-helm-charts/satisfactory)

# satisfactory
 Helm chart for deploying a Satisfactory server in Kubernetes. This chart can be installed without modification to deploy a Satisfactory server using the defaults specified in the [wolveix/satisfactory-server](https://hub.docker.com/r/wolveix/satisfactory-server) image.

# Installation

```sh
helm repo add jess-v https://jess-v.github.io/helm-charts
helm install satisfactory jess-v/satisfactory
```

# Parameters

| Parameter               |  Default  | Function                                            |
| ----------------------- | :-------: | --------------------------------------------------- |
| `autopause`             |   `true`  | pause game when no player is connected              |
| `autosaveInterval`      |   `300`   | autosave interval in seconds                        |
| `autosaveNum`           |    `3`    | number of rotating autosave files                   |
| `autosaveOnDisconnect`  |   `true`  | autosave when last player disconnects               |
| `crashReport`           |   `true`  | automatic crash reporting                           |
| `debug`                 |  `false`  | for debugging the server                            |
| `disableSeasonalEvents` |  `false`  | disable the FICSMAS event (you miserable bastard)   |
| `maxPlayers`            |    `4`    | set the player limit for your server                |
| `pgid`                  |   `1000`  | set the group ID of the user the server will run as |
| `puid`                  |   `1000`  | set the user ID of the user the server will run as  |
| `serverBeaconPort`      |  `15000`  | set the game's beacon port                          |
| `serverGamePort`        |   `7777`  | set the game's port                                 |
| `serverIP`              | `0.0.0.0` | set the game's ip (usually not needed)              |
| `serverQueryPort`       |  `15777`  | set the game's query port                           |
| `skupUpdate`            |  `false`  | avoid updating the game on container start/restart  |
| `steamBeta`             |  `false`  | set experimental game version                       |

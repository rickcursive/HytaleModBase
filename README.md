# Hytale Mod Base

## Get Started

### Prepare The Code

Forking allows to backport improvements of the setup over time. It is also possible to just download
a zip file of the repository or just clone this repository (not recommended).

- Fork this repository and give it a name, we will refer to it as `<plugin-name>`
- Set the name to `<plugin-name>` in [`settings.gradle.kts`](./settings.gradle.kts)
- Set the name in [`build.gradle.kts`](./build.gradle.kts), we will refer to it as `<group-name>`
- Verify that the server version in `build.gradle.kts` matches the one of your client
- Create a new package in `src/main/java` named `<group-name>`

### Set Up The Dev Server

- Create a new folder `run`
- Download the [`hytale-downloader.zip`](https://downloader.hytale.com/hytale-downloader.zip) from the [Hytale Server Manual](https://support.hytale.com/hc/en-us/articles/45326769420827-Hytale-Server-Manual)
- Extract the `hytale-downloader-<os>-<arch>` binary into the run folder
- Run
    ```bash
    cd run
    ./hytale-downloader-<os>-<arch>
    ```
- Follow the login URL displayed
- Extract from the Downloaded zip file `Assets.zip`, `HytaleServer.jar`, and `HytaleServer.aot` into `run/`
- Create a new Run/Debug Configuration
- Choose `JAR Application`
    - Name it `Hytale Server`
    - Path to JAR: `<path-to-your-fork>/run/HytaleServer.jar`
    - Program arguments: `--assets Assets.zip`
    - Working directory: `<path-to-your-fork>/run`

## Thank You

- Hytale Modding: https://www.youtube.com/watch?v=qeAy5Mhgo90
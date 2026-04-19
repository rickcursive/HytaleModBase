# Hytale Mod Base

## Get Started

### Prepare The Code

#### Recommended method:
- Fork this repository and give it a name, we will refer to it as `<plugin-name>`
- Use the GitHub template to create a new repository, we will refer to it as `<plugin-name>`

#### Set the variables
- Set the name to `<plugin-name>` in [`settings.gradle.kts`](./settings.gradle.kts)
- Set the name in [`build.gradle.kts`](./build.gradle.kts), we will refer to it as `<group-name>`
- Verify that the server version in `build.gradle.kts` matches the one of your client
- Create a new package in `src/main/java` named `<group-name>`

#### Alternative methods:
- Download zip file
- Clone this repository (not recommended)

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
# Prismatic Pact — friend builds

Builds of Prismatic Pact for friends. This repo only holds the downloads; the game's source is private.

## Play

1. Download **[PrismaticPactLauncher.exe](https://github.com/Patrick5078/PrismaticPact-releases/releases/download/launcher/PrismaticPactLauncher.exe)** and run it.
   Windows may say it's from an unknown publisher: choose **More info → Run anyway**.
2. Press **Install** (about 1.5 GB), then **Play**.
3. In the game, choose **Play → Custom lobby** and **Connect**. The launcher has already filled in your host's server address.

Open the launcher each time you play. It updates the game when there's a new build, and it shows whether the server is online and on the same version as you.

The game installs to `%LOCALAPPDATA%\PrismaticPact\Game`. Only the newest build is kept.

## For the host

- `BuildRelease.ps1 -Publish` builds the game and uploads it here as the newest release.
- `HostFriends.ps1` starts the server and a Cloudflare tunnel, each in its own window, and publishes the address to `server.json`, where the launcher picks it up.
- `PublishLauncher.ps1` exports the launcher and replaces it on the `launcher` release.

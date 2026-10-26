# Prismatic Pact — friend builds

Builds of Prismatic Pact for friends. This repo only holds the downloads; the game's source is private.

## Play

1. Download **[PrismaticPactLauncher.exe](https://github.com/Patrick5078/PrismaticPact-releases/releases/download/launcher/PrismaticPactLauncher.exe)** and run it.
   Windows may say it's from an unknown publisher: choose **More info → Run anyway**.
2. Press **Install** (about 0.8 GB).
3. Paste the server address your host sends you into the launcher (**Paste**), then press **Play**.
4. In the game, choose **Play → Custom lobby** and **Connect**. The server is already set from the launcher.

Open the launcher each time you play. It updates the game when there's a new patch, shows the patch notes, and tells you whether the server is online and on the same patch as you. Your host's address changes each time they host, so paste the new one when they send it.

The game installs to `%LOCALAPPDATA%\PrismaticPact\Game`. Only the newest patch is kept.

## For the host

- `BuildRelease.ps1 -Publish -NotesFile notes.md` builds the game and uploads it here as the newest release, with its patch notes.
- `HostFriends.ps1` starts the server and a Cloudflare tunnel, each in its own window, and copies the address to your clipboard. Send it to your friends privately; it is never published here.
- `PublishLauncher.ps1` exports the launcher and replaces it on the `launcher` release.

# Stolen Sun

Playable builds of Stolen Sun, a single-player card game: choose an adventurer and take their
deck into a kingdom. The game itself is developed in a private repository; this one exists so
there is a place to download it. Each entry on the
[Releases page](https://github.com/DMod-dev/StolenSun-Releases/releases) is one version with a
macOS and a Windows download.

## macOS

1. Download `StolenSun-<version>-macOS.zip` and unzip it. You get `Stolen Sun.app`; put it in
   *Applications* or leave it where it is.
2. Open it. **The first time, macOS refuses** — *"Stolen Sun" Not Opened. Apple could not verify
   …* — because the build is not notarized (see below). Click *Done*, then open
   *System Settings ▸ Privacy & Security*, scroll down to the line that says *"Stolen Sun" was
   blocked to protect your Mac*, and click **Open Anyway**. Open the app again and confirm.
   This is once per version.

On macOS 15 and later the old right-click ▸ *Open* shortcut no longer works for this; the
Settings route is the only one.

*Why (as of September 2026):* the app is signed but not with an Apple Developer ID and not
notarized, which is what Gatekeeper checks. When a notarized build ships, this section goes away.

## Windows

1. Download `StolenSun-<version>-Windows.zip` and unzip it. You get a `Stolen Sun` folder.
2. Run `Stolen Sun.exe` inside it. Keep the folder together — the `.exe` needs `UnityPlayer.dll`
   and `Stolen Sun_Data` beside it.
3. If SmartScreen shows *Windows protected your PC*, click **More info**, then **Run anyway**.
   The build is not code-signed, which is all that warning means.

## Saves

The game keeps one campaign save, so you can quit and come back to a run:

- macOS: `~/Library/Application Support/DMod/Stolen Sun/`
- Windows: `%USERPROFILE%\AppData\LocalLow\DMod\Stolen Sun\`

Delete that folder to start clean.

## Reporting a problem

Open an issue here with the version (it is in the zip's name), your platform, and what you did
just before it went wrong. A screenshot helps.

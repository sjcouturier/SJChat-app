# SJChat for Windows

Public download host for the **SJChat** Windows desktop client. The app source lives in a
separate private repository; releases are published here via **Velopack** to GitHub Releases.

## Install

**https://sjcouturier.github.io/SJChat-app/**  (Download & Install button)

Or grab the installer directly:

**https://github.com/sjcouturier/SJChat-app/releases/latest/download/SJChat-win-Setup.exe**

The app is self-contained (no .NET install needed) and updates itself automatically after install.
Windows SmartScreen may warn on first run because the app is not code-signed; choose
**More info > Run anyway**.

## How releases are published

The maintainer runs `release.ps1 -Version x.y.z` from the private SJChat repo, which
publishes a self-contained build, packages it with Velopack (`vpk`), and uploads the
installer + update packages to this repo's GitHub Releases.

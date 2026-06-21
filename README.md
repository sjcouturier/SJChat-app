# SJChat for Windows

Public download/installer host for the **SJChat** Windows desktop client.
The application source lives in a separate private repository; this repo only
hosts the compiled ClickOnce installer so it can be downloaded over HTTPS.

## Install

Once a release has been published, install from:

**https://sjcouturier.github.io/SJChat-app/publish.htm**

That page links to `SJChat.application` (the ClickOnce deployment manifest)
and `setup.exe`. The app is self-contained, so no separate .NET runtime
install is required.

## How releases get here

The maintainer publishes the ClickOnce output from Visual Studio
(SJChat.Wpf > Publish > ClickOnceProfile) and pushes the generated files
into this repository's main branch, which GitHub Pages serves.

> .nojekyll is present so GitHub Pages serves the ClickOnce files
> (*.application, *.manifest, *.deploy, ...) without Jekyll processing.

# Sharks · downloads

This repository hosts the releases of **Sharks**, a desktop app that starts your projects in one click, shows every terminal, tracks your hours on its own and gets you into focus.

It only holds the downloads and their release notes. The app's source code is not here.

- **Download:** [latest release](https://github.com/luciaquijada/sharks-releases/releases/latest)
- **Website:** [sharks-app.es/en](https://sharks-app.es/en/)
- **Privacy:** [sharks-app.es/en/privacy](https://sharks-app.es/en/privacy/)
- **Contact:** luciaquijada@sharks-app.es

## Which file do I need?

| Your Mac | File |
| --- | --- |
| Apple silicon (M1 or later) | `Sharks-arm64.dmg` |
| Intel | `Sharks-x64.dmg` |

Requires macOS 13 Ventura or later. A Windows version is coming later.

Not sure which chip you have? Open the Apple menu → About This Mac: it shows either *Chip: Apple M…* or *Processor: … Intel …*.

## Install

1. Open the `.dmg` and drag Sharks to Applications.
2. The first time you open it, macOS asks whether you want to open an app downloaded from the internet. Click **Open**.

Sharks is signed with an Apple Developer ID certificate and notarized by Apple.

## Verify your download

Each release lists the SHA-256 of its files. Compare it in Terminal:

```bash
shasum -a 256 ~/Downloads/Sharks-arm64.dmg
```

To confirm that macOS recognises the app as notarized, after installing it:

```bash
spctl --assess -vv /Applications/Sharks.app
```

The output should end with `source=Notarized Developer ID`.

## Updates

Shortly after it opens, and then once a day, Sharks checks this repository for a newer version and shows a notice when there is one. It sends nothing about you or your Mac: it only reads the public list of releases. You can turn this off, or check by hand, in Settings → About.

## Reporting a problem

Write to luciaquijada@sharks-app.es. For security issues, see [SECURITY.md](SECURITY.md).

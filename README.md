# Trussel IDE

Downloads of the **Trussel IDE**: an editor that reads your whole code base as a graph, lets you design a change
before anyone writes it, and gives your coding agent that graph through its own MCP server.

**[Download the latest version](../../releases/latest)** for macOS (Apple silicon and Intel), Windows and Linux.

This repository holds the installers and the landing page only; the IDE's source is private. Every file is built by
[the workflow in this repository](.github/workflows/build.yml) and published as a release; the newest ten are kept.
The build keeps its output out of the public log, and each successful run's log is deleted when it finishes.

## Installing

| Platform | File | First open |
|---|---|---|
| macOS | `.dmg` (Apple silicon or Intel) | Drag Trussel to Applications, then run `xattr -dr com.apple.quarantine /Applications/Trussel.app` in Terminal once (and again after installing a newer version). Or open it, then System Settings › Privacy & Security › **Open Anyway**. |
| Windows | `.exe` installer, or `.zip` | If SmartScreen stops the installer, choose **More info** › **Run anyway**. |
| Linux | `.deb` (Debian, Ubuntu), `.rpm` (Fedora, RHEL), or `.tar.gz` | `sudo apt install ./Trussel-…-linux-x64.deb`, or `sudo dnf install ./Trussel-…-linux-x64.rpm`. |

The builds are not signed by Apple or Microsoft yet, which is why the first open asks. Each release lists the
SHA-256 of every file in `SHA256SUMS`.

<!-- Mirrored from trussel-frontend's build/trussel/release/releases-repo/ (front-end pass 109): edit it there. -->

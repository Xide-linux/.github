<p align="center">
  <img src="https://raw.githubusercontent.com/Xide-linux/xide-test/main/.github/assets/xide-logo.png" width="130" alt="Xide Logo" />
</p>

<h1 align="center">Xide</h1>

<p align="center">
  An Xcode inspired IDE built for Linux.
</p>

<p align="center">
  <a href="https://github.com/Xide-linux/xide-test/releases">Download</a> ·
  <a href="https://github.com/Xide-linux/xide-test/issues">Report an Issue</a> ·
  <a href="https://xtool.sh">Learn about xtool</a>
</p>

---

## Why Xide?

If you love Xcode's workflow but want to develop iOS apps on Linux, Xide is for you. Open a Swift Package or an existing Xcode or XcodeGen project and build, sign, and run it on your iPhone with ease using [xtool](https://xtool.sh).

## Features

- **Familiar feel** - Navigator, editor tabs and jump bar, inspector, debug area, and toolbar just like Xcode
- **Great Swift editing** - Smart completion, Quick Help, go to definition and references, rename, fix-its, symbol highlighting, folding, minimap, split view, and swift-format
- **Build and run anywhere** - Deploy to your iPhone over USB with `xtool dev`, see errors inline, build unsigned or signed `.ipa` files, archive, or share builds via ntfy
- **Signing simplified** - Sign with your Apple ID through xtool or bring your own certificate and provisioning profile with expiry reminders
- **Tests built in** - Run XCTest and Swift Testing from the Test navigator on your machine
- **On device debugging** - Breakpoints, conditions, and log messages for iOS 17 and up
- **Device tools** - Browse apps, logs, crash reports, take screenshots, or simulate locations
- **Git integration** - View changes, commit, branch, stash, manage remotes, blame, and review diffs
- **Project settings** - Friendly UI for `xtool.yml`, Info.plist, capabilities, packages, build scripts, string catalogs, and asset catalogs
- **Find across your project** - Full project search with regex and replace all
- **Stays in sync** - Picks up changes made outside Xide automatically
- **Optional MCP server** - Let AI agents like Claude Code build, test, run, and manage your project for you

## System Requirements

- **Linux** with glibc (musl isn't supported) and a Vulkan capable GPU (Mesa works well for most)
- **Tools**: `usbmuxd` and `git`. Xide can install them for you via your distro's package manager if they're missing
- **Toolchain**: Swift and xtool are downloaded inside Xide under Settings > Components
- **iOS SDK**: Download `Xcode_27.xip` from Apple, then let Xide set it up

*Tip:* If Swift's sandbox causes issues, launch with `XIDE_NO_SANDBOX=1` and reinstall Swift to use the plain build from swift.org.

## Getting Started

### Build from source

You'll need [Rust 1.88+](https://rustup.rs) and the libraries GPUI needs. Check the [build requirements](https://github.com/Xide-linux/xide-test/blob/main/README.md#requirements) for packages on your distro.

```bash
cargo run --release -- ~/your-ios-project
```

Xide will open that folder or your current directory. Pick your device from the toolbar and hit Run to install and launch your app.

## Get Involved

Found a bug or have an idea? We'd love your help. Open an [issue](https://github.com/Xide-linux/xide-test/issues) or submit a [pull request](https://github.com/Xide-linux/xide-test/pulls).

## License

[See LICENSE](https://github.com/Xide-linux/xide-test/blob/main/LICENSE) for details.

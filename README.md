# LStack Private Beta

This repository provides private beta releases of **LStack** for approved testers.

Learn more at [lstack.ai](https://lstack.ai), or visit the [LStack documentation](https://docs.lstack.ai) for setup and usage guidance.

## Beta access

LStack beta releases are private. Before installing, make sure:

- You have been granted access to this repository.
- [GitHub CLI](https://cli.github.com/) is installed.
- You are signed in by running `gh auth login`.

Your GitHub account must have access to `lstack-ai/beta`.

## Install LStack

```sh
curl -fsSL https://lstack.ai/install.sh | bash
```

The installer uses your authenticated GitHub session to download the correct release for your platform and verifies its SHA-256 checksum before installation.

Supported beta platforms:

- Apple Silicon macOS
- Linux x86-64
- Linux ARM64

## How releases work

LStack uses two types of releases:

- `vX.Y.Z` releases contain the installable artifacts and checksums for a specific version.
- The `stable` release identifies the current recommended beta version.

The installer reads the stable release information, selects the correct artifact for your platform, downloads it from the corresponding versioned release, and verifies it before installation.

GitHub may also display automatically generated “Source code” archives. These are repository snapshots and are not LStack installers. Use the installation command above instead.

Beta releases may change as the product develops. Release notes will describe important changes, compatibility considerations, and any actions required when upgrading.

## Getting started

After installation, follow the [LStack documentation](https://docs.lstack.ai) to complete setup and start using LStack.

If installation fails, confirm that GitHub CLI is authenticated with the account that was granted beta access.

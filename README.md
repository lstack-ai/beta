# LStack Private Beta

This repository provides private beta releases of **LStack** for approved testers.

Learn more at [lstack.ai](https://lstack.ai), or visit the [LStack documentation](https://docs.lstack.ai) for setup and usage guidance.

## Beta access

Before installing, make sure:

- You have been granted access to this repository.
- [GitHub CLI](https://cli.github.com/) is installed.
- You are signed in by running `gh auth login`.

Your GitHub account must have access to `lstack-ai/beta`.

## Install LStack

```sh
curl -fsSL https://lstack.ai/install.sh | bash
```

The installer uses your authenticated GitHub session to select the current stable version, download the correct artifact for your platform, and verify its SHA-256 checksum before installation.

Supported beta platforms:

- Apple Silicon macOS
- Linux x86-64
- Linux ARM64

## Updating LStack

Update to the current stable version:

```sh
lstack update
```

To install a specific available version instead:

```sh
lstack update --version 0.1.1
```

## How releases work

Each `vX.Y.Z` release contains the installable artifacts and checksums for that version.

The repository’s [`stable.json`](stable.json) file identifies the current recommended beta version. The installer and `lstack update` read this file and then download the matching artifact from the corresponding versioned release.

GitHub may also display automatically generated “Source code” archives. These are repository snapshots, not LStack installers. Use the installation command above instead.

See [`CHANGELOG.md`](CHANGELOG.md) for a short summary of changes in each version.

## Getting started

After installation, follow the [LStack documentation](https://docs.lstack.ai) to complete setup and start using LStack.

If installation or updating fails, confirm that GitHub CLI is authenticated with the account that was granted beta access.

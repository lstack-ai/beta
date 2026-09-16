# LStack Beta

This repository provides beta releases of **LStack**.

Learn more at [lstack.ai](https://lstack.ai), or visit the [LStack documentation](https://docs.lstack.ai) for setup and usage guidance.

## Beta access

Downloads are public. You do **not** need a GitHub account, GitHub CLI, or repository invitation to install LStack.

Signing in to LStack is separate from downloading it. Application access still requires an invited LStack beta account.

## Install LStack

```sh
curl -fsSL https://lstack.ai/install.sh | bash
```

The installer selects the current recommended beta version, downloads the correct artifact for your platform over HTTPS, and verifies its SHA-256 checksum before installation. No GitHub authentication is required.

Supported beta platforms:

- Apple Silicon macOS
- Linux x86-64
- Linux ARM64

Docker is not required to install LStack or use the dashboard. It is required when you want to use workers or container-based project runtimes.

## Updating LStack

Update to the current recommended beta version:

```sh
lstack update
```

To install a specific available version, replace `X.Y.Z` with its version number:

```sh
lstack update --version X.Y.Z
```

## How releases work

Each `vX.Y.Z` release contains the installable artifacts and checksums for that version.

The repository’s [stable.json](stable.json) file identifies the current recommended beta version. The installer and ordinary `lstack update` command use this file to select the matching versioned release. An explicit-version update selects the version you requested.

GitHub may also display automatically generated “Source code” archives. These are repository snapshots, not LStack installers. Use the installation command above instead.

See [CHANGELOG.md](CHANGELOG.md) for a short summary of changes in each version.

## Getting started

After installation, start LStack:

```sh
lstack start
```

Follow the [LStack documentation](https://docs.lstack.ai) to complete setup and sign in with your LStack beta account.

If installation or updating fails, follow the reported error and consult the installation documentation. GitHub CLI and `gh auth login` are not prerequisites for the current installer or updater.

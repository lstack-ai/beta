# Changelog

## 0.1.3

- Fixed release downloads for both `lstack update` and version-specific updates.
- Fixed rejected tickets being merged or marked complete by an earlier approval.
- Fixed verification checks being lost when workers create or update verification tickets.
- Added safe worker and unused worker-image cleanup during uninstall, while keeping project runtimes running.

## 0.1.2

- Added password reset directly from the sign-in page.
- Improved Linux onboarding with clearer worker-confinement guidance and readiness checks.
- Added persistent PATH setup instructions after installation.
- Improved installer errors when stable release information cannot be read.
- Cleaned up readiness messaging during initial setup.

## 0.1.1

- Improved Docker detection and worker setup across supported platforms.
- Added the ability to build the worker image during initial setup, before signing in.
- Updated installation and CLI updates to use the repository's `stable.json` release selection.
- Fixed session restart and resume failures caused by invalid session identifiers.

## 0.1.0

Initial LStack private beta release.

- Added support for Apple Silicon macOS, Linux x86-64, and Linux ARM64.
- Added authenticated installation through the private beta repository.
- Added SHA-256 verification for all release artifacts.
- Added the stable release channel for managed installation and updates.

# Changelog

## 0.2.1

- Removed GitHub CLI and GitHub sign-in requirements from installation and updates, and simplified installation guidance.
- Fixed LAN port changes leaving the browser on a forbidden error instead of returning to sign-in.
- Made project lists, counts, and board project filters refresh automatically across open windows and devices.
- Added provider readiness checks that verify real worker execution separately from connectivity, with cleanup and recovery for successful and failed checks.
- Protected uncommitted ticket work when Git capture fails, with clear pause reasons and a Retry capture action.
- Improved failed-run diagnostics with the engine's error details and the affected execution context.
- Fixed dispatch of tickets explicitly assigned to an allowed worker.

## 0.2.0

- Expanded LAN access to the full signed-in dashboard, while keeping initial setup and owner recovery local to the host.
- Fixed LAN address and port changes rolling back, and improved confirmation that LAN access is disabled.
- Improved worker recreation to prevent container conflicts, protect unrelated containers, and report failures more clearly.
- Prevented concurrent worker-image build requests from starting duplicate builds, while honoring explicit rebuild requests.
- Fixed runtime service Open links when using LStack over LAN, with warnings for runtimes bound to localhost.

<br>

---

<br>

## 0.1.4

- Added an option to create a default worker when adding a provider.
- Added a way to review and apply proposed corrections to verification checks.
- Fixed conflicting worker assignments and improved resume, restart, and stop handling.
- Strengthened security for project document reading and search, with clearer messages for blocked documents.

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

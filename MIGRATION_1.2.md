# Updater 1.2 migration artifacts - not activated

The compatibility bridge **1.1.11** and signed-maintenance core **1.2.1** are
staged here for verification. The normal `updater-latest.json` feed still offers
**1.1.10**. Do not manually install these staged packages or instruct a recipient
to migrate yet: the native migration pilot and signing-key recovery preparation
must be completed before the feed is activated.

## Intended path after activation

1. In the existing LeanStream Updater, choose **Update updater**. It installs
   compatibility bridge 1.1.11 using the same add-on ID and local profile.
2. Exit Kodi normally and reopen it. Choose **Update updater** again. The bridge
   checks Kodi's installed, enabled crypto dependency, then downloads only its
   pinned core 1.2.1 package. A missing or incompatible dependency stops safely
   for repair through Kodi; it does not copy PC binaries or hide dependencies.
3. Exit and reopen Kodi normally again. The recipient must explicitly enroll
   this Kodi and approve the selected maintenance permissions before signed
   maintenance jobs can run. Enrollment can be revoked locally.

No uninstall, data clearing, account transfer or new token is part of this path.
Public updater downloads do not use or receive the private content token.
Private LeanStream content is separate and is **not updated by this staging**.
SubtitleDB, trailer changes and helper disabling are not published here as jobs.

## Scope and trust

The bridge is a one-time compatibility step: old clients cannot validate the
new core's additional dependency directly. Its next-hop version, size, hash and
public trust root are pinned inside the bridge. The old HTTPS/hash-only first
hop is not retroactively protected by signatures. The core verifies signed,
targeted, expiring jobs with replay protection, visible review and local backups.

There is no live remote-administration listener, startup update polling or
automatic maintenance. Executable Kodi packages trust their signing operator;
they are not sandboxed. Each recipient's consent and recovery preparations are
required. Code recovery and settings recovery are separate operations.

## Immutable staged packages

| Package | Bytes | SHA-256 |
| --- | ---: | --- |
| `plugin.program.leanstream.updater-1.1.11.zip` | 71,229 | `7d0c43ebefa4b1b81432bb4d6e12c1cac199b435b6dc864206a547d79c5e97ae` |
| `plugin.program.leanstream.updater-1.2.1.zip` | 92,009 | `93b47948ba7b408bd5e0c5405022065362a86fe5361e0b9b26134d1219885492` |

The packages and adjacent `.sha256` files are stored at the repository root.
Older release files remain available. Staging these files is not a claim of a
completed native migration test or a production-ready friend rollout.

# Updater 1.2.2 two-hop migration artifacts

The compatibility bridge **1.1.12** and signed-maintenance core **1.2.2** are
the updater-only migration path for the single in-scope friend Shield, subject
to the recipient's explicit consent.

Package presence alone does not activate the migration. `updater-latest.json`
is authoritative: version **1.1.10** means staged/inactive, while version
**1.1.12** offers the bridge. Change it only after anonymous artifact
verification, the exact native owner-Shield pilot and explicit activation
approval. Do not manually install these packages or instruct the recipient
before activation.

## Intended path after activation

1. In an existing LeanStream Updater from 1.1.2 through 1.1.10, choose
   **Update updater**. It installs compatibility bridge 1.1.12 using the same
   add-on ID and local profile.
2. Exit Kodi normally and reopen it.
3. Choose **Update updater** again. The bridge accepts only its pinned
   core 1.2.2 version, size, SHA-256 and trust-root bytes. Before code
   replacement it requires Kodi's `script.module.pycryptodome` dependency to be
   installed, enabled and at least 3.4.3. A missing, disabled or older dependency
   stops before writes; repair it through Kodi rather than copying PC binaries.
4. Exit Kodi normally and reopen it again, then verify updater 1.2.2.
5. The recipient locally reviews enrollment, channel and permitted scopes.
   Enrollment is never automatic and can be revoked locally.

No USB drive, manual ZIP installation, uninstall, data clearing, new token,
account reset, profile transfer or provider transfer is part of this path.
Public updater downloads do not read or receive the private repository token.

## Updater-only scope

These artifacts update only `plugin.program.leanstream.updater`. They do not
update LeanStream main, the LeanStream skin, SubtitleDB, helper add-ons,
accounts, providers, settings or private content.

This release does not include a signed cumulative Friends-channel content job.
After installing updater 1.2.2, do **not** choose **Update LeanStream** unless a
separately signed current job has later been published, independently verified
and explicitly approved.

## Trust and consent

The old client's first hop uses the existing HTTPS/hash trust boundary; it
cannot retroactively verify signatures that it does not yet support. Bridge 1.1.12
pins the exact next core package and public trust root. Core 1.2.2 verifies
signed, targeted, expiring jobs with replay protection, visible review and
local rollback evidence.

There is no live remote-administration listener, startup update polling,
automatic enrollment or automatic maintenance. Signed executable Kodi packages
trust their signing operator and are not security-sandboxed. The recipient must
consent to this photographed device and review every requested permission.

## Stop conditions

Stop without retrying or resetting anything if:

- the installed or offered version differs from the expected two-hop path;
- a hash, dependency, enrollment or package warning appears unexpectedly;
- a download returns 404 or another network error;
- a token, account, skin, setting or profile changes unexpectedly;
- any step asks for uninstall, data clearing, a new token or profile transfer.

Do not reset the token or account to work around an updater error. Preserve
`.leanstream-managed-*`, journal, history and backup folders for recovery.

## Candidate packages for staged publication

| Package | Bytes | SHA-256 |
| --- | ---: | --- |
| `plugin.program.leanstream.updater-1.1.12.zip` | 71,232 | `c43527268a3a218d2821002fea2c803de4eed2ef7e91edb7f5d0bdc818cf96f4` |
| `plugin.program.leanstream.updater-1.2.2.zip` | 100,885 | `349eb4e6786ee22f859c87f4473ef0389977a57c86b06246be81f4b815ff4ddc` |

Before publishing this notice, place both packages and their adjacent `.sha256`
files at the repository root and verify their exact local bytes. Publish the
notice with the bridge only after the core is already anonymously verified.
Immediately afterward, anonymously verify the served bridge, checksum and
notice before the native pilot or feed activation. Older immutable releases
remain available. Staging these files is not evidence that the native pilot,
feed activation or friend installation has completed.

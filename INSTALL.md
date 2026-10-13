# LeanStream updater 1.1.4 - controlled test

## Minimum and ABI compatibility repair

Version1.1.4 preserves both import minversion and compiled version, and checks
the provided backwards-compatible ABI as Kodi21 does. Duplicate/transitive
declarations and verified planned packages keep both constraints. The former
filesystem1.1.8/minimum1.1.9 warning can be false: the actual declared minimum
may be1.1.7, subject also to the device's provided ABI. Do not upgrade Kodi based
on that old warning alone. Unknown/malformed required metadata and genuinely
incompatible versions remain blockers. Reports show updater/Kodi versions,
requested interface, provided ABI and requesting add-ons for easier diagnosis.
Local tests/actual PC XML audits are not native Shield acceptance; send a fresh
read-only report after upgrading the updater. No credentials are needed to update
the updater itself. This candidate does not publish or install the private suite.

## Suite prerequisites managed by the installer

Kodi built-in interfaces are checked from its application VFS metadata, not
reported missing merely because the ordinary JSON-RPC add-on list omits them.
Required missing add-ons and disabled approved modules are prepared through Kodi
native install/enable dialogs after the paired suite ZIPs and AI files verify.
Available declared optional modules may also be prepared; absent optional ones
are non-blocking. The read-only check never installs anything. Every required
component is rechecked before replacing the private suite code.

Kodi owns repository/platform selection and native confirmation; no security,
repository or account settings are changed. Completed prerequisite changes may
remain after cancellation and are not covered by private suite code rollback.
Old/unknown required versions still block: Kodi21 InstallAddon does not update
already installed old add-ons. No global update, uninstall or guessed success.
Native dialog/runtime behavior and Android metadata still need device acceptance.

## Manual updater self-upgrade

Version 1.1.2 added Update updater (public download) and Restore updater backup.
Install this bootstrap ZIP once over the existing updater. Future updater releases
can then be checked and installed from its menu, after your confirmation and ZIP
verification. A code-only updater backup is saved; settings/credentials remain.
Exit/reopen Kodi normally after a self-upgrade or restore. No automatic updates.

The updater-only feed is updater-latest.json on this public host. It does not
require a GitHub token and cannot select private add-on/skin/AI installation targets.
If an interrupted upgrade leaves the updater unavailable, reinstall this bootstrap
ZIP from the same Kodi source without uninstalling or clearing its settings.

## Included prerequisite-check repair

The prior 1.1.1 repair for "Unrecognised add-on version" is retained for dependency
formats such as 1.26.16+matrix.1. Unknown dependency versions appear in the report;
unknown required versions still block installation. Install this ZIP over the existing updater,
keep all existing settings, then rerun the read-only check. No account reset needed.

## Install directly in Kodi on the Shield

1. Kodi Settings -> File manager -> Add source.
2. Enter https://shana00.github.io/leanstream-updater/ and name it LeanStream Updater.
3. Open Add-ons -> Add-on browser -> Install from ZIP file.
4. If needed, read and accept Kodi's Unknown sources warning yourself.
5. Select LeanStream Updater -> plugin.program.leanstream.updater-1.1.4.zip.
6. Install over the existing updater; do not uninstall it or delete its settings.
7. Open Program add-ons -> LeanStream Private Updater. Verify version 1.1.4; exit/reopen Kodi normally.
8. Run Check installed prerequisites (no changes). Send only a sanitised report.
9. STOP until the private add-on + skin + AI test release is prepared and approved.

## Credentials and private packages

No credentials, personal settings, Kodi profile, account data, add-on, skin or AI
model are included in this public ZIP. Existing device credentials stay on that
device. Each user needs their own approved read-only access to the private package
repository. Configure that privately in the updater only if it is not already set.
Never send tokens, passwords, cookies, support codes or account settings in a chat.

## Default skin after the full private bundle

The paired installer offers to make LeanStream the default after a normal Kodi
restart. This requires owner approval, verified complete installation and intact
model/skin files. Choose Yes in Kodi's native Keep this skin prompt; a timeout or
decline is not overridden. Previous skin stays installed for recovery. Installing
this updater alone never switches a skin. If needed, enable the add-on in My
add-ons and choose Finish LeanStream default-skin setup in the updater.

## Test status and rollback

Local isolated tests and package checks are not Shield runtime acceptance.
Private access, Android file permissions, Kodi registration, D-pad dialogs,
restart and the native skin confirmation must be checked on the actual Shield.
The existing stable private feed is not changed by this updater-only download.
Do not force-stop Kodi or clear its data. Use the updater's verified code restore
before downgrading the updater if you have applied a paired update.

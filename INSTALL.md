# LeanStream updater 1.1.1 - controlled test

## Prerequisite-check repair

Version 1.1.1 fixes the "Unrecognised add-on version" error caused by dependency
formats such as 1.26.16+matrix.1. Unknown dependency versions appear in the report;
unknown required versions still block installation. Install this ZIP over 1.1.0,
keep all existing settings, then rerun the read-only check. No account reset needed.

## Install directly in Kodi on the Shield

1. Kodi Settings -> File manager -> Add source.
2. Enter https://shana00.github.io/leanstream-updater/ and name it LeanStream Updater.
3. Open Add-ons -> Add-on browser -> Install from ZIP file.
4. If needed, read and accept Kodi's Unknown sources warning yourself.
5. Select LeanStream Updater -> plugin.program.leanstream.updater-1.1.1.zip.
6. Install over the existing updater; do not uninstall it or delete its settings.
7. Open Program add-ons -> LeanStream Private Updater. Verify version 1.1.1.
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

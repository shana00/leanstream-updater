# LeanStream Updater1.1.9

## Existing updater

1. Open LeanStream Updater and select **Update updater (public download)**.
2. Approve1.1.9, then exit Kodi normally and reopen. Confirm updater1.1.9.
3. For the owner's approved private test update, select **Check Shield test
   release - add-on + skin + AI**. The update should propose add-on1.0.23.23 and
   skin0.3.2. Do not use the older add-on-only release.
4. Approve the package update. If already using LeanStream, there is no need to
   change the default skin again; choose No for that separate skin-change offer.
5. Exit/reopen Kodi normally after completion. Existing accounts/provider data
   are preserved; no uninstall, data clear, new token or account reset is needed.
6. Check the new vertical menus and highlight Discover/Search/Accounts/Settings
   to populate their panels. Accounts -> Setup check shows the short checklist.

Private suite downloads use only the device's existing authorized read access.
If GitHub access fails, use Check GitHub access and share its safe report, never
the token or a screenshot of credential settings. This publication does not
remotely install on a Shield; its owner approves the local update.

## First installation / recovery

Use Kodi File manager source <https://shana00.github.io/leanstream-updater/> and
Install from ZIP -> plugin.program.leanstream.updater-1.1.9.zip. For an existing
installation, install over it without uninstalling or resetting its settings.
The manual bootstrap is a recovery path if self-update was interrupted.

## Setup report and privacy

The first page has six checkboxes. Checked means installed metadata, file
integrity or saved configuration found, NOT online service validity or playable
sources. Technical details and the QR/saved text include the full sanitized
dependency/AI/provider/service report. MDBList's ratings key is independent of
watch/list synchronization. Playback services are alternatives, not all required.

Download on phone starts a temporary local HTTP server only while the QR is
open, for at most five minutes/eight downloads. Use trusted same-Wi-Fi only:
HTTP is not encrypted. Closing the QR stops sharing. No external QR service,
automatic public upload or email. Save report writes uniquely named text only
to your chosen folder. No raw Kodi log, keys, tokens, account values, source URLs
or account settings are included. Actual phone/remote-device reachability depends
on the local network and remains a device acceptance check.

## Optional preferences and rollback

Setup check applies no preferences. Separate trailer, Android playback and PC
scraping presets require explicit confirmation; decline if unsure. Do not choose
Apply PC scraping preferences merely to install the menu fixes. Existing settings
stay unchanged when those optional offers are declined.

Android playback: MediaCodec ON / Surface OFF, maximum1080p trailers. It affects
ALL Kodi video. HDR/Dolby Vision output remains unverified; review the full warning
before deciding. PC scrape preset: twelve allowlisted preferences,10s timeout,
tier skip off and15 qualifying torrent sources. Cloud/direct/adaptive results can
stop earlier. Counted/cached does not mean playback-tested;10s may limit providers.

Restore last update backup restores suite CODE; Restore updater backup is
separate. Preference restores are separate again and preserve newer choices.
Completed native prerequisite installations may remain after suite cancellation
and are not undone by suite-code rollback. Kodi built-in interfaces are not
separate downloads; optional missing modules alone are not required blockers.

The stable release is unchanged. Startup/return freezes, Keep-skin behavior,
HDR output and individual source/service failures are not claimed solved by
this presentation/setup update. Use your own accounts; never send credentials.

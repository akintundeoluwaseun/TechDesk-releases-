# TechDesk Releases

This repo hosts the download files for TechDesk (Solo, Business, Enterprise).
It doesn't host source code — just installers, one **GitHub Release** per
version.

## Why Releases, not plain folders

GitHub refuses any file over **100 MB** uploaded the normal way (drag-and-drop
into a folder, or the "Add file" button) — it just rejects it. Some of these
installers are 300 MB+. **Releases** are a separate GitHub feature built
specifically for this: attached files there can be up to 2 GB, and they get a
stable, direct download link that starts the download immediately — no
Google Drive-style "scan for viruses" confirmation page.

So: **installer files always go into a Release, never into the `solo/`,
`business/`, or `enterprise/` folders.** Those folders are just for small
text files — changelogs, checksums — not the installers themselves.

## How to publish a new version (step by step)

1. On this repo's GitHub page, click **Releases** (right-hand sidebar) →
   **Create a new release** (or **Draft a new release**).
2. **Tag**: use `solo-v2.0.0` style — edition name, then the version. Example
   tags: `solo-v2.0.0`, `business-v1.0.0`, `enterprise-v1.0.0`.
3. **Release title**: something readable, e.g. "TechDesk Solo 2.0.0".
4. **Description**: whatever's changed in this version (optional but useful).
5. Drag all the installer files for that version into the assets box at the
   bottom (the Windows `.exe`, both macOS `.zip` files, the `.deb`, the
   `.rpm` — whichever apply).
6. Click **Publish release**.
7. Each uploaded file gets its own permanent link, shaped like:
   `https://github.com/akintundeoluwaseun/TechDesk-releases-/releases/download/solo-v2.0.0/TechDesk2.0-Setup-1.exe`
   Send me those links (or the release page URL) and I'll wire them into the
   website's download buttons.

## Current versions

| Edition        | Latest version | Status         |
|----------------|-----------------|----------------|
| Solo           | 2.0.0           | Windows + Linux AppImage live on the site; macOS and .deb/.rpm still pending upload |
| Business       | —               | Not released yet |
| Enterprise     | —               | Not released yet |

This table gets updated by hand each time a new Release goes up — ask me to
update it (and the website's download links) whenever you publish one.

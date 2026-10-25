# dc1-updates

Update channel for the DC-1 Android 17 builds. The tablets' LineageOS Updater reads one index per build:

- `lineage_dc1_gsi.json` (full build)
- `lineage_dc1_gsi_lite.json` (minimal build)

Each index is a JSON array of releases (`datetime`, `type`, `version`, and `files` with `filename`, `sha256`, `size`,
`url`). The update packages are attached to this repository's GitHub Releases and are signed with the project's
release key. A tablet installs only packages signed with that key.

An empty array means no update is published yet.

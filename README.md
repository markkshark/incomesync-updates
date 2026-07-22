# IncomeSync update manifest

Serves `latest.json` for the IncomeSync desktop app update check (notify-only).
The app compares its running version against `version` here and shows a banner.

## Release step
On each release: bump `version` (and `notes`), commit, push. GitHub Pages serves
https://markkshark.github.io/incomesync-updates/latest.json within a minute.
No customer data is involved; the check sends no identifiers beyond the HTTPS request itself.

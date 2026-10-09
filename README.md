# die Confidence — releases

This repository only carries the release files for **die Confidence**, the die Keure desktop app that has coding
agents (Claude Code) work through a workflow step by step and keeps the evidence. The source code lives elsewhere.

An installed die Confidence polls the latest release here for `latest.json` and updates itself. Each release holds:

- `latest.json`: the update manifest the app reads
- `die-confidence_<version>_aarch64.app.tar.gz`: the signed update bundle
- `die Confidence_<version>_arm64.dmg`: for a first install (Apple Silicon)

First install: open the dmg, drag die Confidence to Applications, then run once in Terminal:

```
xattr -cr "/Applications/die Confidence.app"
```

After that the app keeps itself current.

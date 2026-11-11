# Payload Manager source

This repository publishes its own development builds for PS5 Payload Manager.

## Add the source

In Payload Manager, open **Settings → Manage Sources → Add Source**, then paste:

```text
https://github.com/dviree/ShadowMountPluszstd/releases/download/payload-manager/payloads.json
```

The source becomes available after the first successful **PS5 Build and Release** workflow run.

Select **ShadowMount Plus ZSTD (dviree)** to download this fork's compiled ELF. Avoid autoloading a second copy of ShadowMount Plus alongside it.

## Updates

Each successful push or manual build on branch `1.7` publishes an ELF with a unique asset name and regenerates the catalog. The catalog includes a stable payload ID, a development version, the publication date and a SHA-256 checksum. The new ELF is uploaded before the catalog is replaced; previously published ELF assets remain available.

These are development snapshots from this fork, not upstream stable releases. This workflow does not automatically pull upstream code or install updates on your console. Use the same source URL for future builds.

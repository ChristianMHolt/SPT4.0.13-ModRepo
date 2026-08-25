# SPT 4.0.13 Modpack

This repo hosts the **modpack manifest** and the handful of mods that are **not on The Forge**, used by the `ModpackInstaller` app.

- `modpack.json` — the manifest (mod list, pinned versions, SHA-256 hashes, download URLs, install layout).
- `Oryzaki-LootValueNP-1.0.0.zip` — custom mod (not on Forge).
- `LoadAmmoAnim-1.6.0.zip` — Manimal's LoadAmmoAnim (not on Forge).
- `Manimal-HackerMod-1.0.2.zip` — Manimal's HackerMod (not on Forge).
- `FPVDroneModFikaSync.7z` — FPV Drone Mod Fika sync addon (not on Forge).

Everything else in the pack is downloaded directly from The Forge (`sp-mod.com`) at the exact pinned version and verified against the SHA-256 recorded in `modpack.json`.

## Updating the pack

1. Edit / regenerate `modpack.json` (see the `work/` manifest-builder for how it's produced from a local mods folder).
2. Commit and push — the installer always fetches `modpack.json` from this repo's `main` branch.

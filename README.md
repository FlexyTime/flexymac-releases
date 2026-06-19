# flexymac-releases

Auto-update distribution channel for the **Flexytime macOS** app.

Source code lives in the (private) `flexytime-v2` mono. This repo only carries:

- `docs/appcast.xml` — Sparkle appcast served via GitHub Pages at
  <https://flexytime.github.io/flexymac-releases/appcast.xml>.
- GitHub Releases — signed + notarized DMGs, EdDSA-signed by Sparkle.

Releases are produced by the `mac-release.yml` workflow in `flexytime-v2`
on every push to `main` that touches `flexytime-mac/**`. Do not push
changes here by hand — they will be overwritten on the next release.

Bootstrapped 2026-06-19. See
[`flexytime-mac/docs/auto-update-setup.md`](https://github.com/FlexyTime/flexytime-v2/blob/main/flexytime-mac/docs/auto-update-setup.md)
for the full pipeline.

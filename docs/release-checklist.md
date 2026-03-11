# Release Checklist

> If GitHub Actions auto-release is configured, sections 2-3 are handled automatically on merge to `main`.

## 1) Pre-release validation

- [ ] Verify `manifest.json` version bump.
- [ ] Confirm matched URLs are correct and minimal.
- [ ] Test manually on each supported URL.
- [ ] Confirm no real personal data in repo assets.
- [ ] Confirm policy and listing docs are up to date.

## 2) Build release package

- [ ] Create a clean zip of extension root contents:
  - `manifest.json`
  - `hide.css`
  - `icons/` (if included)
- [ ] Exclude `.git`, docs not needed in package, and local artifacts.

Automated workflow package:

- `manifest.json`
- `hide.css`
- `icons/`

Example command:

```bash
zip -r hetu-hide-extension-vX.Y.Z.zip manifest.json hide.css icons
```

## 3) Chrome Web Store submission/update

- [ ] Upload updated zip.
- [ ] Update listing text as needed.
- [ ] Confirm privacy disclosure answers remain accurate.
- [ ] Submit for review.

When auto-release is enabled, these are done by `.github/workflows/release-to-chrome-web-store.yml`.

## 4) Open source release

- [ ] Tag release (`vX.Y.Z`).
- [ ] Add release notes (what changed and why).
- [ ] Publish GitHub release with attached zip (optional).

## 5) Post-release

- [ ] Verify installed store version behavior.
- [ ] Monitor issues and user feedback.

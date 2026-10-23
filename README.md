# VioDeck v1 Downloads

**Private candidate downloads only — not an official release.** This repository has no release tag or GitHub Release. Do not treat these files as supported production installers or redistribute them publicly.

## Artifacts

| File | Platform/format | SHA-256 |
|---|---|---|
| `VioDeck_1.0.0_amd64.AppImage` | Linux x86-64 AppImage | `8e4c56189022bb474a260508c1d3d909a1a6d3d60eee80b0d75c754dc6b2b645` |
| `VioDeck_1.0.0_amd64.deb` | Debian package, amd64 | `a52777228796644cc996a75279aed275397a91a7217a8e64bb52c413b798978f` |

The AppImage is stored with Git LFS. Clone the repo and run `git lfs pull` before checking `SHA256SUMS`.

## Install

See [INSTALL.md](INSTALL.md) for download, checksum, and install steps. The `.deb` and AppImage were built locally on Arch/Omarchy from VioDeck source commit [`a70b231`](https://github.com/michaeldev-collab/viodeck-v1/commit/a70b2319125888f8cc409915f17340f5277f3b53) (branch `feat/keyboard-lighting-page`, open draft [PR #3](https://github.com/michaeldev-collab/viodeck-v1/pull/3), not yet merged to `main`). They are not official Ubuntu 24.04 artifacts and have not passed clean-install, cross-distribution, or physical-device acceptance.

Update 2026-10-22: rebuilt to include a dedicated Keyboard lighting (RGB) navigation page and a profile-select text rendering fix. Physical RGB writes remain backend-gated and disabled; no hardware command is sent by this build.

GitHub Actions for the source candidate was blocked before job steps by an account billing/spending-limit issue. No CI pass is claimed.

## Licensing and release status

The packages include VioDeck's proprietary `LICENSE`, generated third-party notices and license summary, and the Liberation Sans font license under `usr/lib/VioDeck/licenses/`. Copies are in [`legal/`](legal/) for review alongside the downloads. The third-party terms remain applicable to their components.

The packaged proprietary `LICENSE` is not an EULA or privacy policy. A full EULA/privacy policy and VioDeck trademark clearance are still outstanding; see the source repo's `docs/legal/TODO.md`. RGB hardware experiment V1 remains blocked, unauthorized, and untested.

The repository is private; GitHub authentication and access are required to clone/download the AppImage's LFS object.

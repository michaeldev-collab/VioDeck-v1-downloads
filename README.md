# VioDeck v1 Downloads

**Private candidate downloads only — not an official release.** This repository has no release tag or GitHub Release. Do not treat these files as supported production installers or redistribute them publicly.

## Artifacts

| File | Platform/format | SHA-256 |
|---|---|---|
| `VioDeck_1.0.0_amd64.AppImage` | Linux x86-64 AppImage | `ea90c188fd05d9433524dd7d9d98a22c363c05cd49737d0004b633f35296d856` |
| `VioDeck_1.0.0_amd64.deb` | Debian package, amd64 | `0ff58f3856e6b5e7434a26af94fcd2379a8ced01ddf342cd9bf6e87c6e8b564f` |

The AppImage is stored with Git LFS. Clone the repo and run `git lfs pull` before checking `SHA256SUMS`.

## Install

See [INSTALL.md](INSTALL.md) for download, checksum, and install steps. The `.deb` and AppImage were built locally on Arch/Omarchy from VioDeck source commit [`d75ad4b`](https://github.com/michaeldev-collab/viodeck-v1/commit/d75ad4bf01ec7c69c00cd24d7bd92a2e72c4abec). They are not official Ubuntu 24.04 artifacts and have not passed clean-install, cross-distribution, or physical-device acceptance.

GitHub Actions for the source candidate was blocked before job steps by an account billing/spending-limit issue. No CI pass is claimed.

## Licensing and release status

The packages include VioDeck's proprietary `LICENSE`, generated third-party notices and license summary, and the Liberation Sans font license under `usr/lib/VioDeck/licenses/`. Copies are in [`legal/`](legal/) for review alongside the downloads. The third-party terms remain applicable to their components.

The packaged proprietary `LICENSE` is not an EULA or privacy policy. A full EULA/privacy policy and VioDeck trademark clearance are still outstanding; see the source repo's `docs/legal/TODO.md`. RGB hardware experiment V1 remains blocked, unauthorized, and untested.

The repository is private; GitHub authentication and access are required to clone/download the AppImage's LFS object.

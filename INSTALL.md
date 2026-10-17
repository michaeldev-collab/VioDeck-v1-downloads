# Install and verify

These steps apply to the **private VioDeck 1.0.0 candidate** only. The packages were built locally on Arch/Omarchy; they are not official Ubuntu 24.04 builds, and clean-install/cross-distribution acceptance has not been completed. Use a disposable test machine or VM. Do not launch the app while a K1 Pro is attached until its separate hardware test is authorized.

## 1. Download and verify

You need access to this private GitHub repository and Git LFS installed.

```sh
git lfs install
git clone https://github.com/michaeldev-collab/VioDeck-v1-downloads.git
cd VioDeck-v1-downloads
git lfs pull
sha256sum -c SHA256SUMS
```

Both artifact checks must report `OK` before installing.

## 2. Linux x86-64 AppImage

Use this on Linux x86-64. Arch/Omarchy is the build host; other distributions have not been qualified.

```sh
chmod +x VioDeck_1.0.0_amd64.AppImage
./VioDeck_1.0.0_amd64.AppImage --version
```

To open the GUI, run the AppImage without `--version`. Do not launch it with a K1 Pro attached until hardware validation is separately authorized. The package does not migrate a user's profiles.

## 3. Debian package (amd64)

The `.deb` is intended for Debian/Ubuntu-family systems, but this local Arch-built candidate has not been validated on a clean Debian or Ubuntu install. Test in a disposable VM, not on a production device. It declares system dependencies and replaces/conflicts with the legacy `k1-pro-configurator` package name when installed by a package manager.

```sh
sudo apt install ./VioDeck_1.0.0_amd64.deb
```

After installation, the desktop entry is named **VioDeck**. Do not launch it with a K1 Pro attached until hardware validation is separately authorized. Installing the package does not migrate profiles.

## 4. Legal files

The AppImage and `.deb` include the VioDeck `LICENSE`, `THIRD_PARTY_NOTICES.md`, `THIRD_PARTY_LICENSES.md`, and Liberation Sans license under `usr/lib/VioDeck/licenses/`. The corresponding source files are in [`legal/`](legal/). The proprietary license is not an EULA or privacy policy; those documents and VioDeck trademark clearance remain unresolved.

## 5. Support boundary

This is a candidate download, not an official release or promise of supported platforms. GitHub Actions was blocked before any steps by the account billing/spending-limit issue. No CI pass, clean install, cross-distribution acceptance, or physical K1 Pro test is claimed. RGB hardware experiment V1 is blocked, unauthorized, and untested.

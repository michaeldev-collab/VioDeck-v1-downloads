# Third-party licenses

This file is a compatibility alias. The generated inventory — crate and npm
names, versions, SPDX licenses, required notice text, hidapi, and flagged
copyleft/unknown items — is [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md).

Regenerate:

```console
cargo fetch --locked
python3 scripts/generate_third_party_notices.py
```

The machine-readable hash list for the vendored StreamDock transport
binaries remains `third_party/streamdock-sdk/native-binaries.json`.

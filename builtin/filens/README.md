# FiLens CLI for ZimaOS

```sh
sudo zpkg install filens
filens capacity --json
filens read report.pdf --json
```

If the module is not found, run `sudo zpkg update` and retry. To upgrade,
run `sudo zpkg update` followed by `sudo zpkg upgrade filens`.

The system extension installs `/usr/bin/filens`, native Linux x64/arm64 binaries
and shared WASM document engines. It needs no Node.js or background service.
OCR reuses Photos' installed NCNN v7 JSON v2 runtime and RapidOCR model files.
When they are absent or incompatible, OCR reports unavailable; other CLI
capabilities remain usable. No browser site, models or NCNN libraries are
included in this package.

The versioned raw image is served through jsDelivr and kept below 15 MB.
`filens.meta.json` records its URL, size, SHA-256 and the integrity of its source
npm packages. Verify a downloaded image from this directory with
`shasum -a 256 -c SHA256SUMS`. AppManagement's raw module downloader uses one
URL; it does not switch between multiple mirrors.

Build and packaging instructions:
<https://github.com/IceWhaleTech/filens/blob/main/packaging/zimaos/README.md>.

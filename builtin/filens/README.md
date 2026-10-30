# FiLens for ZimaOS

FiLens is a browser frontend for local file previews. ZimaOS serves it at
`/modules/filens/` through the existing gateway.

```sh
sudo zpkg install filens
```

If the module is not found, run `sudo zpkg update` to refresh the store index,
then retry. For updates, run `sudo zpkg update` followed by
`sudo zpkg upgrade filens`.

`filens.meta.json` records the release version, download URL, byte size and
SHA-256. The package is stored as `filens.raw` in the versioned
`filens-v0.1.0` Release. Large raw packages belong in Release assets rather than
Git or jsDelivr's repository CDN. `mod-v2.json` and `mod.json` map the `filens`
name to that asset.

Build and packaging instructions:
<https://github.com/IceWhaleTech/filens/blob/main/packaging/zimaos/README.md>.

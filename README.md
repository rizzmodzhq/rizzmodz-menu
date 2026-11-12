# RizzModz Menu

Public releases of the **RMz** mod menu: the RizzModz Mod Menu, `RMz.framework`, and the RMz Companion app.
This repo holds release binaries only.

## Jailbroken: add the repo

Add **`https://repo.rizzmodz.com/`** in Sileo, Zebra, or Cydia, then install **RizzModz Mod Menu**.
It installs the framework and the Companion with it, and each one updates on its own from the repo.

Rootful and rootless are both supported. Your package manager picks the right build. Roothide support is not available yet.

## Non-jailbroken: NJB inject zip

Download `RMz-<version>-njb-inject.zip` from [Releases](../../releases). It contains `RMzModMenu.dylib` and
`RMz.framework`. Inject both into the target app with your sideloading tool (LiveContainer's Tweaks folder,
ESign, Feather), keeping them side by side in the same folder.

## Release assets

Each framework release (`vX.Y.Z`) on [Releases](../../releases) contains:

| File | What |
|---|---|
| `RMz-Framework-<version>-rootless.deb` / `-rootful.deb` | RMz Framework |
| `RizzModz-Menu-<version>-rootless.deb` / `-rootful.deb` | RizzModz Mod Menu |
| `RMz-Companion-<version>-rootless.deb` / `-rootful.deb` | RMz Companion app |
| `RMz-<version>-njb-inject.zip` | Mod menu + framework for non-jailbroken devices |
| `SHA256SUMS` | Checksums for every file above |

Each package has its own version. Menu and Companion updates between framework releases ship through the repo.

## Verify a download

```sh
shasum -a 256 -c SHA256SUMS --ignore-missing
```

## Support

Report problems in [Issues](../../issues). Include your device, iOS version, jailbreak (or NJB tool),
and the package versions.

# RizzModz Menu

Public releases of the **RMz** mod menu: `RMz.framework` plus the remote client.
This repo holds release binaries only. Grab the latest from [Releases](../../releases).

## Release assets

Every release (`vX.Y.Z`) ships the same set of files:

| File | For |
|---|---|
| `RMz-<version>-rootless.deb` | Rootless jailbreaks (Dopamine, palera1n rootless). Installs under `/var/jb`. |
| `RMz-<version>-rootful.deb` | Rootful jailbreaks (checkra1n, palera1n rootful, unc0ver, Taurine). |
| `RMz-<version>-njb-inject.zip` | Non-jailbroken devices. Has `RMz.framework` and the remote client dylib, for injecting into an IPA. |
| `SHA256SUMS` | Checksums for every asset above. |

> Roothide (`RMz-<version>-roothide.deb`) is not supported yet. It will be added under this name when it is.

## Install

**Jailbroken:** download the `.deb` that matches your jailbreak and install it with Sileo, Zebra, or
`dpkg -i`, then respring.

**Non-jailbroken:** unzip `RMz-<version>-njb-inject.zip` and inject both `RMz.framework` and the client
dylib into the target IPA with your injector or sideloading tool, then sign and install.

## Verify a download

```sh
shasum -a 256 -c SHA256SUMS
```

## Support

Issues with a release can be reported in [Issues](../../issues). Include your iOS version, device,
jailbreak (or njb), and the release version.

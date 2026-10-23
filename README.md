# RustySteamless

A cross-platform rewrite of [Steamless](https://github.com/atom0s/Steamless) in Rust.
It removes SteamStub DRM from executable files, so they can be analyzed and modified after unpacking.

Rusty-Steamless ships as a Tauri app plus a CLI version for automatable or scripted use.

## Build

```
cargo build --release
```

The CLI binary is produced at `target/release/rusty-steamless`. The Tauri GUI builds from `app/` with `npm install && npm run tauri build`.

## CLI usage

```
rusty-steamless <FILE> [--keepbind] [--keepstub] [--dumppayload] [--dumpdrmp] [--realign] [--recalcchecksum] [--exp]
```

## Credits

Rusty-Steamless is a port of **Steamless**, written by [Atom0s](https://github.com/atom0s).
All unpacking logic is derived from the original [Steamless C# project](https://github.com/atom0s/Steamless).

## Feedback

Found a bug or have a suggestion? Please [open an issue](https://github.com/notwinterdust/RustySteamless/issues).

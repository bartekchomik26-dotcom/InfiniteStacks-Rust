# Unlimited Stacks (`unlimited_stacks_mod`)
A native mod for [Horizon](https://github.com/horizon-rust/horizon) that raises the stack limit for items that normally stack to 64, configurable in-game up to `2,147,483,647` (`i32::MAX`).
## Features
- **Configurable Limits**: Set any whole number from `1` to `2,147,483,647` in **Options > Mods > Unlimited Stacks**.
- **Compact HUD Labels**: Automatic compact number formatting on item icons (`1k`, `1.5m`, `2.14b`) with automatic text scaling to fit slot boundaries.
- **Tool & Armor Safe**: Preserves 1-stack items (tools, weapons, armor) and 16-stack items (ender pearls, eggs).
## Compatibility
- Requires Horizon builds with **PR #6800** or later (`cabe8b5de` / Nightly 2026-11-02+).
- Client and server must both run the mod to sync modded stacks above 99.
## Installation
1. Download the latest `.hnmod` release from [Releases](../../releases).
2. Drop `unlimited_stacks_mod-<version>.hnmod` into your Horizon launcher native mods directory:
   - **Windows**: `%AppData%\horizon-launcher\native\`
   - **Linux**: `~/.local/share/horizon-launcher/native/`
3. Click **Build** in the Horizon launcher.
## Packaging
To produce the `.hnmod` bundle:
```bash
zip -r unlimited_stacks_mod-1.2.5.hnmod horizon-native.json mixins/
```
## License
MIT

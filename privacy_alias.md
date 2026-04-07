# Privacy Policy

**AliasManager**
Last updated: April 2025

---

## Summary

AliasManager does not collect, transmit, or sell any personal data. Everything the app does stays on your device or in your personal iCloud account.

---

## What data does AliasManager access?

### Shell configuration files

AliasManager reads and writes the following files on your Mac:

- `~/.zshrc`
- `~/.bashrc`
- `~/.bash_profile`
- `~/.config/fish/config.fish`
- `~/.config/nushell/config.nu`

This data never leaves your device unless you explicitly enable iCloud sync (see below).

### Shell history files

When you use the **Shell History Analysis** feature, AliasManager reads:

- `~/.zsh_history`
- `~/.bash_history`

This data is processed entirely on-device to generate alias suggestions. It is never stored persistently by the app and never transmitted anywhere.

### iCloud Drive (optional)

If you enable **Sync with iCloud Drive**, AliasManager stores a single file named `aliases.aliasmanager` in your personal iCloud Drive container (`iCloud Drive / AliasManager /`). This file contains your alias names, commands, and settings.

This data is synced between your own Apple devices via iCloud and is governed by [Apple's iCloud Privacy Policy](https://www.apple.com/legal/privacy/). AliasManager does not have access to this data — it lives in your personal iCloud account.

iCloud sync is disabled by default and requires your explicit opt-in.

### Local app data

AliasManager stores the following data locally on your device using standard macOS mechanisms:

- **User preferences** (selected theme, active profile, sync settings) - stored in `UserDefaults`
- **Alias profiles** - stored in `~/Library/Application Support/AliasManager/profiles.json`
- **Alias history log** - stored in `~/Library/Application Support/AliasManager/history.json`
- **Config file backups** - stored alongside your config files as `.bak` files (e.g. `~/.zshrc.bak`)

All of this data stays on your device.

---

## What data does AliasManager NOT collect?

- No analytics or usage tracking
- No crash reporting sent to third parties
- No advertising identifiers
- No account registration required
- No data sold or shared with third parties
- No network requests except iCloud sync (which is opt-in and goes to your own account)

---

## Apple Events / Terminal access

AliasManager uses Apple Events to communicate with Terminal.app when you use the **Run in Terminal** or **Reload Shell** features. This only sends the specific command you choose to run. No data is logged or transmitted as a result of this.

---

## Children's Privacy

AliasManager is a developer tool intended for adults. It does not knowingly collect any information from children under 13.

---

## Changes to this policy

If we make changes to this privacy policy, we will update the date at the top of this page. Continued use of the app after changes constitutes acceptance of the updated policy.

---

## Contact

If you have any questions about this privacy policy, please contact us at:

**Email:** [offworldcolonies73@gmail.com](mailto:offworldcolonies73@gmail.com)

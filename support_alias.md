# AliasManager Support

## Contact

Have a question, found a bug, or want to request a feature?

**Email:** [offworldcolonies73@gmail.com](mailto:offworldcolonies73@gmail.com)

We typically respond within 1-2 business days.

---

## Frequently Asked Questions

### The app does not find my aliases

AliasManager looks for aliases in the following files:

- `~/.zshrc`
- `~/.bashrc`
- `~/.bash_profile`
- `~/.config/fish/config.fish`
- `~/.config/nushell/config.nu`

Make sure your aliases are defined in one of these files and that the file exists. If you store aliases in a separate file that is sourced from `.zshrc` (for example `~/.aliases`), you can import that file manually using the **Import...** button in the toolbar.

---

### My aliases disappeared after using the app

AliasManager creates a `.bak` backup of every config file before making any changes. You can find the backup at the same location as the original file, for example `~/.zshrc.bak`. Open it in any text editor to restore your aliases.

---

### Changes are not reflected in my terminal

After editing aliases in AliasManager, use the **Reload Shell** button in the toolbar (the circular arrow icon). This runs `source ~/.zshrc` (or the relevant file) in Terminal so that your changes take effect immediately in the current session.

New terminal windows and tabs will always pick up the changes automatically.

---

### The app asks me to pick a file on launch

If the app is running in sandboxed mode, macOS requires you to explicitly grant access to files outside the app's container. Select your shell config file in the file picker and AliasManager will remember your choice for future launches using a security-scoped bookmark.

---

### iCloud sync is not working

iCloud sync requires:

1. You are signed in to iCloud on your Mac (System Settings > Apple ID)
2. iCloud Drive is enabled
3. You have toggled on **Sync with iCloud Drive** inside AliasManager (toolbar cloud icon)

iCloud is not available in unsigned development builds. If you installed AliasManager from the App Store, iCloud sync should work out of the box once enabled.

---

### Shell history analysis found no suggestions

The history analyzer reads `~/.zsh_history` and `~/.bash_history` and looks for commands you have run 3 or more times. If no suggestions appear:

- Make sure history is enabled in your shell (`HISTFILE` is set and `SAVEHIST` is greater than 0 for zsh)
- Your history file may be empty or very short. Run some commands in the terminal and try again
- Commands shorter than 5 characters are filtered out to avoid noise

---

### How do I switch between profiles?

Click the **Profiles** button in the toolbar (the person icon) to open the Profiles panel. Tap any profile to activate it. Activating a profile enables the aliases associated with that profile and disables the rest.

To create a new profile, click **New Profile** and give it a name and icon. The profile will capture the current enabled/disabled state of all your aliases.

---

### A feature I want is missing

We would love to hear your ideas. Send a message to [offworldcolonies73@gmail.com](mailto:offworldcolonies73@gmail.com) with the subject line **Feature Request** and describe what you would like to see.

---

## System Requirements

- macOS 14.0 (Sonoma) or later
- Compatible with zsh, bash, fish, and nushell

---

## Version History

### 1.0
- Initial release
- Shell history analysis
- Multi-profile support
- iCloud sync
- 160+ preset aliases
- 5 built-in themes
- Command palette (Cmd+K)
- Spotlight integration
- Menu bar access

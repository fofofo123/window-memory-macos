# window-memory

> Remembers your window layout for every monitor setup — automatically restores it when you reconnect.

<p align="center">
  <a href="https://fofofo123.github.io/window-memory/">
    <img src="https://img.shields.io/badge/Install-Open%20guide-0071e3?style=for-the-badge&logo=apple&logoColor=white" alt="Install — open installation guide" />
  </a>
</p>

---

## The problem

Every time you disconnect your external monitor and reconnect it, macOS forgets where your windows were. You spend 2–3 minutes manually repositioning everything. Again.

## What this does

window-memory saves your window layout per monitor configuration and restores it automatically when that configuration is detected again.

- Works with 1, 2, or 3+ monitor setups
- Saves layouts per app, not globally
- Runs silently in the menu bar
- No cloud, no account, no telemetry

## Requirements

- macOS 13 Ventura or later
- Apple Silicon or Intel

## How it works

1. Connect your monitors
2. Arrange windows the way you like
3. window-memory saves the layout automatically
4. Disconnect and reconnect — layout is restored

You can also save manually via the menu bar icon or the keyboard shortcut ⌘⇧S.

## Menu bar

| Action | Description |
|--------|-------------|
| Save layout | Saves current window positions for this monitor config |
| Restore layout | Manually triggers restore |
| Preferences | Configure ignored apps, shortcut, launch at login |

## Configuration

Preferences are stored in ~/.config/window-memory/config.json.

{
  "launch_at_login": true,
  "auto_restore": true,
  "ignored_apps": ["Finder", "Safari"],
  "shortcut": "cmd+shift+s"
}

## Privacy

All data is stored locally on your machine. No analytics, no network requests.

## Contributing

Pull requests are welcome. For major changes, please open an issue first.
cd window-memory
open window-memory.xcodeproj

## License

MIT

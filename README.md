# QNode Controller Plugin for the Q-SYS® Ecosystem

The official Q-SYS Designer® software plugin for QNode™ touchscreen panels by MyQuan™.

## What It Does

The QNode Controller plugin connects Q-SYS® Designer software to QNode hardware over TCP. From a single plugin instance, you can:

- **Auto-discover QNode devices** on the network — no manual IP entry needed
- **Browse and deploy Q-SYS UCI™ layouts** from a dropdown of all available UCIs on your Core
- **Use UCI tokens** for layouts that require authentication bypass
- **Control serial devices** via built-in RS232 and RS485
- **Trigger relays** and digital outputs
- **Set LED ring color** from over 4,000 colors
- **Manage display settings** including brightness, sleep/wake, and screen timeout
- **Monitor device status** including connection state and firmware version
- **Detect motion** via QSense for automation triggers

## Supported Hardware

| Device | Display | Resolution |
|--------|---------|------------|
| QNode 10 | 10.1" IPS | 1280x800 |
| QNode 15 | 15.6" IPS | 1920x1080 |

All QNode panels use the same plugin. One plugin instance per panel.

## Installation

Download the latest `.qplugx` file from the [Releases](https://github.com/MyQuanDev/QNodeControllerPlugin/releases) page.

**Option A — Double-click (recommended):**
1. Double-click the downloaded `.qplugx` file — Q-SYS Designer software will install it automatically
2. Restart Q-SYS Designer software if it was already open

**Option B — Manual install:**
1. Copy the `.qplugx` file to your Q-SYS Designer plugin directory:
   - **Windows**: `%USERPROFILE%\Documents\QSC\Q-Sys Designer\Plugins\`
   - **macOS**: `~/Documents/QSC/Q-Sys Designer/Plugins/`
2. Restart Q-SYS Designer software

The plugin appears in the schematic component list under **MyQuan**.

## Quick Start

1. Add a **QNode Controller** component to your Q-SYS Designer schematic
2. Your QNode panel appears automatically in the **Device** dropdown — select it and the plugin connects
3. Choose a Q-SYS UCI layout from the **UCI** dropdown — it auto-deploys to the panel
4. Configure serial ports, relays, and other I/O as needed from the plugin tabs

No IP addresses to look up. No UCI tokens to copy. Just pick your device and pick your layout.

### Advanced: UCI Token Mode

For Q-SYS UCI layouts that use PIN authentication, set the **UCI Mode** property to **Token** in Q-SYS Designer. This lets you enter a UCI token directly, bypassing the PIN prompt on the panel.

## Plugin Tabs

| Tab | Purpose |
|-----|---------|
| UCI | Auto-discover and deploy Q-SYS UCI layouts, or enter a token manually |
| LED | Set LED ring color with presets or custom RGB |
| Triggers | Control relays, digital outputs, and automation |
| Serial | Configure and send/receive RS232 and RS485 data |
| Settings | Display brightness, sleep timeout, firmware info, reboot |

## Requirements

- Q-SYS Designer software 9.x or later
- Q-SYS Core processor on the same network as the QNode panel
- QNode panel running MyQuan OS

## Documentation

- [QNode 10 Product Page](https://myquan.us/qnode-10.html)
- [QNode 15 Product Page](https://myquan.us/qnode-15.html)
- [MyQuan Website](https://myquan.us)

## Support

For technical support, sales inquiries, or feature requests:
- **Website**: [myquan.us/contact](https://myquan.us/contact.html)
- **Email**: support@myquan.us

## License

Copyright 2026 StealthTech Custom Solutions LLC. All rights reserved.

This plugin is provided free of charge for use with QNode hardware. Redistribution, modification, or reverse engineering is prohibited. See [LICENSE](LICENSE) for details.

---

<sub>Q-SYS and Q-SYS Designer are registered trademarks of QSC, LLC in the U.S. Patent and Trademark Office and other countries. Q-SYS UCI is a trademark of QSC, LLC. MyQuan and QNode are trademarks of StealthTech Custom Solutions LLC.</sub>

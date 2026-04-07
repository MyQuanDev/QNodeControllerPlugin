# Changelog

All notable changes to the QNode Controller plugin will be documented in this file.

## [4.1.6] - 2026-04-07

### Highlights

**Zero-configuration setup.** QNode panels are automatically discovered on the network and appear in a dropdown — no IP addresses to type. All available Q-SYS UCI layouts on the Core are listed in a second dropdown — no tokens to copy. Select your device, select your layout, done.

### New Features

- **Auto-discovery of QNode devices** — panels broadcast their presence on the network. Available devices appear in the plugin's Device dropdown automatically.
- **Auto-discovery of Q-SYS UCI layouts** — all UCIs on the connected Core are fetched and listed by name in a UCI dropdown. Select one to deploy it instantly.
- **UCI Mode property** — choose between Browse mode (dropdown selection) and Token mode (manual entry) at design time. Token mode is useful for Q-SYS UCIs with PIN authentication, where a token bypasses the PIN prompt.
- **Live device rename** — changing a panel's name in QNode settings updates the plugin display immediately, whether the panel is connected or not.

### Under the Hood

- Panels only broadcast when available (not connected to a plugin), preventing multiple plugin instances from connecting to the same panel
- Sequence-numbered discovery packets prevent stale data from network jitter
- UCI ZIP download falls back to direct Core path when the API endpoint is unavailable
- Discovery socket binds to NIC broadcast address for reliable reception on Q-SYS Core hardware
- Hostname resolution via discovery table — manual hostname entry is resolved locally without requiring mDNS

## [4.0.4] - 2026-03-30

### Changed
- Rebranded from QuanNode to QNode Controller

### Features
- Multi-page Q-SYS UCI layout support with tab bar navigation
- Navigation button page switching
- Polygon shape rendering and hit testing
- Z-order hit testing (topmost control wins)
- Real-time button state updates across all pages
- Layer transition handling on page switch
- Serial TX/RX bidirectional communication
- Motion detection via QSense
- LED ring control with 4,096 color combinations
- Relay and digital output control
- Display brightness and sleep timeout management

## [4.0.3] - 2026-03-28

- Initial plugin release

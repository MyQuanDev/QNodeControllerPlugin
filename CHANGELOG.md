# Changelog

All notable changes to the QNode Controller plugin will be documented in this file.

## [4.1.6] - 2026-04-07

### Added
- **Auto-discovery of QNode devices** — panels broadcast their presence on the network and appear in a dropdown. No manual IP entry needed. Select a device and the plugin connects automatically.
- **Auto-discovery of Q-SYS UCI layouts** — all available UCIs on the Core are listed in a dropdown. Pick one and it deploys to the panel instantly.
- **UCI Mode property** — choose between Browse (dropdown selection) and Token (manual entry) in Q-SYS Designer. Token mode is useful for UCIs with PIN authentication.
- **Live device rename** — changing a panel's name in QNode settings updates the plugin immediately, whether connected or not.
- **Sequence-numbered discovery** — prevents stale network packets from overwriting current device information.

### Changed
- Device discovery uses subnet broadcast binding for reliable operation on Q-SYS Core hardware
- QNode panels only broadcast when available (not connected to a plugin), preventing duplicate connections
- UCI downloads fall back to direct Core path if API endpoint is unavailable

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

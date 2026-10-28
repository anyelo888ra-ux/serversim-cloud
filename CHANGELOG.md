# Changelog

## Alpha v0.00.3 — 2026-10-28

### Fixed
- The dashboard Create server shortcut now opens the server creation dialog directly.
- The metric refresh setting now changes the actual refresh interval.
- Malformed saved settings no longer prevent the app from initializing.
- Settings save failures now display a user-facing message.

### Updated
- App title and metadata to Alpha v0.00.3.
- Export filename to identify Alpha v0.00.3.
- Documented the planned mobile/desktop detection idea for Beta v0.09 and added instructions for requesting a Wayback Machine snapshot.

### Verification notes
- Source-level checks confirmed the version metadata, navigation shortcut, refresh interval wiring, and settings error handling are present.
- Browser interaction tests and a live Vercel deployment check have not yet been performed.



All notable changes to ServerSim Cloud are documented here.

## Alpha v0.00.2 — 2026-10-28

### Added
- Import local demo configuration from a JSON file.
- Versioned JSON exports named `serversim-cloud-alpha-v0.00.2.json`.
- Additional simulated terminal commands: `history`, `who`, `hostnamectl`, `ip route`, and `systemctl list-units`.

### Improved
- Updated app title and metadata to Alpha v0.00.2.
- Improved terminal help and made command history available during the current page session.
- Added basic validation for imported JSON structure, file size, and record counts.
- Updated README and release documentation.

### Notes and limitations
- Server states, resource metrics, networking, and terminal output remain simulations stored in the current browser.
- Importing a configuration replaces the current local demo state after confirmation. Export a backup first if you want to preserve it.
- SSH from Windows CMD/PowerShell is not implemented in this Alpha; it remains a potential v1.0.0 goal.
- No real cloud instances, shell commands, ports, databases, or game servers are created.


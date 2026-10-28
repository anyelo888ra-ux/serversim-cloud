# Changelog

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


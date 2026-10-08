# Changelog

All notable changes to this extension will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project uses [Semantic Versioning](https://semver.org/).

## [Unreleased]

### Added

- Added highlighting for the `default` keyword.
- Added highlighting for `flow record`, `flow exporter`, and `flow monitor` names.

### Changed

- Changed highlighting for `tacacs server` commands.
- Changed highlighting for `aaa group server` commands.
- Changed highlighting for `radius server` commands.
- Changed highlighting for `aaa authentication`, `aaa authorization`, and `aaa accounting` commands.
- Changed highlighting for standard and extended access lists.
- Changed highlighting for class maps.
- Changed highlighting for policy maps.
- Changed highlighting for numbered access lists.
- Changed highlighting for `device-sensor` commands.
- Changed highlighting for `access-session` commands.
- Changed highlighting for `device-tracking` commands.
- Changed highlighting for interface templates.
- Changed highlighting for NetFlow.
- Changed highlighting for `control-plane` commands.
- Changed highlighting for `archive` commands.
- Changed highlighting for IP SLA.
- Changed highlighting for `ip dhcp pool` commands.

### Fixed

- Fixed incorrect highlighting for `configure terminal` commands.
- Fixed missing highlighting for `copy` commands.

## [0.2.5] - 2026-09-27

### Added

- Added highlighting for URLs.
- Added highlighting for `crypto isakmp` and `crypto ikev2` commands.
- Added highlighting for key chains.
- Added highlighting for keys in `username` commands.
- Added highlighting for keys in `enable secret` commands.

### Changed

- Changed highlighting of crypto key labels.

### Fixed

- Fixed missing highlighting for crypto key configurations without labels.

## [0.2.4] - 2026-09-13

### Added

- Added highlighting for IP version keywords in any command.
- Added highlighting for VRF usage in `router ospf` commands.
- Added highlighting for VRF usage in `router eigrp` commands.

### Changed

- Changed VRF command highlighting.
- Changed highlighting for `ip route vrf` commands.
- Changed interface highlighting rules.

### Fixed

- Fixed incorrect highlighting for `ip tacacs` commands.
- Fixed missing highlighting for some `router eigrp` commands.
- Fixed issue where 25G interfaces would not highlight.

## [0.2.3] - 2026-08-17

### Added

- Added highlighting rules for various IP commands.
- Added highlighting for various logging commands.
- Added highlighting for crypto key labels.

### Changed

- Changed highlighting rules for physical interfaces.
- Changed highlighting for storage commands to include highlighting the directory.
- Changed highlighting rules for negation (`no`, `shut`, and `shutdown`).

### Fixed

- Fixed bug causing physical interfaces to not highlight under certain conditions.
- Fixed incorrect highlighting for some interface ranges.
- Fixed bug causing subinterfaces to not highlight properly.

## [0.2.2] - 2026-07-20

### Added

- Added highlighting rule for storage commands.
- Added highlighting rule for interface ACL access-groups.
- Added highlighting for interface NetFlow monitors.
- Added highlighting rule for interface channel-groups.
- Added highlighting rule to capture CIDR notation at the end of IP addresses.

### Fixed

- Fixed bug causing interface ranges to not highlight properly.
- Fixed incorrect highlighting for `configure terminal` and `configure confirm` commands.

### Changed

- Changed VLAN highlighting to include IDs and ranges, such as `vlan 10,20-25,30`.

## [0.2.1] - 2026-07-20

### Added

- Added highlighting for Jinja2 variables.
- Added highlighting for Jinja2 loops and conditionals.
- Added highlighting for `errdisable recovery` commands.
- Added highlighting for `device-sensor` commands.
- Added highlighting for device tracking.
- Added highlighting for `access-session` commands.
- Added highlighting for `aaa server` commands.
- Added highlighting for `copy` commands.
- Added highlighting for `write memory` commands.
- Added highlighting for `configure` commands.

### Fixed

- Removed highlighting of `vlan-id` from the VLAN context.
- Fixed username patterns that were not being caught.
- Fixed missing highlighting for some AAA commands.
- Fixed hostname highlighting when Jinja2 syntax is present.
- Fixed incorrect Jinja2 highlighting following `description`.

## [0.2.0] - 2026-07-20

### Fixed

- Refactored internal matching schemas.

## [0.1.1] - 2026-07-19

### Added

- Added rules for highlighting policy-map names.
- Added rules for highlighting class-maps.
- Added rules for highlighting service-templates.

### Fixed

- Changed `remark` highlighting to apply only to the remark text.

## [0.1.0] - 2026-07-18

### Added

- Initial preview release of Cisco IOS and IOS XE syntax highlighting.
- Highlighting for common interface, routing, AAA, ACL, VLAN, logging, service, and system configuration constructs.
- Highlighting for IPv4 addresses and common interface names.
- Emphasis for operationally significant commands including `no`, `shutdown`, `permit`, and `deny`.
- Cisco `!` comment highlighting.
- Full-line Jinja2 comment highlighting for Ansible-oriented configuration templates.
- Language registration for `.ios`, `.iosxe`, and `.cisco` files.

### Known limitations

- Coverage is incomplete and focuses on canonical command forms plus selected common abbreviations.
- The extension provides syntax highlighting only; it does not validate configuration correctness.

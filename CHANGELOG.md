# Changelog

All notable changes to this extension will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project uses [Semantic Versioning](https://semver.org/).

## [Unreleased]

### Added
- v0.2.1 Added highlighting for jinja2 variables.
- v0.2.1 Added highlighting for jinja2 loops and conditionals.
- v0.2.1 Added highlighting for errdisable recovery.
- v0.2.1 Added highlighting for device-sensor.
- v0.2.1 Added highlighting for device-tracker.
- v0.2.1 Added highlighting for access-session.
- v0.2.1 Added highlighting for aaa server.

### Fixed
- v0.2.1 Removed highlighting of vlan-id from vlan context.
- v0.2.1 Fixed username patterns that were not being caught.

## [0.2.0] - 2026-07-20

### Fixed
- v0.2.0 Refactored internal matching schemas.

## [0.1.1] - 2026-07-19

### Added
- v0.1.1 Added rules for highlighting policy-map names.
- v0.1.1 Added rules for highlighting class-maps.
- v0.1.1 Added rules for highlighting service-templates.


### Fixed
- v0.1.1 Removed highlighting from remark keyword to only highlight text.

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
- Jinja2 support is currently limited to full-line comments.

[Unreleased]: https://github.com/buildsthenetwork/cisco-ios-xe-parser/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/buildsthenetwork/cisco-ios-xe-parser/releases/tag/v0.1.0

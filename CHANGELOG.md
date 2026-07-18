# Changelog

All notable changes to this extension will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project uses [Semantic Versioning](https://semver.org/).

## [Unreleased]

### Added

- Additional syntax coverage and refinements will be documented here before the next release.

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

# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

### Added

- `ROADMAP.md` — consolidated view of proposed vs. completed work.

### Changed

### Fixed

- `--json-output` and `--csv` no longer write the progress spinner or status
  prose to stdout. Machine-readable output now goes to stdout and human-facing
  messages to stderr, so the documented `gfi search --json-output | jq ...`
  pipeline works unfiltered.
- An empty result set is now valid in machine formats: `--json-output` prints
  `[]` and `--csv` prints just the header row, instead of a sentence that broke
  the consumer's parser.

## [Initial Release]

- Initial project release

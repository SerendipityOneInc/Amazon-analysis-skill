# Changelog

All notable changes to this project will be documented in this file.

## [1.2.2] - 2026-03-20

### Fixed
- Fixed potential API key exposure in example configurations
- Removed hardcoded endpoint URLs from skill documentation

### Changed
- Rewrote `references/` files for both skills with improved field descriptions and usage examples
- Improved SKILL.md SEO: clearer descriptions for better agent intent matching

## [1.2.1] - 2026-03-18

### Changed
- Updated `amazon-analysis` skill scenarios with more realistic evaluation criteria
- Improved pricing strategy reference with profit margin calculation examples

## [1.2.0] - 2026-03-18

### Added
- Published `amazon-analysis` skill to ClawHub (`npx clawhub install Amazon-analysis-skill`)
- Added `apiclaw` general skill — lightweight overview of all 6 API endpoints

## [1.0.0] - 2026-03-13

### Added
- Initial release with two skills: `apiclaw` (general) and `amazon-analysis` (deep)
- CLI tool (`apiclaw.py`) with 8 subcommands and 14 preset search modes
- Full API reference documentation covering all endpoints and response fields
- 7 scenario reference files: composite, evaluation, pricing, operations, expansion, listing, and market monitoring

# Changelog

All notable changes to this project will be documented in this file.

## [1.1.3] — 2026-03-20

### amazon-analysis
- Fixed potential API key exposure risk in example configurations
- Removed hardcoded endpoint URLs from skill documentation
- Rewrote all reference files with improved field descriptions and usage examples
- Improved SKILL.md descriptions for better agent intent matching
- Enforced mandatory API usage tracking in output
- Enforced mandatory Data Source block in Full Mode output
- Added mandatory pre-execution checklist for Full Mode
- Optimized name and description for search discoverability

## [1.1.2] — 2026-03-18

### amazon-analysis
- **Credits Tracking**: API responses now include `creditsConsumed` and `creditsRemaining`
- **Realtime Data Supplementation**: automatically calls `realtime/product` for top 3-5 ASINs in Full mode
- **Reviews/Analyze Endpoint**: new `analyze` command for AI-powered review analysis (11 dimensions)
- **New Scenario 4.6**: Category Consumer Insights
- **Breaking**: `review` → `rating` rename across fields, filters, and CLI args
- **Breaking**: `topReviews` removed from `realtime/product` (use `reviews/analyze`)
- 6 new market response fields for new product metrics
- Slimmed SKILL.md from 448 → 417 lines

### apiclaw v1.0.0
- Initial release of general skill — platform overview, 6 API endpoints

## [1.1.1] — 2026-03-16

### amazon-analysis
- Improved credential handling security: require user confirmation before writing to config.json
- Use ClawHub standard metadata format for credential declaration
- Emphasize environment variable as preferred credential method

## [1.1.0] — 2026-03-16

### amazon-analysis
- **Security**: removed API key logging, added SECURITY.md
- **8 Documentation Fixes**: interface data differences, API call ordering, null fallbacks
- **New**: Listing Optimization Module (8.1 Analysis, 8.2 Copy Generation, 8.3 Diagnosis)
- **6 Mode Corrections**: beginner, long-tail, new-release, fbm-friendly, speculative, top-bsr
- **New CLI Parameters**: `--keyword-match-type`, `--bsr-min/max`, `--seller-count-min/max`, etc.

## [1.0.0] — 2026-03-13

### amazon-analysis
- Initial release with full Amazon seller analytics skill
- CLI tool (`apiclaw.py`) with 8 subcommands and 14 preset search modes
- Full API reference documentation
- 7 scenario reference files

---

### Repo Maintenance (not versioned)

**2026-03-25**
- Fixed CI markdown link check failure
- Added `README.zh-CN.md` with language switcher
- Updated repo description to match official website positioning

**2026-03-23**
- Restructured repo: added general `apiclaw/` skill, moved amazon-analysis to subdirectory
- Added LICENSE (MIT), CONTRIBUTING.md, CODE_OF_CONDUCT.md, Issue Templates, PR template
- Added CI workflow (CLI smoke test + markdown link check)
- Rewrote README.md with badges, Quick Start, API examples

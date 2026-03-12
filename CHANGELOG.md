# Changelog

All notable changes to this project will be documented in this file.

## 1.0.4 - 2026-02-21

- Added `product_images` fallbacks when `profile_image_url` is missing, so artist thumbnails still resolve more reliably.

## 1.0.3 - 2026-02-21

- Switched scraper settings to Kodi legacy format to restore editable settings dialogs.

## 1.0.2 - 2026-02-21

- Fixed Kodi settings parsing by adding explicit `<control>` definitions for all scraper settings.

## 1.0.1 - 2026-02-21

- Simplified the debug workflow with `tools/debug_audible_scraper.py` in the original monorepo.
- Added addon settings scaffolding.
- Added German and English language files.
- Prepared community translation interfaces with `strings.pot` and `resources/i18n/README.md`.

## 1.0.0 - 2026-02-21

- Added the first installable Audible artist scraper based on the Audible API mapping from the Mp3tag source package.
- Added repository packaging and index integration for the Kodi repo.

# Changelog

All notable changes to this project will be documented in this file.

## 1.0.7 - 2026-03-15

- Reduced artist search results to one stable Audible contributor match per lookup, preventing repeated duplicate artist rows in Kodi.
- Changed artist artwork output to explicit `thumb` entries with `aspect` and `preview` attributes for better Kodi artwork pickup.

## 1.0.6 - 2026-03-15

- Reworked artist search extraction to prefer stable Audible contributor authors instead of fragile product-level fallbacks that could resolve to the wrong person.
- Removed narrator pseudo-results from the XML scraper because Audible product search cannot reliably map them back to one correct artist profile or image.
- Removed the unused debug setting from the addon settings because the XML scraper has no runtime logging hook behind it.

## 1.0.5 - 2026-03-15

- Deduplicated repeated author and narrator search results extracted from Audible product matches.
- Tightened artist album extraction so titles and years no longer bleed across adjacent product objects.
- Kept contributor detail lookups intact for author biographies and profile images such as Aimée Carter.

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

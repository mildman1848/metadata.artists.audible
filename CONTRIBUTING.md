# Contributing to metadata.artists.audible

## Before opening a pull request

- Keep changes focused on the Audible artist scraper or its release automation.
- Follow the PR template.
- Link the related issue when applicable with `closes #<number>`.
- Update `README.md`, `CHANGELOG.md` or localization/docs when behavior changes.
- If you touch publishing logic, verify both this source repo and the `mildman1848.github.io` publish flow.

## Files of interest

| File                                    | Purpose                                           |
| --------------------------------------- | ------------------------------------------------- |
| `metadata.artists.audible/`             | Kodi scraper addon payload                        |
| `metadata.artists.audible/audible.xml`  | Kodi scraper URL/result/detail mapping            |
| `metadata.artists.audible/resources/`   | Settings, i18n files and translations             |
| `scripts/build_release.py`              | Builds the addon ZIP                              |
| `scripts/publish_to_repo.py`            | Publishes the addon into the Kodi repository repo |
| `.github/workflows/release-publish.yml` | Cross-repo release publishing                     |

## Local validation

- `python3 -m py_compile $(find . -path './.git' -prune -o -path './node_modules' -prune -o -path './dist' -prune -o -path '*/__pycache__/*' -prune -o -name '*.py' -print)`
- `xmllint --noout metadata.artists.audible/addon.xml metadata.artists.audible/audible.xml metadata.artists.audible/resources/settings.xml`
- `python3 scripts/build_release.py`
- `python3 scripts/publish_to_repo.py --publish-repo /path/to/mildman1848.github.io`

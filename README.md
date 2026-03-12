# metadata.artists.audible

Kodi-Metadaten-Scraper für Autoren- und Erzählerdaten aus der Audible Catalog API.

## Struktur

- `metadata.artists.audible/`: installierbares Kodi-Addon
- `scripts/build_release.py`: erzeugt das Release-ZIP unter `dist/`
- `scripts/publish_to_repo.py`: publiziert das Addon nach `mildman1848.github.io`
- `.github/workflows/release-publish.yml`: veröffentlicht nach einem GitHub-Release automatisch in die Kodi-Repo

## Repository-Hygiene

Das Repo enthält dieselbe Grundausstattung wie die anderen eigenständigen Addon-Repos:

- `CHANGELOG.md`, `SECURITY.md`, `CONTRIBUTING.md`
- Issue- und PR-Templates unter `.github/`
- `Dependabot`, `CI`, `CodeQL`, `Security`, `Greetings` und `Stale` Workflows
- Prettier-, Git- und Editor-Konfiguration für konsistente Änderungen

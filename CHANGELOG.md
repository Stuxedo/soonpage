# Changelog

All notable changes to Coming Soon Page are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/) (MAJOR.MINOR.PATCH).

## v1.1.2

### Removed

- The "A Stux.Cloud Service" credit link &mdash; Stux.Cloud and Stuxedo are instances, not services, so they don't get a service/project credit badge

## v1.1.1

### Changed

- Heading now reads "This service/instance/project/website", since this page is reused across any of those, not just a website

## v1.1.0

### Added

- Self-hosted Exo 2, Barlow and Inter font files under `assets/fonts/`, replacing the Google Fonts CDN link
- A "Boring Legal Stuff" legal hub (`legal.html` + `legal/`: privacy, terms, cookies, imprint, disclaimer, opt-out)
- `changelog.html`, which fetches and renders `CHANGELOG.md` at runtime
- A version indicator in the footer, fetched live from `VERSION.md`
- Cross-origin `postMessage` title sync, so a page embedding this one in an iframe can mirror this page's `<title>`
- `dev-server.sh` / `dev-server.bat` for local previewing
- A custom `404.html` error page

### Changed

- General contact switched from `support@stuxedo.com` to `hello@stuxedo.com`

## v1.0.3

### Fixed
- `README.md` said Stuxedo is "a part of the Stux.Group brand" directly — the actual chain is Stuxedo → Stux.Cloud → Stux Group Ltd. Corrected to name Stux.Cloud as the direct operator, with Stux Group Ltd's full registration details.
### Added
- "A Stux.Cloud Service" credit (linking to `https://services.stux.cloud`) next to the "Powered by Stuxedo" badge.

## v1.0.2

### Fixed
- `README.md`'s Stux.Group brand icon URL had a leftover duplicated `/global/` path segment (`global.media.stux.group/global/icon.png`) — corrected to `https://global.media.stux.group/icon.png`

## v1.0.1

### Changed
- `README.md`'s footer brand-attribution block updated to the new format (Built & Maintained by Stuxedo / Stuxedo is a part of the Stux.Group brand of businesses), replacing the older disclaimer. No "Hosted by" clause here since Stuxedo is the hosting brand itself; the redundant separate "Made by Stuxedo" line was also removed since the new footer already covers that

## v1.0.0

### Added
- `VERSION.md` and this `CHANGELOG.md`, versioning the repo for the first time
- `CONTRIBUTING.md`
- `commit.sh` / `commit.bat` — commit + tag scripts that read the release version from `VERSION.md`

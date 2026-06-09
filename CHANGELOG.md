# Changelog

This document records notable changes made to the Rotary Club of Stevenage Grange website (sgrc.org.uk). The format is loosely based on *Keep a Changelog*.

## Background

The website runs on WordPress using the Astra theme and Elementor. During the course of maintaining the site, it became clear that not all changes are captured in Git.

Two types of updates have been involved:

* **`[code]` Repository-managed changes.** These include custom CSS contained in `custom.css` and JavaScript added through the Head & Footer plugin. These changes form part of the codebase and appear in the commit history.

* **`[config]` WordPress-managed changes.** These include Elementor content edits, page updates, navigation changes, and plugin settings. As these are stored within the WordPress database, they do not automatically appear in the repository history.

The distinction between these categories provides a more complete picture of the work carried out on the website.

---

## [In Progress]

* Investigation into the black-circle Elementor icons displayed on the homepage. Possible causes I observed include the Font Awesome 4 to 5 migration (`[config]`, Elementor Settings → Advanced) or outdated cached CSS (`[code]`/cache). The root cause is yet to be confirmed.

* Verification of the updated Hero "Join Us" button linking to `/join-us/`, including confirmation of the page slug and cache refresh.

## 2006-05-31

### Changed

* `[config]` Updated the homepage Hero CTA by changing the "Join Us" button link from the placeholder `#` to `/join-us/`.

## 2026-05-30

### Added

* `[code]` Implemented client-side validation for the contact form, including an on-submit success message.

* `[config]` Introduced a "Get Involved" dropdown navigation menu containing four active links.

### Changed

* `[code]` Adjusted the header height to 180px and resized the logo to 160px.

### Fixed

* `[config]` Corrected the homepage configuration so that it loads from the site root.

---

## Notes

Entries have been grouped under **Added**, **Changed**, **Fixed**, and **Removed**, with each item identified as either `[code]` or `[config]` to distinguish between repository-managed and WordPress-managed changes.

# Starquix

A visual editor for [Astro](https://astro.build) websites. You build pages on a canvas, like in a design tool, and every change is written as real code to an Astro folder on your Mac.

**[Download for Mac](https://github.com/Mayhopar/Starquix-releases/releases/latest)** — macOS 13 or later, Apple Silicon.

[Why it exists, with a demo video →](https://mayhopar.com/blog/introducing-starquix/)

## What it does

- Visual editing of real Astro files, styled with Tailwind
- Content collections for blogs, and SEO settings
- A terminal where you can run a coding agent, and an AI chat that takes your own API key
- Publishing to Cloudflare, GitHub Pages, Netlify and Vercel

## Install

1. Download `Starquix-<version>-arm64.dmg` from the [latest release](https://github.com/Mayhopar/Starquix-releases/releases/latest).
2. Open it and drag Starquix to Applications.

The app is signed with an Apple Developer ID and notarized by Apple.

## Update

Starquix does not update itself yet. Download the newer dmg and replace the app in Applications. Your projects live in `~/Starquix` and are not touched.

To hear about new versions, click **Watch → Custom → Releases** at the top of this page.

## Verify a download

```sh
shasum -a 256 Starquix-<version>-arm64.dmg
spctl -a -vv -t open --context context:primary-signature Starquix-<version>-arm64.dmg
```

The first line must match the SHA-256 in the release notes. The second must say `accepted`, `source=Notarized Developer ID` and `origin=Developer ID Application: Oleg Maykhopar (67L4BCPLP8)`.

## Bugs and ideas

[Open an issue](https://github.com/Mayhopar/Starquix-releases/issues/new/choose). For a security problem, [report it privately](https://github.com/Mayhopar/Starquix-releases/security/advisories/new) instead.

## About this repository

It holds the downloads and release notes, not the app's source code. The "Source code" archives that GitHub attaches to every release do not contain the app.

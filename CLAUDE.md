# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

Static GitHub Pages site for **Q Extension** — a landing page and privacy policy for three Chrome extensions by NYAN. Hosted at `quxessdev.org` (set via `CNAME`). No build step, no framework, no dependencies.

## Deployment

Push to `main` — GitHub Pages deploys automatically. There is no build, compile, or preview step. Changes are live within ~1 minute of pushing.

## File structure

- `index.html` — landing page with extension cards (SnapShot, Save As JPG/PNG, Tab Volume)
- `privacy.html` — privacy policy page
- `icons/` — extension icon PNGs referenced by both HTML files
- `google59bbc55ff7349f1f.html` — Google Search Console verification file, do not delete

## Key facts about the extensions

All three extensions are **completely free**, no license key, no sign-in, no paywall. They work locally with no external server communication.

- **SnapShot** — screenshot capture with annotation ([Chrome Web Store](https://chromewebstore.google.com/detail/snapshot/genafeokeecllomennekdnppfmodfjhh))
- **Save As JPG/PNG** — right-click image conversion ([Chrome Web Store](https://chromewebstore.google.com/detail/save-as-jpgpng/bklacifbkikmemlbcmpnkkmipoifjpko))
- **Tab Volume** — per-tab audio control ([Chrome Web Store](https://chromewebstore.google.com/detail/tab-volume/flegnbbaknaknoghhcaoijfmkofabphg))

## Design system (inline in HTML)

Both pages share the same CSS variables and font stack — all styles are embedded in `<style>` tags, no external stylesheet. Fonts loaded from Google Fonts: `Instrument Serif` (headings), `Geist Mono` (labels/badges), `Outfit` (body). Color palette centers on `--accent: #1d4e36` (dark green).

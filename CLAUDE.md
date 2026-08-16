# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

A single-page professional profile site for Helen T. Qin (TJHSST student — research, competition math/CS, and classics/arts profile), built from her resume.

## Structure

- `index.html` — the site. Self-contained static HTML with an inline `<style>` block; no build step, framework, or dependencies. Open the file directly in a browser to preview.
- `mockups/` — earlier style studies (`journal.html`, `inscription.html`, `scoreboard.html`) explored before `journal.html`'s academic-journal treatment was chosen for the real site. Kept for reference; not deployed.

## Design system (index.html)

- Visual concept: a precision/competition scoreboard — graph-paper grid background, a headline stat strip, tabular data (`table.scores`) with `tabular-nums`. Graphite ink + signal-blue accent palette, both light and dark themes defined via CSS custom properties on `:root` (light default, `@media (prefers-color-scheme: dark)`, and `[data-theme="dark"]`/`[data-theme="light"]` overrides).
- Sections, in order: Research, Publications, Results (STEM/competition placements — AMC/AIME, USACO, USABO, CyberCamp, CyberPatriot), Awards (service, classics, arts — one table with a Category column), Activities, Skills.
- No contact information is listed on the page (deliberate).
- Content is transcribed from her resume; when adding new entries, match the existing card/row/table formatting rather than introducing new patterns.

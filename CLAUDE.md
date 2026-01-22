# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Universal Search is a single-page HTML application that allows users to search multiple search engines simultaneously by opening results in new browser tabs.

## Architecture

Single file (`universal-search.html`) containing:
- **CSS**: CSS custom properties for theming (light/dark mode), responsive grid layout for search engine checkboxes
- **HTML**: Search input, button, categorized engine checkboxes, theme toggle
- **JavaScript**: Engine configuration, localStorage persistence for theme and selected engines, popup handling

## Key Data Structures

- `categories[]`: Array of category objects, each containing `name` and `engines[]`
- `searchEngines`: Flattened array of all engines (derived from categories)
- `defaultEngines[]`: Engine IDs checked by default on first visit

## Adding a New Search Engine

Add to the appropriate category in the `categories` array:
```javascript
{ id: 'unique-id', name: 'Display Name', url: 'https://example.com/search', param: 'q', extra: '&optional=params' }
```

## localStorage Keys

- `theme`: 'light' or 'dark'
- `selectedEngines`: JSON array of selected engine IDs

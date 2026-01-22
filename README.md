# Universal Search

Search multiple search engines simultaneously with a single query. One click opens all your selected engines in new tabs.

![Dark Mode](https://img.shields.io/badge/theme-dark-1a1a1a) ![Light Mode](https://img.shields.io/badge/theme-light-f5f5f5)

## Features

- **Simultaneous Search** - Enter your query once, search everywhere
- **18 Search Engines** - Google, DuckDuckGo, YouTube, Wikipedia, and more
- **Categorized Selection** - Engines organized into General Search, Audiovisual, and Tools
- **Customizable** - Choose which engines to include with checkboxes
- **Dark/Light Theme** - Toggle between themes with one click
- **Remembers Preferences** - Your theme and engine selections are saved locally

## Search Engines

### General Search
Google, DuckDuckGo, Startpage, Wikipedia EN/NL

### Audiovisual
YouTube, Google Images, DuckDuckGo Images, Startpage Images

### Tools
Google Translate, Google Drive, Wolfram Alpha, Google Maps, DuckDuckGo Maps

## Usage

1. Open `universal-search.html` in your browser
2. Select the search engines you want to use
3. Type your search query
4. Click **"search in tabs"** or press Enter
5. All selected engines open in new tabs

## Browser Permissions

The tool needs permission to open multiple tabs. When prompted, allow popups for the page. Most browsers show this option in the address bar when popups are blocked.

## Installation

No installation needed. Just download and open the HTML file in any modern browser.

```
git clone https://github.com/yourusername/universal-search.git
```

Or simply download `universal-search.html` and double-click to open.

## Customization

To add or remove search engines, edit the `categories` array in the JavaScript section:

```javascript
{
  id: 'unique-id',
  name: 'Display Name',
  url: 'https://example.com/search',
  param: 'q',           // query parameter name
  extra: '&type=web'    // optional extra parameters
}
```

## License

MIT

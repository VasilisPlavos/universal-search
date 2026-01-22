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

## Contributing

Contributions are welcome! The easiest way to contribute is by adding new search engines.

### Adding a Search Engine

1. Fork this repository
2. Edit `universal-search.html`
3. Add your engine to the appropriate category in the `categories` array:

```javascript
{
  id: 'unique-id',
  name: 'Display Name',
  url: 'https://example.com/search',
  param: 'q',           // query parameter name
  extra: '&type=web'    // optional extra parameters
}
```

4. Test it locally
5. Submit a pull request

### Ideas for New Engines

- ChatGPT, Gemini, Perplexity
- Bing, Yahoo, Brave Search
- Reddit, Twitter/X, LinkedIn
- Amazon, eBay, AliExpress
- GitHub, Stack Overflow
- Spotify, SoundCloud
- IMDb, Rotten Tomatoes
- News sites (Google News, BBC, CNN)

Feel free to suggest new categories too!

## License

MIT

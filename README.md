# Claude-Usage-Insights

A browser extension that shows your Claude.ai usage — session, weekly limits, and usage analytics — right where you're already working, with no separate dashboard to check.

[![Install on Edge Add-ons](https://img.shields.io/badge/Edge-Install-blue)](https://microsoftedge.microsoft.com/addons/detail/bofieddolapfocplbondjcfkgaofdalk)
![License: MIT](https://img.shields.io/badge/license-MIT-green)

<img width="1280" height="800" alt="Claude_Usage_Insights_v2_1280x800" src="https://github.com/user-attachments/assets/43bb4ace-da8c-4e19-8cd3-777b3fb1112d" />


## Why this exists

Most Claude usage extensions only show you a live snapshot — a bar that says how full your session or weekly limit is right now. Claude Usage Insights adds the analytics layer on top: how your usage trends over time, so you can actually plan around your limits instead of just reacting to them when they show up.

## Features

- **Live session usage** — 5-hour rolling window, with reset countdown
- **Live weekly usage** — 7-day window, with reset countdown
- **Usage analytics** — It shows session consumption details, weekly consumption, and usage analytics dashboard available
- Reads usage data the same way claude.ai's own Settings page does — no separate login, no API key
- Works entirely in your browser

## Privacy

- No account, no API key, no sign-up
- No analytics, telemetry, or third-party services
- The extension reads usage data directly from claude.ai using your existing browser session — nothing is sent anywhere else
- We do not save anything, everything happens locally

All processing happens locally in your browser. Full source is in this repo — nothing here is happening that you can't read for yourself.

## Installation

**From the Edge Add-ons store (recommended)**
1. Go to https://microsoftedge.microsoft.com/addons/detail/claude-usage-insights/bofieddolapfocplbondjcfkgaofdalk
2. Click "Get"

**Manual install (for development or before store approval)**
1. Clone this repo: `git clone https://github.com/Tushar-Vishwakarma/Claude-Usage-Insights.git`
2. Open `edge://extensions` (or `chrome://extensions`)
3. Enable **Developer mode** (top right)
4. Click **Load unpacked** and select the cloned folder

## How it works

Claude Usage Insights runs only on `claude.ai`. It reads the same usage numbers shown on the official `claude.ai/settings/usage` page and displays them [inline in the Claude sidebar / as a popup — update to match your actual UI]. No credentials are read or stored — your browser attaches your existing claude.ai session automatically when the extension requests usage data, the same way any page you're logged into works.

## Roadmap

- [ ] Usage history / trend charts
- [ ] Per-model usage breakdown (Opus / Sonnet / Haiku)
- [ ] Custom threshold alerts
- [ ] Multi-account support

## Contributing

Issues and pull requests are welcome. If you're proposing a larger change, open an issue first so we can talk through the approach.

## Disclaimer

This is an independent, open-source project. It is not affiliated with, endorsed by, or a product of Anthropic. "Claude" is a trademark of Anthropic PBC.

## License

MIT — see [LICENSE](LICENSE) for details.

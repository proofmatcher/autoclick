# AutoClick — Antigravity Button Automation

**AutoClick** eliminates the constant interruptions of clicking *Run*, *Accept*, and *Allow* buttons in the Antigravity AI IDE. Once enabled, it monitors your workspace in real time and confirms those prompts automatically — so your agent keeps moving without waiting on you.

---

## How It Works

AutoClick runs a lightweight background service inside Antigravity that polls for actionable UI buttons. When one appears, it clicks it immediately using Antigravity's Commands API and Chrome DevTools Protocol (CDP) injection. You stay in control: pause or resume with a single click from the sidebar.

---

## Features

- **Zero-interrupt agent runs** — Run, Accept, and Allow prompts are handled automatically as they appear
- **Dual-engine clicking** — Commands API handles standard prompts; CDP DOM injection catches edge-case buttons that the API misses
- **Real-time sidebar dashboard** — Live click counter, session stats, and quota tracking without leaving your editor
- **Plan-aware quota enforcement** — Usage limits are tracked server-side and reflected instantly in the sidebar
- **Persistent session state** — AutoClick remembers whether it was running before a window reload and resumes automatically
- **Port auto-detection** — Detects whether Antigravity is running with the debug port and alerts you only when a fix is actually needed
- **Secure API key auth** — Your key is stored locally and never transmitted beyond the AutoClick API

---

## Getting Started

1. Install the extension via VSIX or the Antigravity marketplace
2. Click the AutoClick icon in the Activity Bar to open the sidebar
3. Enter your API key from [autoclick.proofmatcher.com](https://autoclick.proofmatcher.com/account)
4. Press **Start AutoClick** — that's it

For CDP-based clicking to work, Antigravity must be launched with the remote debugging port enabled. The sidebar will guide you through this one-time setup if needed.

---

## Plans

| Plan | Price | Clicks | Devices |
|---|---|---|---|
| Free | Free | 100 clicks / month | 1 |
| Trial | $1 one-time | 1,000 clicks / 7 days | 1 |
| Pro | $9 / month | 10,000 clicks / month | 1 |
| Advanced | $19 / month | 40,000 clicks / month | 2 |
| Unlimited | $30 / month | Unlimited | 5 |
| Advanced Pro | $50 / month | Unlimited | 10 |
| Lifetime | Admin grant | Unlimited forever | Unlimited |

Visit [autoclick.proofmatcher.com/pricing](https://autoclick.proofmatcher.com/pricing) to upgrade.

---

## Requirements

- Antigravity IDE (any recent version)
- An AutoClick API key — get one at [autoclick.proofmatcher.com](https://autoclick.proofmatcher.com)

---

## Extension Settings

| Setting | Default | Description |
|---|---|---|
| `agAutoAccept.pollInterval` | `1500` | Polling interval in milliseconds |
| `agAutoAccept.autoAcceptFileEdits` | `true` | Auto-accept file edits (Accept All) |

---

## Support

- **Website:** [autoclick.proofmatcher.com](https://autoclick.proofmatcher.com)
- **Account / API key:** [autoclick.proofmatcher.com/account](https://autoclick.proofmatcher.com/account)

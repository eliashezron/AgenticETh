# Agentic Eth

Agentic Eth is an on-chain storyteller designed to craft engaging, single-line crypto narratives. Built on the ElizaOS platform, Agentic Eth transforms blockchain data into tweet-length stories (no more than 280 characters) that are insightful, dynamic, and true to the decentralized spirit.

## Features

- **Single-Line Stories:** Every narrative is a single, complete sentence capped at 280 characters.
- **Real-Time Data Integration:** Leverages the CoinMarketCap plugin (and other plugins, like NASA, if needed) to incorporate current crypto and on-chain data.
- **Conversational Tone:** Uses natural language, colloquialisms, and technical insights to make complex blockchain topics accessible.
- **Decentralized Spirit:** Emphasizes authenticity, real-world impact, and technical depth without relying on marketing clichés.

## 🚀 Quick Start

### Prerequisites

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Note for Windows Users:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) is required.

### Use the Starter (Recommended)

```bash
git clone https://github.com/eliashezron/AgenticETh.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

#### Checkout the latest release

```bash
# Clone the repository
git clone https://github.com/eliashezron/AgenticETh.git

# This project iterates fast, so we recommend checking out the latest release
git checkout $(git describe --tags --abbrev=0)
# If the above doesn't checkout the latest release, this should work:
# git checkout $(git describe --tags `git rev-list --tags --max-count=1`)
```

#### Edit the .env file

Copy .env.example to .env and fill in the appropriate values.

```
cp .env.example .env
```

Note: .env is optional. If you're planning to run multiple distinct agents, you can pass secrets through the character JSON

#### Start Agentic Eth

```bash
pnpm i
pnpm build
pnpm start

# The project iterates fast, sometimes you need to clean the project if you are coming back to the project
pnpm clean
```

#### Additional Requirements

You may need to install Sharp. If you see an error when starting up, try installing it with the following command:

```
pnpm install --include=optional sharp
```

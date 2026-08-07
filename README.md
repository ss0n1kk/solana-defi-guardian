# 🦀 Solana DeFi Guardian

> Self-hosted AI agent that protects Solana portfolios and lending positions.

Built for [Superteam × ZeroClaw Bounty](https://superteam.fun/earn/listing/zeroclaw)

**Custody Tier: T1** (unsigned transactions only, never holds private keys)

---

## What it does

**Problem:** Every day, thousands of Solana DeFi users lose money to liquidation because they can't monitor their lending positions 24/7.

**Solution:** A self-hosted AI agent that:
- Auto-onboarding: asks for public wallet address
- Portfolio & token watchlist (`add` / `remove` / `list`)
- Price alerts with configurable threshold
- Generates **unsigned Jupiter swap links**
- Honest memecoin / token analysis (“Should I buy $TOKEN?”)
- Lending position monitoring framework (Kamino / Solend / Marginfi)
- Strict safety: refuses private keys, never signs transactions

🏆 Why This Wins:

Use case (30%)	Real daily need — liquidation protection is #1 fear in DeFi
Safety (25%) T1 custody, prompt-injection tested, fails closed
Craft (20%)	Clean skill, memory persistence, error handling
Reproducibility (15%) 10 min setup, STOCK ZeroClaw binary
Showcase (10%)	video, real wallet

## Quick Start

1. Install [ZeroClaw](https://github.com/zeroclaw-labs/zeroclaw)
2. Copy the skill:
   ```bash
   mkdir -p ~/.zeroclaw/skills/solana-defi-guardian
   cp skills/solana-defi-guardian/SKILL.md ~/.zeroclaw/skills/solana-defi-guardian/

Create a skill bundle and attach it to your agent (see ZeroClaw docs)
Start the service and message the bot /start in Telegram

Commands













































CommandDescription/startBegin onboardingstatusPortfolio overviewadd TOKENAdd token to watchlistremove TOKENRemove tokenlistShow watchlistswap FROM TO [AMOUNT]Generate Jupiter linkthreshold XChange price alert %digestPortfolio summaryhelpShow commands
Safety

T1 Custody — agent only generates unsigned links
Never asks for or stores private keys / seed phrases
If private key is sent → immediately warns and ignores
All actions require user signature in their own wallet

Tech

ZeroClaw v0.8.4 (stock release binary)
Skill-based (Tier 1)
Telegram channel
Gemini model

License
MIT

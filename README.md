<p align="center">
  <img src="https://img.shields.io/badge/Status-Draft%20v0.1-blue?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/Web3-Infrastructure-cyan?style=for-the-badge" alt="Web3">
  <img src="https://img.shields.io/badge/License-For%20Discussion-gray?style=for-the-badge" alt="License">
</p>

<h1 align="center">VELA</h1>
<p align="center"><strong>Borderless Communication. Frictionless Finance.</strong></p>
<p align="center">无国界通讯，无摩擦金融</p>

---

## 📌 What is VELA?

VELA is a conceptual design for a **messaging platform with built-in global payment capabilities** — powered by production-ready Web3 protocols. Users chat and transfer value across borders as naturally as sending a message, with blockchain entirely invisible to the end user.

> *"The next billion people to use Web3 will not know they are using Web3."*

## 📄 Whitepaper

The whitepaper is a single-file interactive HTML document with:

- 🌐 **Bilingual content** (中文 / English)
- 🎨 **Premium dark UI** with glassmorphism, micro-animations, and responsive design
- 📊 **Real market data** sourced from World Bank RPW Q3 2025
- 🏗️ **Technical architecture** with layered system diagram and protocol flow

**➡️ Open `chainlink-whitepaper.html` in any modern browser to view.**

## 🏗️ Technical Architecture

```
┌─────────────────────────────────────────────────────────┐
│  CLIENT        Chat UI │ Wallet UI │ Mini-Apps │ KYC    │
├─────────────────────────────────────────────────────────┤
│  PROTOCOL      Signal Protocol │ ERC-4337 │ CCTP V2    │
├─────────────────────────────────────────────────────────┤
│  INFRA         Base L2 │ USDC Native │ Bundler Node     │
├─────────────────────────────────────────────────────────┤
│  COMPLIANCE    KYC Provider │ AML │ Travel Rule │ FATF  │
└─────────────────────────────────────────────────────────┘
```

| Layer | Technology | Why |
|-------|-----------|-----|
| Settlement | **Base (Coinbase L2)** | Gas < $0.01/tx, enterprise-grade |
| Gas Abstraction | **ERC-4337 Paymaster** | Users hold zero ETH |
| Messaging | **Signal Protocol** | E2E encryption, forward secrecy |
| Identity | **ZK Proofs** | Privacy-preserving verification |
| Cross-chain | **Circle CCTP V2** | Native burn-and-mint, no bridge risk |
| Asset | **USDC (Circle)** | Regulated, 1:1 reserve audited |

## 🔑 Key Design Decisions

### Why Signal Protocol instead of ZK for messaging?
Zero-Knowledge Proofs are **verification protocols** (proving a statement true without revealing data), not encryption protocols. E2E message encryption requires key agreement + Double Ratchet — that's Signal Protocol's core strength. ZK is used for **identity verification and group membership proofs**.

### Why no custom token or ICO?
The business model is based on **verifiable cash flows** (ads, premium subscriptions, platform commissions, enterprise API fees) — not token speculation. Only Circle-issued USDC is used, avoiding reserve management risk and additional regulatory burden.

### Why Base L2 over building a new chain?
Competitive advantage comes from the **UX layer**, not the infrastructure layer. Using battle-tested L2 + Circle CCTP minimizes technical and compliance risk while delivering < $0.01 gas fees.

## 📊 Market Context

| Metric | Value | Source |
|--------|-------|--------|
| Global Remittance Market | **$905B** (2024) | World Bank |
| Global Avg. Remittance Fee | **6.36%** | World Bank RPW Q3 2025 |
| Bank Channel Avg. Fee | **14.99%** | World Bank RPW Q3 2025 |
| VELA Target E2E Fee | **< 1%** | Incl. fiat on/off-ramp |
| VELA Settlement Time | **< 30s** | Base L2 + CCTP V2 |

## 📋 Whitepaper Sections

| # | Section | Description |
|---|---------|-------------|
| 01 | Executive Summary | Product overview with real market data |
| 02 | The Problem | Global pain points with World Bank statistics |
| 03 | The Solution | Core product + "Attention → Finance" insight |
| 04 | Technical Architecture | Layered system, protocol details, transfer flow |
| 05 | Compliance & Regulation | KYC tiers, Travel Rule, MiCA/FinCEN/MAS licensing |
| 06 | Business Model | Revenue projections at 1M MAU baseline |
| 07 | Go-To-Market | 3-phase strategy targeting remittance corridors |
| 08 | Competitive Landscape | vs WeChat, Telegram, PayPal, Circle CPN, SWIFT |
| 09 | Risks & Challenges | 6 core risks with mitigation strategies |
| 10 | Vision | Long-term thesis |

## 🛡️ Compliance Framework

The whitepaper includes a detailed compliance-by-design approach:

- **Tiered KYC/AML** — 3 levels from phone verification to enhanced due diligence
- **FATF Travel Rule** — Full Recommendation 16 compliance via Notabene/Sygna
- **Multi-jurisdiction licensing** — EU (MiCA CASP), US (FinCEN MSB + State MTL), SG (MAS MPI), UAE (VARA)
- **Stablecoin strategy** — USDC only, no self-issued tokens

## 🛠️ Tech Stack (Whitepaper itself)

The whitepaper document is built with:

- Pure **HTML + CSS + JavaScript** (zero dependencies)
- **Google Fonts**: Inter, Space Grotesk, Noto Serif SC
- Scroll-reveal animations via `IntersectionObserver`
- Responsive design (desktop → mobile)
- Dark glassmorphism design system

## 📁 Project Structure

```
.
├── vela-whitepaper.html   # Interactive whitepaper (open in browser)
└── README.md                   # This file
```

## 🚀 Quick Start

```bash
# Simply open in browser
open chainlink-whitepaper.html

# Or serve locally
python -m http.server 8080
# Then visit http://localhost:8080/chainlink-whitepaper.html
```

## 📝 Note

This is a **conceptual whitepaper** created to demonstrate product thinking, technical architecture understanding, and compliance awareness in the Web3 space. It is not affiliated with any existing project or company.

---

<p align="center">
  <strong>VELA</strong> — Draft v0.1 — For Discussion Purposes Only
</p>

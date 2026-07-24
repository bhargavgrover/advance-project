<div align="center">

# 🌍 Advance Project

### Real-time Global Intelligence Dashboard

AI-powered news aggregation, geopolitical monitoring, and infrastructure tracking in a unified situational awareness interface.

[![GitHub stars](https://img.shields.io/github/stars/bhargavgrover/advance-project?style=social)](https://github.com/bhargavgrover/advance-project/stargazers)
[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![npm](https://img.shields.io/npm/v/worldmonitor?logo=npm&label=npm)](https://www.npmjs.com/package/worldmonitor)
[![Last commit](https://img.shields.io/github/last-commit/bhargavgrover/advance-project)](https://github.com/bhargavgrover/advance-project/commits/main)

---

### 🚀 Live Demos

<a href="https://www.worldmonitor.app"><strong>Main Dashboard</strong></a> ·
<a href="https://tech.worldmonitor.app"><strong>Tech Monitor</strong></a> ·
<a href="https://finance.worldmonitor.app"><strong>Finance Radar</strong></a> ·
<a href="https://commodity.worldmonitor.app"><strong>Commodity Tracker</strong></a>

</div>

---

## 📋 Overview

**Advance Project** (formerly World Monitor) is a cutting-edge, real-time global intelligence dashboard designed to aggregate, analyze, and visualize data from hundreds of sources across the globe. Whether you're tracking geopolitical shifts, monitoring financial markets, or keeping an eye on natural disasters, this platform provides a unified operational picture.

Built with a modern tech stack and designed for scale, it serves as both a web application and a native desktop app, with programmatic access via APIs, SDKs, and CLI tools.

---

## ✨ Key Features

- **📰 500+ Curated News Feeds** — Across 15 categories, AI-synthesized into actionable briefs
- **🌐 Dual Map Engine** — 3D globe (globe.gl) and WebGL flat map (deck.gl) with 56+ map layer types
- **🔄 Cross-Stream Correlation** — Military, economic, disaster, and escalation signal convergence
- **📊 Country Instability Index (CII)** — Server-authoritative CII v8 stress scoring for 31 Tier-1 countries
- **💰 Finance Radar** — 29 stock exchanges, commodities, crypto, and 7-signal market composite
- **🤖 Local AI Support** — Run everything with Ollama, no API keys required
- **🎨 6 Site Variants** — From a single codebase (World, Tech, Finance, Commodity, Happy, Energy)
- **💻 Native Desktop App** — Built with Tauri 2 for macOS, Windows, and Linux
- **🌍 25 Languages** — With native-language feeds and RTL support
- **🔌 MCP & REST APIs** — Agent-friendly access with SDKs for Python, Ruby, Go, and Node.js

---

## 🛠️ Tech Stack

| Category | Technologies |
|----------|-------------|
| **Frontend** | Vanilla TypeScript, Vite, globe.gl + Three.js, deck.gl + MapLibre GL |
| **Desktop** | Tauri 2 (Rust) with Node.js sidecar |
| **AI/ML** | Ollama / Groq / OpenRouter, Transformers.js (browser-side) |
| **API Contracts** | Protocol Buffers (281 protos, 35 services) |
| **Deployment** | Vercel Edge Functions (60+), Railway relay, Docker |
| **Caching** | Redis (Upstash), 3-tier cache, CDN, service worker |
| **Database** | Convex (real-time reactive backend) |

---

## 🚀 Quick Start

### Prerequisites

- [Node.js](https://nodejs.org/) (v18+)
- [npm](https://www.npmjs.com/)

### Installation

```bash
# Clone the repository
git clone https://github.com/bhargavgrover/advance-project.git
cd advance-project

# Install dependencies
npm install

# Start development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser. Override the port with `DEV_PORT` in `.env.local`.

### Variant-Specific Development

```bash
npm run dev:tech       # Tech variant
npm run dev:finance    # Finance variant
npm run dev:commodity  # Commodity variant
npm run dev:happy      # Happy variant
npm run dev:energy     # Energy variant
```

---

## 📦 Programmatic Access

Advance Project is built for agents and scripts as well as browsers:

- **MCP Server** — `https://worldmonitor.app/mcp` (Streamable HTTP)
- **REST API** — Base `https://api.worldmonitor.app`
- **CLI** — `npx worldmonitor` or `npm install -g worldmonitor`
- **SDKs** — Python, Ruby, Go (official zero-dependency client libraries)

```bash
# Example: Get risk assessment for a country
npx worldmonitor risk IR --api-key wm_xxx
```

---

## 🐳 Docker Deployment

```bash
docker-compose up -d
```

See the [self-hosting guide](https://www.worldmonitor.app/docs/getting-started) for detailed deployment options.

---

## 📁 Project Structure

```
advance-project/
├── api/              # Vercel Edge Functions (60+ API endpoints)
├── src/              # Frontend source code
├── server/           # Server-side code
├── cli/              # CLI tool source
├── sdk/              # Client SDKs (Python, Ruby, Go)
├── convex/           # Convex backend functions
├── src-tauri/        # Tauri desktop app (Rust)
├── shared/           # Shared utilities and types
├── docs/             # Documentation
├── e2e/              # Playwright end-to-end tests
├── tests/            # Data validation tests
├── deploy/           # Deployment configurations
└── docker/           # Docker setup
```

---

## 🧪 Testing

```bash
# Type checking
npm run typecheck

# Run data tests
npm run test:data

# Run end-to-end tests
npm run test:e2e

# Production build
npm run build
```

---

## 🤝 Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

```bash
# Before submitting a PR
npm run typecheck
npm run build:full
```

---

## 📄 License

**AGPL-3.0-only** — This project is licensed under the GNU Affero General Public License v3.0. See [LICENSE](./LICENSE) for details.

| Use Case | Allowed? |
|----------|----------|
| Personal / Research / Educational | ✅ Yes, under AGPL-3.0 |
| Self-hosted Instance | ✅ Yes, under AGPL-3.0 |
| Fork and Modify | ✅ Yes, share source under AGPL-3.0 |
| Commercial Use / SaaS | ✅ Yes, under AGPL-3.0 |
| Private-source Proprietary Use | ❌ Requires separate license |

---

## 👤 Author

**Bhargav Grover**

<a href="https://github.com/bhargavgrover">
  <img src="https://img.shields.io/badge/GitHub-bhargavgrover-181717?style=for-the-badge&logo=github" alt="GitHub">
</a>

---

## 🙏 Acknowledgments

- Original project by [Elie Habib](https://github.com/koala73)
- [Wingbits](https://wingbits.com) for flight data
- All contributors and open-source maintainers

---

<div align="center">
  <p>
    <a href="https://github.com/bhargavgrover/advance-project/issues">Report Bug</a> ·
    <a href="https://github.com/bhargavgrover/advance-project/issues">Request Feature</a> ·
    <a href="https://github.com/bhargavgrover/advance-project/discussions">Discussions</a>
  </p>
  <p>⭐ Star this repo if you find it useful! ⭐</p>
</div>



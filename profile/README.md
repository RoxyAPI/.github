<a href="https://roxyapi.com">
  <img src="https://raw.githubusercontent.com/RoxyAPI/.github/main/profile/assets/hero.png" alt="RoxyAPI. The data layer for insight, belief, and prediction products. Astrology, Vedic, tarot, numerology, and more behind one API key." width="100%">
</a>

# RoxyAPI

[![Live API](https://img.shields.io/badge/API-Live_playground-1f6feb?style=flat-square&logo=swagger&logoColor=white)](https://roxyapi.com/api-reference)
[![Methodology](https://img.shields.io/badge/Methodology-NASA_JPL_verified-fb923c?style=flat-square)](https://roxyapi.com/methodology)
[![Benchmark](https://img.shields.io/badge/Benchmark-Open_%26_MIT-22c55e?style=flat-square&logo=github&logoColor=white)](https://github.com/RoxyAPI/astrology-api-benchmark)
[![Pricing](https://img.shields.io/badge/Pricing-Plans_%26_quotas-0ea5e9?style=flat-square)](https://roxyapi.com/pricing)
[![Starters](https://img.shields.io/badge/Starters-Open_source-8b5cf6?style=flat-square)](https://roxyapi.com/starters)
[![MCP](https://img.shields.io/badge/MCP-Remote_%26_no_setup-ec4899?style=flat-square)](https://roxyapi.com/docs/mcp)

**Official SDKs**

[![npm](https://img.shields.io/npm/v/@roxyapi/sdk?style=flat-square&logo=npm&label=%40roxyapi%2Fsdk)](https://www.npmjs.com/package/@roxyapi/sdk)
[![PyPI](https://img.shields.io/pypi/v/roxy-sdk?style=flat-square&logo=pypi&logoColor=white&label=roxy-sdk)](https://pypi.org/project/roxy-sdk/)

The data layer for insight, belief, and prediction products.

RoxyAPI is the only multi-domain spiritual intelligence API. 130+ production endpoints across 10 domains behind one API key, with remote MCP servers per product, verified astronomy, and clean commercial licensing. Think of it as the Stripe of insight APIs: AI-native infrastructure for astrology, tarot, numerology, and prediction apps so builders can ship in days instead of months.

Every calculation is rigorously verified against authoritative sources. The proof is public, the breadth is one key, the licensing is clean.

## What RoxyAPI does

One subscription gives builders production-ready access to every major spiritual and prediction domain through a single REST API and a single set of MCP servers. Domains in canonical order:

- **Western astrology**: natal charts, daily horoscopes, weekly and monthly horoscopes, synastry, compatibility scoring, transits, moon phase. Placidus, whole-sign, equal, and Koch house systems.
- **Vedic and KP astrology**: kundli, detailed panchang (rahu kaal, abhijit muhurta, brahma muhurta, choghadiya, hora), Vimshottari dasha (current period and full 120-year timeline), dosha analysis (Manglik, Kaal Sarp, Sade Sati), navamsa, 36-point Ashtakoota Guna Milan compatibility, plus KP sub-lord, sub-sub-lord, and ruling-planet horary. KP is the sharpest technical differentiator versus generic Vedic providers.
- **Numerology**: Life Path, full chart, compatibility, personal year, expression. Pythagorean reduction with master-number (11, 22, 33) and karmic-debt detection.
- **Tarot**: daily card, three-card spread, Celtic Cross, yes-no, love spread, custom draws. Deterministic seeded draws for once-per-day behavior.
- **Biorhythm**: daily, multi-day forecast, compatibility, critical-day alerts. 10 cycle types.
- **I Ching**: 64-hexagram catalog, daily hexagram, three-coin cast with changing lines and resulting hexagram.
- **Crystals**: by zodiac, by chakra, birthstone, free-text search.
- **Dream interpretation**: symbol catalog, daily symbol, structured meanings.
- **Angel numbers**: by exact number, universal lookup with digit-root fallback, daily.
- **Location and timezone resolution** for accurate birth-data inputs (call this first when any chart endpoint needs coordinates).

Every endpoint returns structured JSON, ships rich field descriptions for tool-calling agents, and is callable from REST, the official SDKs, or remote MCP.

## Quick links

| Surface | URL |
|---|---|
| Live API playground | https://roxyapi.com/api-reference |
| Documentation and guides | https://roxyapi.com/docs |
| Pricing | https://roxyapi.com/pricing |
| Methodology and accuracy | https://roxyapi.com/methodology |
| Public benchmark (open, MIT) | https://github.com/RoxyAPI/astrology-api-benchmark |
| Starter templates | https://roxyapi.com/starters |
| OpenAPI specs | https://roxyapi.com/api/v2/openapi.json |
| Agent discovery | https://roxyapi.com/llms.txt |

## Official SDKs

| Language | Package | Repository |
|---|---|---|
| TypeScript | `@roxyapi/sdk` | [RoxyAPI/sdk-typescript](https://github.com/RoxyAPI/sdk-typescript) |
| Python | `roxy-sdk` | [RoxyAPI/sdk-python](https://github.com/RoxyAPI/sdk-python) |
| WordPress plugin | RoxyAPI for WordPress | [RoxyAPI/sdk-wordpress](https://github.com/RoxyAPI/sdk-wordpress) |

Both code SDKs are auto-generated from the OpenAPI specification, so new endpoints land in your IDE the day they ship. Each SDK ships an AGENTS.md so AI coding assistants in Cursor, Claude Code, Copilot, and Windsurf know how to call RoxyAPI without prompt-engineering.

## MCP servers

RoxyAPI was MCP-first from day one. Every product domain ships its own remote Streamable HTTP MCP server. No local processes, no stdio wrappers, no self-hosting. Point Claude Desktop, Cursor, VS Code, Windsurf, or any MCP-compatible client at the URL and it is running in seconds.

| Domain | MCP endpoint |
|---|---|
| Western astrology | `https://roxyapi.com/mcp/astrology` |
| Vedic and KP astrology | `https://roxyapi.com/mcp/vedic-astrology` |
| Numerology | `https://roxyapi.com/mcp/numerology` |
| Tarot | `https://roxyapi.com/mcp/tarot` |
| Biorhythm | `https://roxyapi.com/mcp/biorhythm` |
| I Ching | `https://roxyapi.com/mcp/iching` |
| Crystals | `https://roxyapi.com/mcp/crystals` |
| Dreams | `https://roxyapi.com/mcp/dreams` |
| Angel numbers | `https://roxyapi.com/mcp/angel-numbers` |
| Location and timezone | `https://roxyapi.com/mcp/location` |

The flagship multi-MCP reference integration is [RoxyAPI/astrology-ai-chatbot](https://github.com/RoxyAPI/astrology-ai-chatbot), an MIT-licensed chatbot starter that wires multiple RoxyAPI MCP servers into a single conversational agent.

## Verified accuracy

Astronomy is the one place AI confidently lies. RoxyAPI treats accuracy as the moat.

- Powered by **Roxy Ephemeris**, cross-referenced against **NASA JPL Horizons DE441** as the physics ground truth.
- Vedic and KP outputs cross-referenced against DrikPanchang, onlinejyotish.com, JyotishApp, and timeanddate.com.
- Public methodology with tolerance thresholds and verification tables: [roxyapi.com/methodology](https://roxyapi.com/methodology).
- Public, MIT-licensed benchmark anyone can clone, run, or point at any astrology API: [RoxyAPI/astrology-api-benchmark](https://github.com/RoxyAPI/astrology-api-benchmark). 210 reference planet positions across 21 birth charts, 210 of 210 within tolerance, median deviation 0.27 arcmin.
- No AGPL, no copyleft, no commercial-license entanglements passed to customers. Clean commercial licensing for production use.

## Starter templates

Open-source starters that wrap RoxyAPI into a working app you can fork and ship:

- [astrology-ai-chatbot](https://github.com/RoxyAPI/astrology-ai-chatbot): flagship multi-MCP astrology assistant
- [astrology-starter-app](https://github.com/RoxyAPI/astrology-starter-app): Western astrology baseline
- [vedic-astrology-starter-app](https://github.com/RoxyAPI/vedic-astrology-starter-app): Vedic and KP focused
- [jyotish-vedic-astrology-app](https://github.com/RoxyAPI/jyotish-vedic-astrology-app): Indian-market Jyotish app with Kundli, Panchang, Gun Milan, Dasha
- [numerology-starter-app](https://github.com/RoxyAPI/numerology-starter-app): Life Path, master numbers, karmic debt
- [tarot-starter-app](https://github.com/RoxyAPI/tarot-starter-app): tarot reader with seeded draws
- [dreams-starter-app](https://github.com/RoxyAPI/dreams-starter-app): dream journal with interpretation

## Get started

1. Grab a key at [roxyapi.com/pricing](https://roxyapi.com/pricing). Every plan includes every domain.
2. Try the live playground at [roxyapi.com/api-reference](https://roxyapi.com/api-reference).
3. Install an SDK or point your MCP client at one of the endpoints above.
4. Ship.

## Contact

Questions, integration help, or partnership inquiries: [roxyapi.com/contact](https://roxyapi.com/contact).

Built by [Roxy Labs](https://roxyapi.com). The Stripe of insight APIs.

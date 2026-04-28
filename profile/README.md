# RoxyAPI

The data layer for insight, belief, and prediction products.

RoxyAPI is the only multi-domain spiritual intelligence API. 130+ production endpoints across 10 domains behind one API key, with remote MCP servers per product, verified astronomy, and clean commercial licensing. Think of it as the Stripe of insight APIs: AI-native infrastructure for astrology, tarot, numerology, and prediction apps so builders can ship in days instead of months.

Every calculation is rigorously verified against authoritative sources. The proof is public, the breadth is one key, the licensing is clean.

## What RoxyAPI does

One subscription gives builders production-ready access to every major spiritual and prediction domain through a single REST API and a single set of MCP servers. Domains covered:

- Astrology (Western, Vedic, KP) with birth charts, transits, dashas, panchang, kundli, and synastry
- Numerology (Pythagorean, Chaldean, Life Path, master numbers, karmic debt, personal year)
- Tarot (deck data, daily pulls, spread generators, deterministic seeded draws)
- Daily horoscopes (12 zodiac signs, multi-language)
- Biorhythm (10 cycle types, compatibility, critical-day windows)
- I Ching (64 hexagrams, changing lines, Wilhelm-style interpretation)
- Dream interpretation (symbol library plus structured analysis)
- Crystals (catalog, properties, intentions, chakra mapping)
- Angel numbers (repeating, sequential, mirror, master patterns)
- Location and timezone resolution for accurate birth-data inputs

Every endpoint returns structured JSON, ships rich field descriptions for tool-calling agents, and is callable from REST, the official SDKs, or remote MCP.

## What you can build

- AI astrology and tarot chatbots backed by Claude, GPT, or Gemini
- Birth-chart and kundli generators for matrimonial and dating platforms
- Daily horoscope features embedded in wellness, news, or lifestyle apps
- Numerology and personality apps for self-discovery and onboarding flows
- Dream-journal apps with AI interpretation and pattern tracking
- Spiritual AI agents that reason over birth charts, panchang, dashas, and tarot through MCP tool calls
- White-label insight engines for coaches, astrologers, and content creators

## Quick links

| Surface | URL |
|---|---|
| Live API docs and playground | https://roxyapi.com/docs |
| Pricing | https://roxyapi.com/pricing |
| Methodology and accuracy | https://roxyapi.com/methodology |
| Public benchmark (open, MIT) | https://github.com/RoxyAPI/astrology-api-benchmark |
| Starter templates | https://roxyapi.com/starters |
| OpenAPI specs | https://roxyapi.com/api/v2/openapi.json |
| Agent discovery | https://roxyapi.com/llms.txt |

## Official SDKs

[![npm](https://img.shields.io/npm/v/@roxyapi/sdk?label=npm)](https://www.npmjs.com/package/@roxyapi/sdk)
[![PyPI](https://img.shields.io/pypi/v/roxy-sdk?label=PyPI)](https://pypi.org/project/roxy-sdk/)

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
| Dreams | `https://roxyapi.com/mcp/dreams` |
| Crystals | `https://roxyapi.com/mcp/crystals` |
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
- [astrology-starter-app](https://github.com/RoxyAPI/astrology-starter-app): full astrology app baseline
- [vedic-astrology-starter-app](https://github.com/RoxyAPI/vedic-astrology-starter-app): Vedic and KP focused
- [jyotish-vedic-astrology-app](https://github.com/RoxyAPI/jyotish-vedic-astrology-app): Indian market Jyotish app
- [tarot-starter-app](https://github.com/RoxyAPI/tarot-starter-app): tarot reader with seeded draws
- [numerology-starter-app](https://github.com/RoxyAPI/numerology-starter-app): Life Path, master numbers, karmic debt
- [dreams-starter-app](https://github.com/RoxyAPI/dreams-starter-app): dream journal with interpretation

## Get started

1. Grab a key at [roxyapi.com/pricing](https://roxyapi.com/pricing). Plans run from 5K to 1M requests per month, all 10 domains included.
2. Try the playground at [roxyapi.com/docs](https://roxyapi.com/docs).
3. Install an SDK or point your MCP client at one of the endpoints above.
4. Ship.

## Contact

Questions, integration help, or partnership inquiries: hello@roxyapi.com.

Built by [Roxy Labs](https://roxyapi.com). The Stripe of insight APIs.

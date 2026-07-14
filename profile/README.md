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
[![Packagist](https://img.shields.io/packagist/v/roxyapi/sdk?style=flat-square&logo=packagist&logoColor=white&label=roxyapi%2Fsdk)](https://packagist.org/packages/roxyapi/sdk)
[![NuGet](https://img.shields.io/nuget/v/RoxyApi.Sdk?style=flat-square&logo=nuget&logoColor=white&label=RoxyApi.Sdk)](https://www.nuget.org/packages/RoxyApi.Sdk)
[![Go module](https://img.shields.io/github/v/tag/RoxyAPI/sdk-go?style=flat-square&logo=go&logoColor=white&label=sdk-go)](https://pkg.go.dev/github.com/RoxyAPI/sdk-go)
[![WordPress plugin](https://img.shields.io/wordpress/plugin/v/roxyapi?style=flat-square&logo=wordpress&logoColor=white&label=wordpress.org)](https://wordpress.org/plugins/roxyapi/)

**Drop-in UI**

[![@roxyapi/ui](https://img.shields.io/npm/v/@roxyapi/ui?style=flat-square&logo=webcomponentsdotorg&logoColor=white&label=%40roxyapi%2Fui)](https://www.npmjs.com/package/@roxyapi/ui)
[![@roxyapi/ui-react](https://img.shields.io/npm/v/@roxyapi/ui-react?style=flat-square&logo=react&logoColor=white&label=%40roxyapi%2Fui-react)](https://www.npmjs.com/package/@roxyapi/ui-react)
[![@roxyapi/ui-vue](https://img.shields.io/npm/v/@roxyapi/ui-vue?style=flat-square&logo=vuedotjs&logoColor=white&label=%40roxyapi%2Fui-vue)](https://www.npmjs.com/package/@roxyapi/ui-vue)

The data layer for insight, belief, and prediction products.

RoxyAPI is the only multi-domain spiritual intelligence API. 160+ production endpoints across 12+ genuinely distinct domains behind one API key, with remote MCP servers per product, verified astronomy, and clean commercial licensing. Distinct means distinct: astrology is one domain that includes natal charts, horoscopes, synastry, and transits, not three domains counted separately. Think of it as the Stripe of insight APIs: AI-native infrastructure for astrology, tarot, numerology, and prediction apps so builders can ship in days instead of months.

Every calculation is rigorously verified against authoritative sources. The proof is public, the breadth is one key, the licensing is clean.

## What RoxyAPI does

One subscription gives builders production-ready access to every major spiritual and prediction domain through a single REST API and a single set of MCP servers. Domains in canonical order:

- **Western astrology**: natal charts, daily horoscopes, weekly and monthly horoscopes, synastry, compatibility scoring, transits, moon phase. Placidus, whole-sign, equal, and Koch house systems.
- **Vedic and KP astrology**: kundli, detailed panchang (rahu kaal, abhijit muhurta, brahma muhurta, choghadiya, hora), Vimshottari dasha (current period and full 120-year timeline), dosha analysis (Manglik, Kaal Sarp, Sade Sati), navamsa, 36-point Ashtakoota Guna Milan compatibility, plus KP sub-lord, sub-sub-lord, and ruling-planet horary. KP is the sharpest technical differentiator versus generic Vedic providers.
- **Numerology**: Life Path, full chart, compatibility, personal year, expression. Pythagorean reduction with master-number (11, 22, 33) and karmic-debt detection.
- **Tarot**: daily card, three-card spread, Celtic Cross, yes-no, love spread, custom draws. Deterministic seeded draws for once-per-day behavior.
- **Human Design**: full bodygraph (type, strategy, inner authority, profile, definition), defined and open centers, channels, gates, current transit overlay, and two-person connection (composite) charts.
- **Forecast**: cross-domain predictive timelines, transit windows, and significant-date detection across Western, Vedic, and biorhythm signals for any date range.
- **Biorhythm**: daily, multi-day forecast, compatibility, critical-day alerts. 10 cycle types.
- **I Ching**: 64-hexagram catalog, daily hexagram, three-coin cast with changing lines and resulting hexagram.
- **Crystals**: by zodiac, by chakra, birthstone, free-text search.
- **Dream interpretation**: symbol catalog, daily symbol, structured meanings.
- **Angel numbers**: by exact number, universal lookup with digit-root fallback, daily.
- **Location and timezone resolution** for accurate birth-data inputs (call this first when any chart endpoint needs coordinates).

Every endpoint returns structured JSON, ships rich field descriptions for tool-calling agents, and is callable from REST, the official SDKs, or remote MCP. Translated interpretations are available in 8 languages via the `?lang=` parameter.

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
| PHP | `roxyapi/sdk` | [RoxyAPI/sdk-php](https://github.com/RoxyAPI/sdk-php) |
| C# and .NET | `RoxyApi.Sdk` | [RoxyAPI/sdk-dotnet](https://github.com/RoxyAPI/sdk-dotnet) |
| Go | `github.com/RoxyAPI/sdk-go` | [RoxyAPI/sdk-go](https://github.com/RoxyAPI/sdk-go) |
| WordPress plugin | [Live on WordPress.org](https://wordpress.org/plugins/roxyapi/) | [RoxyAPI/sdk-wordpress](https://github.com/RoxyAPI/sdk-wordpress) |

All five code SDKs stay in lockstep with the API, so new endpoints land in your IDE the day they ship. The C# and .NET package targets net8.0 and netstandard2.0, so it runs on modern .NET, ASP.NET Core, Blazor, MAUI, and Unity. The Go module installs with a single `go get github.com/RoxyAPI/sdk-go` and is built for cloud-native and serverless backends. Each SDK ships an AGENTS.md so AI coding assistants in Cursor, Claude Code, Copilot, and Windsurf know how to call RoxyAPI without prompt-engineering.

The WordPress plugin is live on WordPress.org for no-code installs: drop a shortcode, no code required.

## Drop-in UI components

Roxy UI renders the API response for you: natal wheels, kundli, panchang, tarot spreads, numerology charts, Human Design bodygraphs, and biorhythm curves, themed with `--roxy-*` CSS custom properties and typed from the OpenAPI spec. Pass the SDK response straight into `data`, with no field renames and no glue code. Install exactly one package for your framework.

| Framework | Package |
|---|---|
| Web components, any framework or none | [`@roxyapi/ui`](https://www.npmjs.com/package/@roxyapi/ui) |
| React and Next.js | [`@roxyapi/ui-react`](https://www.npmjs.com/package/@roxyapi/ui-react) |
| Vue and Nuxt | [`@roxyapi/ui-vue`](https://www.npmjs.com/package/@roxyapi/ui-vue) |

Live component gallery and theming reference: [roxyapi.com/ui](https://roxyapi.com/ui).

## MCP servers

RoxyAPI was MCP-first from day one, and ships two kinds of remote Streamable HTTP MCP server for two different jobs. No local processes, no stdio wrappers, no self-hosting. Point a client at a URL and it is running in seconds.

### Docs server, for coding agents

The Docs server at `https://roxyapi.com/mcp/docs` exposes one tool, `search_docs`, over the entire RoxyAPI reference: every endpoint, parameter, SDK call, and guide. It is public, needs no API key, and returns documentation only, never live calculations. This is the server to give an AI coding assistant such as GitHub Copilot, Claude Code, or Cursor. Connect it while you build and the agent wires the whole RoxyAPI stack into your app, with the right field names the first time, in under 30 minutes.

```json
{
  "mcpServers": {
    "roxy-docs": {
      "url": "https://roxyapi.com/mcp/docs"
    }
  }
}
```

### Domain servers, for runtime agents

Each product domain ships its own MCP server that performs real, billable calculations. These are for the runtime agents and automations your users actually interact with: ChatGPT, Claude Desktop, and Gemini, workflow tools like n8n, Make, and Zapier, agent platforms like Dify and CrewAI, and Telegram, WhatsApp, and Slack bots. One API key unlocks every domain.

| Domain | MCP endpoint |
|---|---|
| Western astrology | `https://roxyapi.com/mcp/astrology` |
| Vedic and KP astrology | `https://roxyapi.com/mcp/vedic-astrology` |
| Numerology | `https://roxyapi.com/mcp/numerology` |
| Tarot | `https://roxyapi.com/mcp/tarot` |
| Human Design | `https://roxyapi.com/mcp/human-design` |
| Forecast | `https://roxyapi.com/mcp/forecast` |
| Biorhythm | `https://roxyapi.com/mcp/biorhythm` |
| I Ching | `https://roxyapi.com/mcp/iching` |
| Crystals | `https://roxyapi.com/mcp/crystals` |
| Dreams | `https://roxyapi.com/mcp/dreams` |
| Angel numbers | `https://roxyapi.com/mcp/angel-numbers` |
| Location and timezone | `https://roxyapi.com/mcp/location` |

Add your API key via the `X-API-Key` header on the domain servers. Rule of thumb: a coding agent wants the Docs server to write the integration, a runtime agent wants a domain server to compute a real chart.

The flagship multi-MCP reference integration is [RoxyAPI/astrology-ai-chatbot](https://github.com/RoxyAPI/astrology-ai-chatbot), an MIT-licensed chatbot starter that wires multiple RoxyAPI MCP servers into a single conversational agent.

## Verified accuracy

<a href="https://roxyapi.com/methodology">
  <img src="https://raw.githubusercontent.com/RoxyAPI/.github/main/profile/assets/verified.png" alt="Verified accuracy. Cross-checked against NASA JPL Horizons. Open methodology and public benchmark." width="100%">
</a>

Astronomy is the one place AI confidently lies. RoxyAPI treats accuracy as the moat.

- Powered by **Roxy Ephemeris**, cross-referenced against **NASA JPL Horizons DE441** as the physics ground truth.
- Vedic and KP outputs cross-referenced against DrikPanchang, onlinejyotish.com, JyotishApp, and timeanddate.com.
- Public methodology with tolerance thresholds and verification tables: [roxyapi.com/methodology](https://roxyapi.com/methodology).
- Public, MIT-licensed benchmark anyone can clone, run, or point at any astrology API: [RoxyAPI/astrology-api-benchmark](https://github.com/RoxyAPI/astrology-api-benchmark). 210 reference planet positions across 21 birth charts, 210 of 210 within tolerance, median deviation 0.27 arcmin.
- No AGPL, no copyleft, no commercial-license entanglements passed to customers. Clean commercial licensing for production use.

## Starter templates

Open-source templates, all MIT, that wrap RoxyAPI into a working app you can fork, rebrand, and ship:

- [spiritual-practitioner-website-template](https://github.com/RoxyAPI/spiritual-practitioner-website-template): a complete white-label website for a working astrologer, tarot reader, or numerologist. Free readings on your own domain, bookings, blog, prices, four palettes. Edit one config file, deploy, done. The self-hosted alternative to renting a page builder.
- [astrology-ai-chatbot](https://github.com/RoxyAPI/astrology-ai-chatbot): flagship multi-MCP astrology assistant
- [spiritual-ai-voice-assistant](https://github.com/RoxyAPI/spiritual-ai-voice-assistant): voice-driven spiritual assistant with an embeddable widget
- [astrology-starter-app](https://github.com/RoxyAPI/astrology-starter-app): Western astrology baseline
- [vedic-astrology-starter-app](https://github.com/RoxyAPI/vedic-astrology-starter-app): Vedic and KP focused
- [jyotish-vedic-astrology-app](https://github.com/RoxyAPI/jyotish-vedic-astrology-app): Jyotish app with Kundli, Panchang, Gun Milan, Dasha, built on the drop-in UI components
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

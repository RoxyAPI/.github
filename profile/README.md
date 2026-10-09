<a href="https://roxyapi.com">
  <img src="https://raw.githubusercontent.com/RoxyAPI/.github/main/profile/assets/hero.png" alt="RoxyAPI. The Spiritual OS layer for agentic AI. Insight products, shipped in days. One key, flat pricing." width="100%">
</a>

# RoxyAPI

**RoxyAPI is the data layer for insight, belief and prediction apps: one Astrology API key for all 18+ insight domains, with a hosted astrology MCP server for every domain.** Western and Vedic astrology, forecast, Human Design, Chinese astrology, feng shui, Mesoamerican astrology, Vastu, numerology, Kabbalah, tarot, biorhythm, Ayurveda, I Ching, crystals, dreams, angel numbers and location, through one REST API, typed SDKs in five languages, and Remote MCP. Calculations read the NASA JPL DE440 ephemeris directly and are verified against NASA JPL Horizons. One request is one unit on every endpoint, nothing AGPL sits anywhere in the stack, and every plan includes every domain.

The Spiritual OS layer for agentic AI. Your app and your agents plug in; your model, your prompt and your users stay yours.

[![Live API](https://img.shields.io/badge/API-Live_playground-1f6feb?style=flat-square&logo=swagger&logoColor=white)](https://roxyapi.com/api-reference)
[![MCP](https://img.shields.io/badge/MCP-Remote_%26_stdio-ec4899?style=flat-square)](https://github.com/RoxyAPI/astrology-mcp-server)
[![Methodology](https://img.shields.io/badge/Methodology-NASA_JPL_verified-fb923c?style=flat-square)](https://roxyapi.com/methodology)
[![Benchmark](https://img.shields.io/badge/Benchmark-Open_%26_MIT-22c55e?style=flat-square&logo=github&logoColor=white)](https://github.com/RoxyAPI/astrology-api-benchmark)
[![OpenAPI](https://img.shields.io/badge/OpenAPI-3.1_spec-6ba539?style=flat-square&logo=openapiinitiative&logoColor=white)](https://github.com/RoxyAPI/astrology-api-openapi)
[![Pricing](https://img.shields.io/badge/Pricing-Plans_%26_quotas-0ea5e9?style=flat-square)](https://roxyapi.com/pricing)
[![Templates](https://img.shields.io/badge/Templates-MIT_licensed-8b5cf6?style=flat-square)](https://roxyapi.com/templates)
[![Widgets](https://img.shields.io/badge/Widgets-No_code_embeds-14b8a6?style=flat-square)](https://roxyapi.com/widgets)

## RoxyAPI at a glance

| | |
|---|---|
| Domains under one key | 18+, each a genuinely distinct system |
| Production endpoints | 261+, one call returns a complete result |
| Agent tools over Remote MCP | 258+, one tool per calculation endpoint, one hosted server per domain |
| Automated tests per deploy | 13,000+, including 3,000+ gold-standard tests pinned to named external references |
| Median deviation from NASA JPL Horizons DE441 | 0.05 arcseconds (0.00001 degrees), in an open MIT benchmark you can re-run |
| Interpretation languages | 10+ via one query parameter, included in every plan |
| Typed SDKs | TypeScript, Python, PHP, C# and Go, plus a WordPress plugin and an n8n node |
| Pricing | 1 request = 1 unit on REST and MCP alike, no credit weighting. From 39 USD per month for every domain, as low as 1.80 USD per domain on annual billing |
| Median response time | Under 50 ms |
| Uptime | Reported on an [independent status page](https://stats.uptimerobot.com/T0kPZKlAjf "Live RoxyAPI uptime on UptimeRobot, an independently hosted third party status page") we cannot edit, against a 99.95 percent SLA |
| Data at rest | Germany, inside the EU, on every plan |
| Licensing | Commercial on every plan. No AGPL, no copyleft, no royalties |

Every structural figure above is re-countable by you against the [live OpenAPI spec](https://roxyapi.com/api/v2/openapi.json "The combined RoxyAPI OpenAPI specification, generated from production so it cannot drift") and this GitHub org. Usage figures and their measurement dates are published at [roxyapi.com/transparency](https://roxyapi.com/transparency "RoxyAPI transparency report: structural counts, dated usage figures, and citable facts").

## Astrology MCP servers for AI agents

RoxyAPI ships Remote MCP over Streamable HTTP: hosted, one server per domain, nothing to install. Point a client at a URL and it runs.

**Runtime agents** (Claude Desktop, n8n, Zapier, Copilot Studio, Mistral, Perplexity, and any agent framework that can set a request header) use the domain servers, which perform real calculations. One API key unlocks every domain.

| Domain | Remote MCP endpoint |
|---|---|
| Western astrology | `https://roxyapi.com/mcp/astrology` |
| Vedic and KP astrology | `https://roxyapi.com/mcp/vedic-astrology` |
| Forecast | `https://roxyapi.com/mcp/forecast` |
| Human Design | `https://roxyapi.com/mcp/human-design` |
| Chinese astrology | `https://roxyapi.com/mcp/chinese-astrology` |
| Feng shui | `https://roxyapi.com/mcp/feng-shui` |
| Mesoamerican astrology | `https://roxyapi.com/mcp/mesoamerican-astrology` |
| Vastu | `https://roxyapi.com/mcp/vastu` |
| Numerology | `https://roxyapi.com/mcp/numerology` |
| Kabbalah | `https://roxyapi.com/mcp/kabbalah` |
| Tarot | `https://roxyapi.com/mcp/tarot` |
| Biorhythm | `https://roxyapi.com/mcp/biorhythm` |
| Ayurveda | `https://roxyapi.com/mcp/ayurveda` |
| I Ching | `https://roxyapi.com/mcp/iching` |
| Crystals | `https://roxyapi.com/mcp/crystals` |
| Dreams | `https://roxyapi.com/mcp/dreams` |
| Angel numbers | `https://roxyapi.com/mcp/angel-numbers` |
| Location and timezone | `https://roxyapi.com/mcp/location` |

Client setup, authentication and every config format: [roxyapi.com/docs/mcp](https://roxyapi.com/docs/mcp "RoxyAPI Remote MCP setup: server URLs, client configuration, compact responses, and which server to point a coding agent at").

**Clients that only start local servers** run the open source [astrology-mcp-server](https://github.com/RoxyAPI/astrology-mcp-server "RoxyAPI astrology MCP server: a stdio package that relays to the hosted Remote MCP servers, same tools, same key") package, or Claude Desktop users double-click the one-file [desktop extension](https://github.com/RoxyAPI/astrology-mcp-server/releases/latest/download/astrology-mcp-server.mcpb "RoxyAPI astrology MCP server as a one-click Claude Desktop extension"). Both relay to the same hosted servers, so the tools, the answers and the billing are identical:

```json
{
  "mcpServers": {
    "roxy-astrology": {
      "command": "npx",
      "args": ["-y", "@roxyapi/mcp"],
      "env": { "ROXY_API_KEY": "your-key" }
    }
  }
}
```

**Coding agents** (GitHub Copilot, Claude Code, Cursor, Codex, Gemini CLI) use the keyless docs server at `https://roxyapi.com/mcp/docs`. Its one tool, `search_docs`, searches every endpoint, parameter, SDK call and guide, so the agent wires the integration with the right field names the first time. RoxyAPI is also a one-step [plugin for Claude Code and Cursor](https://github.com/RoxyAPI/agent-plugin "RoxyAPI agent plugin for Claude Code, Cursor and Agent Plugins clients: bundles the keyless docs MCP server and a skill in one install").

**Lower inference cost, same data.** Pass `compact: true` on any tool call for a lossless, token-optimized response: arrays of same-shaped rows travel columnar, so a field name is sent once instead of once per row. About 40 percent fewer tokens on a natal chart, about 52 percent on astrocartography. Your quota is unchanged, because 1 request stays 1 unit.

**Charts, not paragraphs, in AI chat.** `componentForTool` in the UI library maps any Remote MCP tool name to the component that draws its result, so a chatbot shows a natal wheel, a kundli or a tarot spread beside the model reply. The flagship [astrology-ai-chatbot](https://github.com/RoxyAPI/astrology-ai-chatbot "Open source MIT licensed AI astrology chatbot wiring multiple RoxyAPI Remote MCP servers into one conversational agent") template ships it.

## Simple surface, advanced core

Breadth usually costs depth. Here it does not, and the proof is named endpoints rather than adjectives. One request returns a complete result, so the advanced layer lives inside the engine instead of inside your integration.

| Domain | What ships past the basics |
|---|---|
| [Western astrology](https://roxyapi.com/products/astrology-api "RoxyAPI western astrology: fixed stars, asteroids, Arabic lots, aspect patterns, progressions, solar arc, profections, astrocartography, relocation and local space maps, and return charts") | Natal charts in Placidus, whole-sign, equal and Koch, daily to yearly horoscopes that name the dated sky events behind each reading, synastry, composite and compatibility scoring, plus fixed stars, asteroid goddesses, Arabic lots, Black Moon Lilith, aspect patterns, secondary progressions, solar arc, profections, astrocartography, relocation charts, local space, and solar, lunar and planetary returns. |
| [Vedic and KP](https://roxyapi.com/products/vedic-astrology-api "RoxyAPI Vedic astrology: 44 yoga verdicts with classical evidence, shadbala, bhava bala, ashtakavarga, Arudha padas, Chara Karakas, avasthas, upagrahas, and KP sub-lords") | Kundli, detailed panchang, Vimshottari dasha to sookshma, doshas, divisional charts, Ashtakoota and South Indian matchmaking, KP sub-lords and ruling planets, and 44 classical yoga verdicts that each carry the evidence that triggered them and the rule that silenced them. Plus shadbala, bhava bala, ashtakavarga, Arudha padas, Chara Karakas, upagrahas, bhav chalit and 17 avastha states. |
| [Forecast](https://roxyapi.com/products/forecast-api "RoxyAPI forecast: one request merges western transit events, Vimshottari dasha boundaries, and biorhythm critical days into a single significance-scored timeline") | One request merges Western transit events, Vimshottari dasha boundaries and biorhythm critical days into a single time-ordered, significance-scored feed. |
| [Human Design](https://roxyapi.com/products/human-design-api "RoxyAPI human design: Variables with Color, Tone and Base, Penta group analysis, connection charts, and transit overlays on a natal bodygraph") | Full bodygraph with type, authority, profile and incarnation cross, the design moment solved on the true 88 degree solar arc, Variables with Color, Tone and Base, Penta, connection charts and transit overlays. |
| [Chinese astrology and feng shui](https://roxyapi.com/products/chinese-astrology-api "RoxyAPI Chinese astrology: BaZi Four Pillars, luck pillars, day master strength, lunisolar calendar and almanac with typed school conventions") | BaZi Four Pillars, luck pillars, day master strength, the lunisolar calendar with solar terms as astronomical instants, the almanac day and auspicious-date search, Xuan Kong flying stars, Kua and Eight Mansions. The school splits that make two calculators disagree are typed parameters, echoed on every response. |
| [Mesoamerican astrology](https://roxyapi.com/products/mesoamerican-astrology-api "RoxyAPI Mesoamerican astrology: four correlation constants, three name traditions, a typed Year Bearer school, and a Long Count converter that runs both ways") | Tzolkin, Haab, Long Count, Calendar Round and the Aztec tonalpohualli, with four published correlation constants as a typed field and the resolved value echoed back. |
| [Vastu](https://roxyapi.com/products/vastu-api "RoxyAPI Vastu: per-rule verse citations as typed fields, text-parameterised Ayadi, and griha pravesh dates composed over the panchang") | Entrance padas, the 81 and 64 pada mandala, plot analysis, Ayadi and griha pravesh dates, with every rule citing its verse as a typed `source` field. |
| [Kabbalah](https://roxyapi.com/products/kabbalah-api "RoxyAPI Kabbalah: every candidate Hebrew spelling returned, ten typed conventions echoed on the response, the 72 names derived from the verses") | Gematria across rabbinic ciphers with every candidate Hebrew spelling of a Latin name shown, birth profiles, the 72 names derived from the verses rather than copied from a table, and the Tree of Life with typed school variants. |
| [Ayurveda](https://roxyapi.com/products/ayurveda-api "RoxyAPI Ayurveda: constitution from the three classical chart factors, ritucharya from solar longitude, no questionnaire and no health input") | Constitution from the three classical factors of the birth chart with their verses, ritu from the exact solar longitude, and dinacharya as clock times from the local sunrise. General-wellness framing. |
| Numerology, tarot, biorhythm, I Ching, crystals, dreams, angel numbers | Life Path and full charts with master numbers and karmic debt, seeded tarot spreads, ten biorhythm cycles, three-coin I Ching casts, and structured content catalogues, every one localized. |

**The domains compose, they do not merely coexist.** Human Design is computed from the Western ephemeris and the I Ching hexagram set, the Ayurvedic constitution is read from the Vedic birth chart, and Vastu griha pravesh dates are found over the same panchang. The sidereal and tropical engines are tested to return the same sky at zero tolerance. That is the capability single-domain vendors cannot be stitched into.

## Verified accuracy

<a href="https://roxyapi.com/methodology">
  <img src="https://raw.githubusercontent.com/RoxyAPI/.github/main/profile/assets/verified.png" alt="Verified accuracy. Cross-checked against NASA JPL Horizons. Open methodology and public benchmark." width="100%">
</a>

Astronomy is the one place AI confidently invents answers. RoxyAPI publishes the evidence instead of asking to be trusted.

- **Roxy Ephemeris**, built in house, reads the **NASA JPL DE440** ephemeris directly and is verified against **NASA JPL Horizons DE441**.
- **13,000+ automated tests run on every deploy**, including **3,000+ gold-standard tests** each pinned to a named external reference.
- **An open, MIT-licensed benchmark** anyone can clone and point at any astrology API: [astrology-api-benchmark](https://github.com/RoxyAPI/astrology-api-benchmark "MIT licensed reproducible astrology API accuracy benchmark verified against NASA JPL Horizons DE441"). Median deviation **0.05 arcseconds (0.00001 degrees)**; its README holds the full results, the worst point named, and the script and dataset to reproduce them.
- **Published methodology** with the test corpus, tolerances and reference sources per domain: [roxyapi.com/methodology](https://roxyapi.com/methodology "RoxyAPI methodology: test corpus, tolerances, named reference sources, and verification tables").
- **Proof before you pay.** The [live playground](https://roxyapi.com/api-reference "RoxyAPI live playground returning real production responses from the typed OpenAPI specification, no signup required") returns real production responses with no signup.

## Licensing, privacy and data residency

- **No AGPL, no copyleft, no source disclosure.** The engine is built in house, so nothing copyleft reaches your product. AGPL copyleft triggers on network access and an API is a network service, which is why [Google bans AGPL dependencies company-wide](https://opensource.google/documentation/reference/using/agpl-policy "Google open source policy: AGPL licensed code may not be used at Google"). A package manager often hands teams a copyleft wrapper as the free path, and the obligation arrives unread. Ask any provider for their position in writing, including us; ours is at [roxyapi.com/policy/license](https://roxyapi.com/policy/license "RoxyAPI commercial license: no AGPL, no copyleft, no per user royalties, full commercial terms on every plan").
- **A commercial license on every plan.** Ship closed-source apps to any app store, white label for clients, and pass the license audits that funding rounds and acquisitions run.
- **Stateless by design.** Birth data is computed in memory and never written to a database, so there is no store to breach and nothing to erase when a data subject request arrives. Memory and personalization stay in your stack; the MIT [ai-spiritual-companion](https://github.com/RoxyAPI/ai-spiritual-companion "MIT AI companion template that remembers every user, on a database the operator owns") template ships that layer ready to fork.
- **EU data residency and an Article 28 DPA on every plan.** Stored data stays in Germany for every customer, and the DPA, Standard Contractual Clauses, technical measures and a dated subprocessor register are published for procurement: [roxyapi.com/policy/dpa](https://roxyapi.com/policy/dpa "RoxyAPI self serve GDPR Article 28 Data Processing Addendum").
- **Bring your own LLM.** No per-token markup and no hidden system prompt: your agent calls the tools, your model writes the reply in your voice.

## How RoxyAPI compares

Category-level, no names. Run these checks against any vendor, including us.

| Capability | RoxyAPI | Legacy astrology APIs | DIY open source libraries |
|---|---|---|---|
| Domains under one key and one subscription | Yes, 18+ | No, priced per product | No, one library each |
| One call returns a complete result | Yes | Often split across separately billed calls | Assembly required |
| Flat request pricing, 1 request = 1 unit on REST and MCP | Yes | Varies, credit tables weight endpoints | Yes, self hosted |
| New domains land inside the existing plan | Yes | No, new invoice | No, new build |
| Hosted Remote MCP server per domain | Yes, plus a stdio package | Varies, local stdio wrappers | No, build your own |
| Token-optimized agent responses | Yes, opt-in and lossless | Not offered | Not offered |
| Automated tests published per deploy | Yes, 13,000+ with 3,000+ gold-standard | Not published | Yours to write |
| Open benchmark anyone can re-run against any provider | Yes, MIT | No public artifact | Run it yourself |
| Real production responses before you pay | Yes, no signup | Varies, signup or sandbox | Install first |
| Typed SDKs generated from a live spec | Yes, 5 languages | Varies, hand-kept exports | Read the source |
| Drop-in UI components and no-code widgets | Yes | No | No |
| Interpretation text localized in 10+ languages | Yes | Varies, horoscopes mostly | No, numbers only |
| Engine free of AGPL copyleft exposure | Yes | Varies, inherited from a wrapper | No, copyleft is common |
| EU data residency with an Article 28 DPA on every plan | Yes | Varies, enterprise only | Yours to write |
| Stateless, zero end-user data stored | Yes | Varies, accounts and logs | Yes, self hosted |

**Honest footnote.** If you need exactly one domain, run your own servers and accept copyleft terms, a free library is cheaper. Everything else in this table is where RoxyAPI earns its keep.

## Build with it

**Typed SDKs**, generated from the live OpenAPI spec so they cannot drift. Each ships an AGENTS.md so coding assistants call RoxyAPI correctly.

| Language | Package | Repository |
|---|---|---|
| TypeScript | `@roxyapi/sdk` | [sdk-typescript](https://github.com/RoxyAPI/sdk-typescript) |
| Python | `roxy-sdk` | [sdk-python](https://github.com/RoxyAPI/sdk-python) |
| PHP | `roxyapi/sdk` | [sdk-php](https://github.com/RoxyAPI/sdk-php) |
| C# and .NET | `RoxyApi.Sdk` | [sdk-dotnet](https://github.com/RoxyAPI/sdk-dotnet) |
| Go | `github.com/RoxyAPI/sdk-go` | [sdk-go](https://github.com/RoxyAPI/sdk-go) |

[![npm](https://img.shields.io/npm/v/@roxyapi/sdk?style=flat-square&logo=npm&label=%40roxyapi%2Fsdk)](https://www.npmjs.com/package/@roxyapi/sdk)
[![PyPI](https://img.shields.io/pypi/v/roxy-sdk?style=flat-square&logo=pypi&logoColor=white&label=roxy-sdk)](https://pypi.org/project/roxy-sdk/)
[![Packagist](https://img.shields.io/packagist/v/roxyapi/sdk?style=flat-square&logo=packagist&logoColor=white&label=roxyapi%2Fsdk)](https://packagist.org/packages/roxyapi/sdk)
[![NuGet](https://img.shields.io/nuget/v/RoxyApi.Sdk?style=flat-square&logo=nuget&logoColor=white&label=RoxyApi.Sdk)](https://www.nuget.org/packages/RoxyApi.Sdk)
[![Go module](https://img.shields.io/github/v/tag/RoxyAPI/sdk-go?style=flat-square&logo=go&logoColor=white&label=sdk-go)](https://pkg.go.dev/github.com/RoxyAPI/sdk-go)
[![MCP](https://img.shields.io/npm/v/@roxyapi/mcp?style=flat-square&logo=npm&label=%40roxyapi%2Fmcp)](https://www.npmjs.com/package/@roxyapi/mcp)

**The OpenAPI spec as a repository.** [astrology-api-openapi](https://github.com/RoxyAPI/astrology-api-openapi "RoxyAPI OpenAPI 3.1 specification, refreshed daily from production") holds the full OpenAPI 3.1 specification, refreshed daily from production. Import it into Postman, Insomnia or Bruno, or generate a client in any language. Ready-made [Postman collections](https://github.com/RoxyAPI/postman-collections "RoxyAPI Postman collections for every domain, generated from the live OpenAPI specification") are generated from it.

**Roxy UI, for developers.** Drop-in components render the API response for you: natal wheels, synastry charts, Vedic kundli, KP charts, dasha timelines, panchang tables, shadbala grids, Human Design bodygraphs, tarot spreads, numerology cards, hexagrams, biorhythm curves and astrocartography maps. Themed with CSS custom properties, typed from the spec, MIT licensed. Live gallery: [roxyapi.com/ui](https://roxyapi.com/ui "Roxy UI live component gallery").

| Framework | Package |
|---|---|
| Web components, any framework or none | [`@roxyapi/ui`](https://www.npmjs.com/package/@roxyapi/ui) |
| React and Next.js | [`@roxyapi/ui-react`](https://www.npmjs.com/package/@roxyapi/ui-react) |
| Vue and Nuxt | [`@roxyapi/ui-vue`](https://www.npmjs.com/package/@roxyapi/ui-vue) |

Single-component starters: [natal-chart-wheel](https://github.com/RoxyAPI/natal-chart-wheel "Natal chart wheel web component: planets, houses and aspects from a birth date, time and city"), [kundli-chart](https://github.com/RoxyAPI/kundli-chart "Kundli chart web component: North, South and East Indian Vedic birth chart from birth data") and [human-design-bodygraph](https://github.com/RoxyAPI/human-design-bodygraph "Human Design bodygraph web component: centers, channels, gates, type, authority and profile").

**Widgets, for everyone else.** The same components in no-code mode: paste one snippet into Squarespace, Wix, Shopify, WordPress, Notion or Linktree and a live reading renders with no backend. Browser-safe publishable keys are scoped to the sites you name. Gallery and snippets: [roxyapi.com/widgets](https://roxyapi.com/widgets "RoxyAPI copy-paste astrology widgets for any website, no code and no backend").

**No-code and automation.** The [WordPress plugin](https://wordpress.org/plugins/roxyapi/ "RoxyAPI WordPress plugin on WordPress.org: Gutenberg blocks and shortcodes") ([sdk-wordpress](https://github.com/RoxyAPI/sdk-wordpress)) adds Gutenberg blocks and shortcodes. The [n8n node](https://github.com/RoxyAPI/n8n-nodes-roxyapi "RoxyAPI n8n community node: every domain as an n8n resource, usable as an AI Agent tool") puts every domain into n8n workflows and its AI Agent, and [n8n-astrology-ai-agent](https://github.com/RoxyAPI/n8n-astrology-ai-agent "Import-ready n8n astrology AI agent workflow") is an import-ready chat agent built on it.

## Templates

Open source, MIT licensed apps you can fork, rebrand and ship as your own product:

- [astrology-ai-chatbot](https://github.com/RoxyAPI/astrology-ai-chatbot): flagship multi-MCP AI astrology assistant. Discovers the tool catalog over Remote MCP, draws every tool result as a chart, spread or bodygraph beside the reply, works with any LLM.
- [ai-spiritual-companion](https://github.com/RoxyAPI/ai-spiritual-companion): an AI companion that remembers every user, with semantic recall, full reading history and accounts with row level security on a database the operator owns.
- [spiritual-practitioner-website-template](https://github.com/RoxyAPI/spiritual-practitioner-website-template): a complete white-label website for an astrologer, tarot reader or numerologist. Edit one config file, deploy.
- [spiritual-ai-voice-assistant](https://github.com/RoxyAPI/spiritual-ai-voice-assistant): voice-driven spiritual assistant with an embeddable widget.
- [jyotish-vedic-astrology-app](https://github.com/RoxyAPI/jyotish-vedic-astrology-app): Jyotish web app with kundli, panchang, Gun Milan and dasha.
- [astrology-supabase-starter](https://github.com/RoxyAPI/astrology-supabase-starter): the backend on its own, Edge Functions plus a Postgres cache, for teams that already have a front end.
- Mobile starters for React Native and Expo: [astrology](https://github.com/RoxyAPI/astrology-starter-app), [vedic astrology](https://github.com/RoxyAPI/vedic-astrology-starter-app), [numerology](https://github.com/RoxyAPI/numerology-starter-app), [tarot](https://github.com/RoxyAPI/tarot-starter-app), [dreams](https://github.com/RoxyAPI/dreams-starter-app).

Gallery with screenshots and one-click deploys: [roxyapi.com/templates](https://roxyapi.com/templates "Open source MIT licensed RoxyAPI templates you can clone and white label").

## Per-endpoint code samples

One small repository per high-demand capability, each with runnable TypeScript, JavaScript and Python samples against the live API:

- **Western:** [natal-chart-api](https://github.com/RoxyAPI/natal-chart-api), [daily-horoscope-api](https://github.com/RoxyAPI/daily-horoscope-api), [synastry-api](https://github.com/RoxyAPI/synastry-api), [astrology-compatibility-api](https://github.com/RoxyAPI/astrology-compatibility-api), [transit-forecast-api](https://github.com/RoxyAPI/transit-forecast-api), [moon-phase-api](https://github.com/RoxyAPI/moon-phase-api)
- **Vedic and KP:** [kundli-api](https://github.com/RoxyAPI/kundli-api), [kundli-matching-api](https://github.com/RoxyAPI/kundli-matching-api), [panchang-api](https://github.com/RoxyAPI/panchang-api), [dasha-api](https://github.com/RoxyAPI/dasha-api), [kp-astrology-api](https://github.com/RoxyAPI/kp-astrology-api)
- **Chinese astrology and feng shui:** [bazi-api](https://github.com/RoxyAPI/bazi-api), [chinese-lunar-calendar-api](https://github.com/RoxyAPI/chinese-lunar-calendar-api), [chinese-almanac-api](https://github.com/RoxyAPI/chinese-almanac-api), [feng-shui-flying-stars-api](https://github.com/RoxyAPI/feng-shui-flying-stars-api), [kua-number-api](https://github.com/RoxyAPI/kua-number-api), [tai-sui-api](https://github.com/RoxyAPI/tai-sui-api)
- **More domains:** [human-design-api](https://github.com/RoxyAPI/human-design-api), [numerology-api](https://github.com/RoxyAPI/numerology-api), [tarot-api](https://github.com/RoxyAPI/tarot-api), [biorhythm-api](https://github.com/RoxyAPI/biorhythm-api)

## Track record

Newer than the incumbents, and further along than that usually implies.

| When | What |
|---|---|
| 2020 | Groundwork begins on the in-house Roxy Ephemeris engine, built for APIs and agents from the start |
| 2024 | The platform opens to the public |
| March 2025 | Cumulative production traffic crosses 1 million API requests |
| March 2026 | Production traffic reaches a run rate of 10 million requests per quarter |
| May 2026 | About 200,000 calls per month arrive from AI agents over Remote MCP |
| September 2026 | Roxy Ephemeris reads the NASA JPL DE440 ephemeris directly; the open benchmark median is 0.05 arcseconds |

RoxyAPI is independently operated, and every number on this page is one you can check.

## Questions developers ask before integrating

**What is the best astrology API for AI agents?**
Pick on what an agent needs: a hosted MCP server it can call with no local install, typed tools generated from a real spec, verified numbers, and one key across every domain a conversation can wander into. RoxyAPI ships a Remote MCP server per domain, a stdio package for local-only clients, 258+ typed tools and an open benchmark, so you can check each claim before you commit.

**Is RoxyAPI just an astrology API?**
No. Astrology is one of 18+ distinct domains on the same key. One system counts once, so the total reads smaller than a padded catalog and delivers more per call.

**Should I build this myself?**
You can compute a chart yourself, but a production offering is ongoing engineering: accuracy kept verified against NASA JPL Horizons, 18+ domains, interpretations in 10+ languages, Remote MCP, typed SDKs, UI components and the uptime behind all of it. Licensing comes first: the free path is often a copyleft wrapper, and copyleft triggers on network access. If you need exactly one domain and can self-host, a library is cheaper, and we say so.

**Do you use Swiss Ephemeris?**
No. RoxyAPI runs Roxy Ephemeris, an in-house engine that reads the NASA JPL DE440 ephemeris directly and is verified against NASA JPL Horizons DE441. There is no copyleft obligation to inherit and no commercial ephemeris license to renew.

**How do I know the calculations are right?**
Clone the [MIT benchmark](https://github.com/RoxyAPI/astrology-api-benchmark "Reproducible MIT licensed accuracy benchmark for any astrology API"), run it against RoxyAPI, then against any other provider. The methodology page publishes the corpus, tolerances and reference sources behind every domain.

**What does it cost to add a domain?**
Nothing. Every plan includes every domain, every endpoint, Remote MCP, the SDKs, the UI components, the widgets and the 10+ interpretation languages, and new domains join the plan you already have.

**Can I use it in a closed-source commercial product?**
Yes. Every plan is a commercial license with no copyleft and no per-user royalties. The MIT templates and UI components can ship under your own brand.

**Where is the data stored?**
Nothing about your end users is kept: birth data is computed in memory and never written to a database. Operational data stays in Germany on every plan, under published Article 28 terms.

## Quick links

| Surface | URL |
|---|---|
| Live API playground | https://roxyapi.com/api-reference |
| Documentation | https://roxyapi.com/docs |
| Remote MCP setup | https://roxyapi.com/docs/mcp |
| Pricing | https://roxyapi.com/pricing |
| Methodology | https://roxyapi.com/methodology |
| Transparency report | https://roxyapi.com/transparency |
| Changelog | https://roxyapi.com/changelog |
| OpenAPI specification | https://roxyapi.com/api/v2/openapi.json |
| Agent discovery | https://roxyapi.com/llms.txt |

## Get started

1. Get a key at [roxyapi.com/pricing](https://roxyapi.com/pricing "RoxyAPI plans and quotas: every domain included on every plan, instant activation"). Every plan includes every domain.
2. Try the [live playground](https://roxyapi.com/api-reference "RoxyAPI live playground with real production responses and no signup").
3. Install an SDK, paste a widget, or point your agent at a Remote MCP server.

Questions or partnerships: [roxyapi.com/contact](https://roxyapi.com/contact "Contact RoxyAPI for integration help, procurement questions, or partnership inquiries"). Built by [Roxy Labs](https://roxyapi.com). The Stripe of insight APIs.

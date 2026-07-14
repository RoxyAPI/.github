# Security policy

## Reporting a vulnerability

Found a security issue in any RoxyAPI repo or in the API itself? Do not open a public issue.

Report it at https://roxyapi.com/contact?subject=security

We acknowledge reports within 48 hours and target a fix within 7 days for critical issues.

## Scope

In scope:
- The API at https://roxyapi.com/api/v2/* and the remote MCP servers at https://roxyapi.com/mcp/*
- Official SDKs: TypeScript (`@roxyapi/sdk`), Python (`roxy-sdk`), PHP (`roxyapi/sdk`), C# and .NET (`RoxyApi.Sdk`), Go (`github.com/RoxyAPI/sdk-go`), and the WordPress plugin
- Drop-in UI packages: `@roxyapi/ui`, `@roxyapi/ui-react`, `@roxyapi/ui-vue`
- Open-source starter templates published under https://github.com/RoxyAPI/
- Any other repo under https://github.com/RoxyAPI/

Out of scope:
- Vulnerabilities in third-party dependencies that already have a published advisory
- Rate-limit bypass using valid paid API keys (rate limits are commercial limits, not security boundaries)
- Self-XSS or social-engineering scenarios

## Acknowledgement

Researchers who report valid issues responsibly are credited in our security log if they choose to be named.

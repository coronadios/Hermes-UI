# Hermes UI

Hermes UI is an orchestration layer built on top of Hermes Agent. It provides a visual, interactive interface for managing 25 specialized agents, each with a defined purpose.

## Quick Start

Open `index.html` in any modern browser:

```bash
open index.html
```

No build step, no server required. The UI loads agents from `agents/hermes_agents.json`, applies the Linear dark design system, and connects to Gemini / OpenRouter APIs via the configured `api_config.json`.

## What It Includes

- **25 Agents** with defined roles (Sentry, Architect, Lens, Oracle, Forge, etc.)
- **Chat Interface** — select any agent or talk with the Principal agent
- **Dark Mode** — Linear-inspired palette with accessible contrast (16.5:1 verified)
- **SVG Graphics** — no emoji buttons; all icons are geometric SVG
- **Responsive Layout** — works on desktop and mobile
- **Accessibility** — `aria-label`, `focus-visible`, `prefers-reduced-motion`, keyboard navigation
- **Real-Time Loop** — background monitoring process (`loop.log`)
- **Local Persistence** — agent selection saved to `localStorage`

## Design System

Based on the Linear (`popular-web-designs` skill) design tokens:
- Background: `#08090a`
- Surface: `#191a1b`
- Accent: `#7170ff`
- Typography: Inter Variable with `cv01`, `ss03`
- Border: `rgba(255,255,255,0.08)`

## Agents

| Agent | Function |
|---|---|
| Sentry | System monitoring and alerts |
| Cartographer | File and dependency mapping |
| Scribe | Change and log documentation |
| Architect | Architecture and refactoring |
| Curator | Content filtering |
| Echo | Action confirmation |
| Lens | Code review |
| Pulse | Performance measurement |
| Bridge | API connections |
| Vault | Credential management |
| Oracle | Context-aware responses |
| Warden | Privacy and access control |
| Beacon | Notifications |
| Forge | Build generation |
| Mirror | Remote sync |
| Chronos | Scheduled tasks |
| Herald | Progress reporting |
| Compass | Navigation guidance |
| Tinker | Safe experimentation |
| Aegis | Attack defense |
| Aurora | Visual improvement |
| Cipher | Data encryption |
| Nomad | Migration and backups |
| Seer | Trend prediction |
| Anchor | System stability |

## Using the Chat

1. Select an agent from the dropdown or click a card.
2. The agent's role appears in the info panel.
3. Type in the input and press Send. The agent responds automatically without blocking other work.

## File Structure

```
HermesUI/
├── index.html          # Main interface
├── style.css            # Linear dark design tokens
├── app.js               # Minimal initialization
├── agents/
│   ├── hermes_agents.json
│   └── api_config.json
├── assets/
│   └── svg/
│       ├── hermes_logo.svg
│       └── icon_run.svg
└── loop.log             # Background loop log
```

## Development

- Edit `index.html`, `style.css`, or `agents/hermes_agents.json`
- Refresh the browser (no build needed)
- The loop (`loop.log`) continues in the background

## License

MIT — same as Hermes Agent.

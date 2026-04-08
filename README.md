# // parallel — Interactive Explainer

An unofficial, single-file interactive explainer for [Parallel Web Systems](https://parallel.ai) — a company building web search infrastructure for AI agents. The page makes three of Parallel's core engineering concepts viscerally click in under 60 seconds each: structured web search (how Parallel compresses messy HTML into clean, token-efficient JSON for AI agents), Basis confidence scoring (how every output field ships with a citation, an excerpt, and a calibrated HIGH / MEDIUM / LOW confidence rating), and multi-hop agentic research (how the Task API autonomously chains searches, navigates portals, and fills knowledge gaps without any task-specific training).

## Why I built this

I'm a MechE student who went deep on Parallel's docs and kept wishing there were a live, interactive demo of the three concepts their frontend team is explicitly building developer education around. So I built the explainer I wish existed. Each section is hands-on: Section 1 lets you fire real search queries through Claude's web search tool and watch the structured JSON come back; Section 2 lets you research any company and see Basis-style confidence scoring across eight fields; Section 3 animates the real Opendoor HOA workflow step-by-step with no API call required.

## How to run

1. Clone or download this repo.
2. Open `index.html` directly in any browser — no build step, no server needed.
3. Paste your [Anthropic API key](https://console.anthropic.com) into the floating input in the bottom-right corner. It's saved to `localStorage` and overrides the hardcoded placeholder.
4. Sections 1 and 2 are live — they call `claude-sonnet-4-20250514` with web search enabled. Section 3 is a pure animation (always works, no key needed).

## Links

- [parallel.ai](https://parallel.ai)
- [Parallel Docs](https://docs.parallel.ai)

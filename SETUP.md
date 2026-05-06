# Setup — do this before the workshop starts

You need three pieces working before Challenge 0:

1. **APM** — Anthropic's Agent Package Manager CLI
2. **`skill-creator`** — installed via APM
3. **JIRA MCP server** — connection details from your facilitator

If any of these fails during setup, raise it BEFORE the workshop. Five quiet minutes of pre-flight beat 50 minutes of frustration.

## 1. Install APM

APM is Anthropic's CLI for installing and managing Agent Skills. Follow the install instructions on the projector (they point at the official APM documentation — pinning a URL here would just go stale).

Verify with:
```bash
apm --version
```

## 2. Install workshop skills

From the root of this repository:
```bash
apm install
```

APM reads `apm.yaml` and installs the listed skills (currently: `skill-creator`) into your Copilot environment.

Verify by asking Copilot:
> "What skills do I have access to?"

You should see `skill-creator` in the list. You'll use it in Challenge 1 to bootstrap your `coffee-feature-decomposer` skill.

## 3. Connect to the JIRA MCP server

Your facilitator hands you:
- The MCP server endpoint
- Auth credentials
- **Your team identifier** (e.g. `T1`, `T2`, ...) — pin this down. You'll use it on every ticket.

Write your team identifier here so you don't lose it: **`T___`**

Wire these into your Copilot configuration following the projector instructions. You'll test the connection in Challenge 0.

## You're ready when…
- `apm --version` works
- Copilot can list `skill-creator` as an available skill
- You know your team identifier
- The JIRA MCP server is configured (even if untested — Challenge 0 tests it)

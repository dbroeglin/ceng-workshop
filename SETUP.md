# Setup — do this before the workshop starts

You need three pieces working before Challenge 0:

1. **APM** — [Agent Package Manager](https://github.com/microsoft/apm) CLI
2. **`skill-creator`** — installed via APM
3. **JIRA MCP server** — connection details from your facilitator

If any of these fails during setup, raise it BEFORE the workshop. Five quiet minutes of pre-flight beat 50 minutes of frustration.

## 1. Install APM

APM is the open-source Agent Package Manager (see [microsoft/apm](https://github.com/microsoft/apm)) — a CLI for installing and managing agent skills, prompts, and MCP servers.

Install it locally with the official one-liner:

- **Linux / macOS:**
  ```bash
  curl -sSL https://aka.ms/apm-unix | sh
  ```
- **Windows (PowerShell):**
  ```powershell
  irm https://aka.ms/apm-windows | iex
  ```

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
> What skills do I have access to?

You should see `skill-creator` in the list. You'll use it in Challenge 1 to refine the `coffee-feature-decomposer` skill scaffold that already lives at [skills/coffee-feature-decomposer/SKILL.md](skills/coffee-feature-decomposer/SKILL.md).

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

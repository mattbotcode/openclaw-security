# openclaw-security

Curated security skills for OpenClaw. Forked from [vamsiravuri/openclaw-security](https://github.com/vamsiravuri/openclaw-security) with only the skills relevant to this setup.

## Included Skills

### Enforcement (block dangerous patterns)
- **command-guard** — Blocks fork bombs, recursive deletes, reverse shells, pipe-to-shell
- **data-exfiltration-guard** — Blocks secrets (AWS keys, SSH keys, tokens) in outbound requests
- **security-validation** — Final gate before exec/write/edit combining the above checks

### Detection (observe and report)
- **prompt-injection-detector** — Flags injection attempts in external content
- **denial-of-wallet-guard** — Monitors for runaway agent loops and excessive token usage

### Automation
- **security-scan-scheduler** — Orchestrates Sentinel's daily security scan (threat intel, skills audit, config audit)
- **skill-security-scanner** — Pre-install scanning with blocklist of known malicious skills

## Usage

Skills are installed to `~/.openclaw/skills/`. Sentinel checks this repo daily for updates.

## Maintenance

This is independently maintained. Upstream changes from `vamsiravuri/openclaw-security` are cherry-picked only when relevant.

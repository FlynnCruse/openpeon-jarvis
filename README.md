# J.A.R.V.I.S. — OpenPeon Sound Pack

A CESP v1.0 sound pack for [peon-ping](https://github.com/PeonPing/peon-ping). 45 voice lines inspired by Paul Bettany's JARVIS from the MCU — calm, dry, never panicked.

> "I've also prepared a safety briefing for you to entirely ignore."

## Install

**If you already have peon-ping:**

```bash
peon packs install jarvis
peon packs use jarvis
```

**Manual install (any OS):**

```bash
git clone https://github.com/FlynnCruse/openpeon-jarvis.git
```

Then copy to your peon-ping packs directory:

```bash
# macOS / Linux
cp -r openpeon-jarvis ~/.claude/hooks/peon-ping/packs/jarvis

# Windows (PowerShell)
Copy-Item -Recurse openpeon-jarvis $env:USERPROFILE\.claude\hooks\peon-ping\packs\jarvis
```

Set it as active:

```bash
peon --pack jarvis
```

## Verify

```bash
peon --status          # should show "pack: jarvis"
peon preview           # hear one from each category
```

## Categories

| Event | Sounds | Example |
|-------|--------|---------|
| `session.start` | 5 | *"Welcome home, sir."* |
| `task.acknowledge` | 8 | *"For you, sir, always."* |
| `task.complete` | 7 | *"As always, sir, a great pleasure watching you work."* |
| `task.error` | 7 | *"That's broken. Which does narrow things down considerably."* |
| `input.required` | 7 | *"I've reached the part that requires a human. You'll do."* |
| `resource.limit` | 5 | *"Sir, I think I need to sleep now."* |
| `user.spam` | 6 | *"I am aware. I remain aware. I will continue to be aware."* |

**45 lines total** — 16 canon MCU quotes + 29 original lines written in JARVIS voice.

## Supported Tools

Works with any tool that supports peon-ping: Claude Code, Codex, Cursor, Windsurf, Kiro, Copilot, Gemini CLI, and more.

## Voice

Generated with [ElevenLabs](https://elevenlabs.io) using a custom JARVIS voice clone (`eleven_multilingual_v2`, 44.1kHz MP3).

## Disclaimer

This is a fan project. JARVIS and related characters are property of Marvel/Disney. Voice generated via ElevenLabs. Not affiliated with or endorsed by Marvel, Disney, or Paul Bettany.

## License

CC-BY-NC-4.0

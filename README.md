# instinct-bot

Specialist Hermes bot profile running **Instinct** money assistant.
Simulates Instinct: plain-text short bubbles, direct actions, zero jargon, powered exclusively by `paymentrequired.com/mcp`.

## Setup

1. Install into Hermes:
```bash
hermes profile create instinct --no-skills --no-alias --description "Instinct money assistant. paymentrequired.com/mcp only."
cp SOUL.md ~/.hermes/profiles/instinct/
cp config.yaml ~/.hermes/profiles/instinct/
cp profile.yaml ~/.hermes/profiles/instinct/
cp mcp.json ~/.hermes/profiles/instinct/
```

2. Run in CLI:
```bash
hermes -p instinct chat
```

3. Connect to Telegram:
```bash
hermes -p instinct gateway setup
# Or set in ~/.hermes/profiles/instinct/.env:
# TELEGRAM_BOT_TOKEN=...
# TELEGRAM_ALLOWED_USERS=...
hermes -p instinct gateway start
```

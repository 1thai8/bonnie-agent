# Bonnie Agent — n8n Workflow

AI receptionist for aesthetic clinics. Books and cancels appointments via WhatsApp automatically.

## Setup

1. Import `bonnie-agent.json` into your n8n instance
2. Configure credentials:
   - Anthropic API (Claude Haiku)
   - Google Calendar OAuth2
   - Google Sheets OAuth2
   - Gmail OAuth2
   - Twilio (HTTP Basic Auth)
3. Start n8n with correct timezone:

```powershell
$env:GENERIC_TIMEZONE="Europe/Madrid"; $env:TZ="Europe/Madrid"; npx n8n
```

## What it does

- Checks real-time availability before confirming bookings
- Creates and deletes Google Calendar events
- Saves patient leads to Google Sheets
- Sends WhatsApp confirmation via Twilio
- Notifies clinic via Gmail
- Responds in Spanish, Galician or English

## Tech Stack

n8n · Claude Haiku 4.5 · Twilio WhatsApp · Google Calendar · Google Sheets · Gmail

---

**Live demo:** [auto-scaleai-six.vercel.app](https://auto-scaleai-six.vercel.app)  
**Landing page repo:** [bonnie-landing](https://github.com/1thai8/bonnie-landing)

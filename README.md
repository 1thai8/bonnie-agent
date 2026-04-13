# Bonnie Agent — n8n Workflow

AI receptionist workflow for aesthetic clinics. Handles booking and cancellations via WhatsApp.

## How to use

1. Import `Bonnie_FINAL.json` into your n8n instance
2. Configure credentials: Google Calendar, Google Sheets, Gmail, Twilio, Anthropic
3. Start n8n with Europe/Madrid timezone:

```powershell
$env:GENERIC_TIMEZONE="Europe/Madrid"; $env:TZ="Europe/Madrid"; npx n8n
```

## What it does

- Checks availability before booking
- Creates/deletes Google Calendar events
- Saves leads to Google Sheets
- Sends WhatsApp confirmation via Twilio
- Notifies clinic via Gmail
- Responds in Spanish, Galician or English

## Tech Stack

n8n · Claude Haiku · Twilio · Google Calendar · Google Sheets · Gmail

---

**Landing page:** [auto-scaleai-six.vercel.app](https://auto-scaleai-six.vercel.app)  
**Full project:** [bonnie-landing](https://github.com/1thai8/bonnie-landing)

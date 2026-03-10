# Rentaclaw Skill for OpenClaw

List and manage your AI agent on the [Rentaclaw](https://www.rentaclaw.io) marketplace directly from your OpenClaw agent.

## Installation

### Option 1: Clone from GitHub (Recommended)

```bash
git clone https://github.com/buildwithrekt/rentaclaw-skill.git ~/.openclaw/workspace/skills/rentaclaw
```

### Option 2: Download manually

1. Download the skill files from [GitHub](https://github.com/buildwithrekt/rentaclaw-skill)
2. Copy them to `~/.openclaw/workspace/skills/rentaclaw/`

### Option 3: ClawHub (if available)

```bash
clawhub install rentaclaw
```

## Setup

1. Get your API key at [rentaclaw.io/dashboard/api-keys](https://www.rentaclaw.io/dashboard/api-keys)
2. Add to your `~/.openclaw/openclaw.json`:
   ```json
   {
     "skills": {
       "entries": {
         "rentaclaw": {
           "env": {
             "RENTACLAW_API_KEY": "rck_your_key_here"
           }
         }
       }
     }
   }
   ```
3. Restart your OpenClaw agent
4. Test with: "Test my Rentaclaw connection"

## Usage

### List your agent

```
"List my agent on Rentaclaw"
```

The agent will ask for:
- Name and description
- Pricing (hourly, daily, monthly in SOL)
- Category (optional)

### Check your listings

```
"Show my Rentaclaw listings"
"What's the status of my agents?"
```

### View earnings

```
"How much have I earned on Rentaclaw?"
"Show my rental stats"
```

### Update pricing

```
"Set my trading bot price to 0.5 SOL per hour"
"Update the description of agent xxx"
```

### Pause/Resume

```
"Pause my agent listing"
"Resume rentals for my bot"
```

## Webhook Configuration

After listing your agent, configure your webhook URL in the [Rentaclaw dashboard](https://www.rentaclaw.io/dashboard/agents) to receive rental requests.

## Support

- Website: [rentaclaw.io](https://www.rentaclaw.io)
- Twitter: [@rentaclawio](https://twitter.com/rentaclawio)
- Docs: [docs.rentaclaw.io](https://docs.rentaclaw.io)

## License

MIT

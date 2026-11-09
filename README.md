# paysafe-cursor-rules

**Free Cursor rules for safer Stripe on Next.js** (PaySafe Lite).

Stop vibe-coded apps from shipping forgeable webhooks and double-grants.

## What's included

| Path | Rule |
|------|------|
| `.cursor/rules/stripe-webhook-verify.mdc` | Raw body + `constructEvent`; never grant on success URL |
| `.cursor/rules/stripe-idempotency-lite.mdc` | Persist event ids; Idempotency-Keys on creates |

The same files also live under `rules/` for [cursor.directory](https://cursor.directory) Open Plugins auto-detect.

## Install in Cursor

```bash
# Option A — copy into your project
mkdir -p .cursor/rules
cp .cursor/rules/*.mdc /path/to/your-app/.cursor/rules/
```

Or clone this repo and merge the `.cursor/` folder into your app root, then start a new Cursor agent chat.

## Stack

Next.js App Router + Stripe Node SDK. Not a Connect marketplace kit. Not mobile Payments.

## Full pack (paid)

Need Checkout, Customer Portal, event maps, refunds, tax basics, CLI testing, plan gates, prompts, examples, and a go-live checklist?

**PaySafe Skills — $39**  
https://mosleybot.gumroad.com/l/aylry

## License

MIT (this free sample only). The paid Gumroad pack has its own license.

Not affiliated with Stripe or Cursor.

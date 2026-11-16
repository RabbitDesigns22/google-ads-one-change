# google-ads-one-change

**When a small Google Ads campaign turns expensive, your agent checks the tracking first, then makes one small change with your yes and measures it before touching anything else.**

`google-ads-one-change` is an agent skill for Claude Code (and any agent that reads `SKILL.md` skills). It is for agencies and owners who run small Search campaigns, about 1-5 USD a day, where a few conversions a month decide everything.

Without it, an agent asked to "fix the campaign" tends to:
- change keywords, bids, budget and match types on the same day;
- trust a cost per conversion built on 2 conversions;
- blame the ads when the conversion tag or the button was broken;
- click "Apply" on Google's recommendations.

This skill gives it:
- **Measurable triggers:** CPA over 2x its own baseline, 3+ days of spend with no conversions, low CTR, junk search-term spend, limited or poor ads. The baseline comes from the campaign's own history or the same niche, never across niches.
- **A fixed diagnostic order:** tracking first, then search terms, negatives, ads, keywords and match types, schedule and location, and the landing page.
- **One change at a time.** Each change gets a written proposal, the owner's yes, a field-by-field read-back, a log line with the metric and the measurement date, and a 5-7 day wait. The wait follows Google's own learning-period rules, linked in the skill.
- **Hard rules:**
  - no auto-applied recommendations, auto-created assets or AI-generated text;
  - no budget increase to compensate for an expensive campaign;
  - no health or income promises.

## Install

```bash
npx skills@1.8.1 add https://github.com/RabbitDesigns22/google-ads-one-change/tree/547b177b7e120fcf83f9abef2569184d3fc82f13
```

Or copy `skills/google-ads-one-change/` into `~/.claude/skills/`.

## Works well with

- A negative-keyword skill for mining search terms (n-grams, match types, levels).
- A full account-audit or root-cause diagnostic skill when the 6 steps do not explain the problem.
- [`small-budget-ads`](https://github.com/RabbitDesigns22/small-budget-ads), the same "small budget, few conversions" logic for Meta Ads.

## Status and limits

Version 1. Built from the author's agency work: small-business Search campaigns that send people to WhatsApp or a phone call. The account owner asked for a way to improve weak accounts without "moving the campaigns so much".

- The 3% CTR and 20% junk-spend thresholds are the author's working numbers, not Google's.
- The skill does not connect to the Google Ads API. The agent reads the interface or your exports.
- It has not been measured over many accounts yet. Treat the triggers as a starting point and tune them to your niche.

MIT. Issues welcome.

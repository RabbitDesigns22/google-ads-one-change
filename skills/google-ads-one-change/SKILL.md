---
name: google-ads-one-change
description: >-
  Load when a live Google Ads Search campaign underperforms and the job is to IMPROVE it, not just audit it, especially on small budgets (about 1-5 USD a day) where conversions are few: "fix the campaign", "cost per conversion is too high", "no conversions for days", "optimize Google Ads", "it spends but nobody calls", "mejora la campaña", "no convierte". It gives measurable triggers (CPA over 2x its own baseline, 3+ days of spend with no conversions, low CTR, junk search terms, limited or poor ads), a fixed diagnostic order that starts with checking the conversion tracking itself, then search terms, negatives, ads, keywords and match types, schedule and location, landing page, and then ONE small change with the owner's written yes, read back field by field, logged with what it measures and when, and a 5-7 day wait before the next one (based on Google's own learning-period rules). Not for building a new campaign, not for Meta Ads, not a full account audit.
license: MIT
---

# Google Ads: improve a weak campaign one change at a time

A small campaign gets few conversions. When it turns expensive, the temptation is to change everything at once: new keywords, a new bid strategy, a bigger budget, broad match "to get data". Then nobody knows which change helped, the bid strategy goes back into learning, and the client pays for the experiment. This skill forces the opposite: **look first, make one small change with a yes, and measure it before touching the next thing.**

If a rule from the account owner or the client contradicts this skill, the owner's rule wins.

## 1. Does it need improving? (any one trigger)

Read every number yourself, on screen, with the exact date range Google shows, for the same campaign.

| Trigger | How to measure it |
|---|---|
| Expensive conversions | Cost per conversion over the last 14 days **> 2x its baseline** |
| Spend without conversions | **3+ days in a row** with spend and 0 conversions, or spend without a conversion above 2x the baseline |
| Low CTR | With 200+ impressions in 7 days, Search CTR under half of the account's best 30 days. No history: under 3% (a working threshold, not a Google number) |
| Junk search terms | 20%+ of 7-day spend on terms that cannot buy (another city, "what is", free, jobs, DIY) |
| Something limited | An ad or keyword "Disapproved", "Eligible (limited)", ad strength "Poor", or "Low search volume" |

**Baseline**, in this order:
1. The same campaign's previous 30 days.
2. With no history: accounts **in the same niche**. A WhatsApp click for a supplement and a call for a repair do not cost the same, so comparing across niches calls normal "expensive".
3. Whenever you write "average", say which accounts and which dates.

**Too little data:** with fewer than 3 conversions in 14 days, cost per conversion is noise. Two conversions more or less halve it or double it. Do not touch bids or budget then; the change goes to search terms, negatives, ads or tracking.

Quick math: daily budget ÷ cost per conversion = conversions per day. At 3 USD a day and 12 USD per conversion that is 0.25 a day, so Smart Bidding has almost nothing to learn from, and every junk term weighs a lot.

## 2. Before changing anything

1. **May this account be changed at all?** Some owners freeze accounts ("leave it as it is"). Then you only report: urgent items (a disapproved ad, no funds, the landing page down), and no proposals.
2. **When was the last change?** Open the change history.
   - If the last change in that campaign was to **ads, copy, negatives, schedule or location**, wait **at least 5 days** before the next one.
   - If it **added or removed keywords, or changed the bid strategy or the conversion goal**, wait **7 days**.
   - Until then, make no other change. Write down when the next one is due.
   - Why: per Google, adding or removing keywords, a new or reactivated strategy, and a significant goal change put the bid strategy "in learning" for up to 7 days. Budget, target, creative and targeting changes do not. Judge the result after 2 weeks or 2 conversion cycles, whichever is longer ([Google Ads Help](https://support.google.com/google-ads/answer/13020501)).
3. **Does tracking work?** A campaign "with no conversions" may simply have a broken button or tag.
   - Open the landing pages: each returns 200.
   - The conversion tag (AW-…) and its label are on each page.
   - Every call or chat button points to the right number.
   - Measure page speed twice, and compare against a fast site. A slow local DNS once made every site, google.com included, look 12-20 s slow on the first try and under 1 s on the second. Never report "slow site" from one measurement.
   - Real sales come from the client, not from Google. Google only sees the click on the button.

## 3. Diagnose in this order

The order runs from what saves the most money and breaks the least to what moves the most.

1. **Search terms**, last 14 days: the 10 that spent most, and every term unrelated to the business.
2. **Negatives** from that list, with the right match type and level. First check the real service area: a nearby city the client does serve is a good term, not a negative.
3. **Ads and copy:**
   - Ad strength.
   - Headlines that echo the ad group's keyword.
   - Prices that match the landing page exactly.
   - Never leave one ad per group; replace the worst one with a new version.
4. **Keywords and match types:**
   - Pause keywords that spent 2-3x the baseline without converting.
   - "Low search volume" keywords do not spend, so they are not the problem.
   - Use phrase and exact match. Broad match only once conversions are plentiful.
5. **Schedule and location:**
   - Ads run when someone actually answers the phone or the chat.
   - Location targets "presence", people who are there, not "interest".
6. **Landing page and conversion:**
   - The ad and the page say the same thing.
   - The page is fast on a phone.
   - The conversion action counts what it should: one per click, the right category, and a value if there is one.

If none of these explains it, run a full root-cause diagnostic before you touch the budget. Never raise the budget "to see if it helps".

## 4. One small change, with a yes

1. **Pick ONE:** the change with the biggest expected effect from what you saw, that touches the smallest part of the account. Log the other candidates, in order, as "next".
2. **Propose it like this:**
   ```
   Account / campaign / ad group:
   Change:          (exact: the text, the keyword, the setting)
   Why:             (the number you saw, with its date range)
   Measured by:     (cost per conversion, CTR, junk-spend share...)
   Value before:    (last 14 days)
   Measured on:     (date, 14 days later)
   Not touched:
   ```
3. **Get the owner's written yes, change by change:** for enabling, budget, bids, keywords and negatives. Loading something **paused** is the only thing that needs no yes, and only when the owner asked for it.
4. **Apply it, reload, and read it back field by field.** Then check the change history: only that change should be there.

## 5. Hard rules
- **No auto-applied recommendations, no automatically created assets, no AI-generated text or "AI Max" expansion**, unless the owner turned them on in writing. They can insert brand names the client may not use, and claims the landing page does not make. Never click "Apply" on a recommendation as a shortcut.
- **One change per campaign every 5-7 days** (see 2.2).
- **Budget increases and enabling** only with the owner's written yes, never to compensate for an expensive campaign.
- **No health, income or results promises** in the copy.
- If Google disapproves something, read the reason and fix it. Do not appeal blindly.

## 6. Log and measure

Keep one line per change in the client's file:
```
YYYY-MM-DD HH:MM | change | why (number) | metric | value before | measured on YYYY-MM-DD | result: (pending)
```

On the measurement date, compare the same number of days before and after, then write the result:
- **better:** keep it;
- **same:** keep it, and the next candidate goes ahead;
- **worse:** propose undoing it, also with a yes.

## 7. Report (5 lines max, real local time)
```
Google Ads · <client> · <time>
Saw: <trigger with number and date range>; tracking <ok / broken>.
Changed: <the change, or "nothing: last change on <date>, next due <date>">.
Measured: <metric, value before, date>.
Waiting on: <the yes being asked for, or what the web or sales side must do>.
```
Before sending, check the currency, the account, the dates, and that you saw every number yourself.

## What this prevents
- Comparing niches and calling normal "expensive".
- Judging a campaign on 2 conversions.
- Four changes on the same day, so nobody knows which one worked.
- Blaming the ads when the button was broken.
- Raising the budget of an expensive campaign.
- Letting Google write copy or assets with a brand the client may not use.

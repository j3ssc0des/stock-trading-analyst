# Risk & Position Sizing Framework

Use this when the user is asking about how big to make a trade, where to put a stop, or how a trade fits with what they already own. Most blow-ups come from sizing mistakes, not stock-picking mistakes — take this section seriously.

## The core idea

You don't size a position by how much you want to make. You size it by how much you can afford to lose if you're wrong, and where the chart/thesis tells you that you're wrong.

The math:

```
Position size ($) = Risk per trade ($) / (Entry price − Stop price)  ×  Entry price
```

In words: how many dollars are you willing to lose on this trade? Divide that by the per-share loss you'd take at your stop. That's your share count. Multiply by entry price for the dollar size.

## Risk per trade

A common rule of thumb: risk no more than 1–2% of total trading capital on any single idea. If the user has $50k in trading capital and uses 1%, that's $500 of risk per trade — meaning the worst-case loss on the trade, from entry to stop, should not exceed $500.

This is a discipline tool, not a law. The point is that any individual idea — including the one you're highest-conviction on — should not be able to put you out of business.

## Where to put the stop

Stops should be placed *based on the chart and the thesis*, not based on a percentage. If the technical structure says "this setup is wrong below $98," the stop goes a bit below $98. If the thesis says "the bull case requires Q3 gross margin to come in above 45%," then poor margins are the stop, not a price level.

A stop that's too tight gets you knocked out by normal noise. A stop that's too wide makes the position size tiny and the trade unworkable. If you find yourself with no logical place to put a stop, that's a sign the trade isn't well-defined yet.

For volatile stocks, use ATR (Average True Range) as a sanity check — your stop distance should usually be at least ~1× the daily ATR to avoid being shaken out by ordinary moves.

## Risk/reward

Before sizing, sanity-check the math:

- **Reward** = (target price − entry price)
- **Risk** = (entry price − stop price)
- **R:R** = Reward / Risk

You want R:R of at least 1.5–2:1, ideally 3:1 for swing trades. If the next clear resistance is barely above your entry and your stop has to be wide, it's not a good trade — even if you're right about direction.

## Portfolio fit

Before adding a position, the user should ask:

- **Correlation** — Do I already own this exposure? Owning NVDA, AMD, AVGO, and TSM is one bet, not four. Concentration in correlated names is hidden leverage.
- **Sector weight** — How much of the portfolio is now in one sector? Tech-heavy is fine if intentional; tech-heavy by accident is a problem.
- **Cash level** — Does the portfolio have enough dry powder for opportunities and drawdowns?
- **Single-name max** — A common rule: no single position above 5–10% of portfolio (varies by conviction and account type).

## Common sizing mistakes to flag

- **Anchoring to dollar amounts** ("I'll put $10k in") rather than to risk. $10k in a stock with a 20% stop is $2k of risk; $10k in a stock with a 5% stop is $500. Same notional, very different risk.
- **Averaging down without a plan.** Adding to a losing position to "lower the cost basis" is fine if it was always part of the plan. It's a problem if it's an emotional response to being wrong.
- **Removing the stop because price is approaching it.** The stop existed because the thesis required it. Removing it means you've decided to be a long-term holder without admitting it.
- **Sizing based on conviction alone.** High conviction is a reason to take the trade, not a reason to make it huge. The math still has to work.

## Quick checklist when the user asks about sizing

1. What's the entry?
2. Where's the stop, and what specifically would have to happen to trigger it?
3. What's the rough first target?
4. What's the R:R?
5. What % of portfolio capital does this position represent at entry?
6. What % of portfolio capital is at risk (entry-to-stop loss)?
7. Does this overlap with positions the user already holds?

If you don't have answers to most of these, the user isn't ready to size the trade — they're still working out what the trade *is*.

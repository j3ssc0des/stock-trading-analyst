# Options Basics (read only if the user is trading options)

This is a quick reference to keep your analysis grounded. It's not an options course — if the user is asking detailed strategy questions and you're unsure, say so rather than guessing.

## What an option is

A call option is the right (not obligation) to buy 100 shares at the strike price by expiration. A put is the right to sell. The buyer pays a premium; the seller collects it.

## The Greeks (the ones that actually matter)

- **Delta** — How much the option price moves per $1 move in the underlying. A 0.50-delta call gains roughly $0.50 if the stock goes up $1. Delta also approximates the market-implied probability the option finishes in the money.
- **Theta** — Time decay. How much the option loses per day, all else equal. Theta accelerates as expiration approaches, especially in the last 30 days. If you're long premium, theta is the headwind.
- **Vega** — Sensitivity to implied volatility. Long options are long vega: they gain if IV rises. This is why options can lose money even when the stock moves in your direction (IV crush, especially after earnings).
- **Gamma** — How fast delta changes. Matters most for short-dated, near-the-money options. High gamma means wild P&L swings.

## Implied volatility (IV)

IV is the market's expectation of how much the stock will move, annualized. Pay attention to:

- **IV rank / IV percentile** — Where is current IV relative to its 1-year history? Buying options when IV rank is high (e.g., > 50) is expensive; selling premium then is more attractive. The opposite when IV rank is low.
- **IV crush** — IV typically inflates into known events (earnings, FDA decisions) and collapses immediately after. A long call can lose money post-earnings even if the stock goes up, if IV drops more than the move helps.

## Options-implied move

Around earnings, you can estimate the market-implied one-day move from at-the-money straddle pricing:

```
Implied move ≈ (ATM call price + ATM put price) / stock price
```

If NVDA is at $900 and the ATM straddle is priced at $63, the implied move is ~7%. This is a useful framing for any earnings-related trade — bulls need a move bigger than that to make money on long calls, after IV crush.

## When to mention what

- **Long calls / puts** — Highlight the delta, theta, and IV rank. Note the breakeven (strike + premium for calls, strike − premium for puts). Flag that they expire — this isn't stock.
- **Spreads (vertical, calendar, diagonal)** — Useful for defined-risk views. Note the max gain, max loss, and break-evens.
- **Selling premium (covered calls, cash-secured puts)** — Frame as income strategies with capped upside. Note assignment risk and that selling puts is functionally similar to a limit buy order with extra steps.
- **Iron condors / strangles / straddles** — These are vol bets. Long premium = betting on a big move; short premium = betting on quiet markets. If the user isn't thinking in IV terms, they shouldn't be doing these.

## Things to flag

- Single-name short premium can have unbounded losses (naked calls) or large losses (cash-secured puts). Make sure the user understands the risk profile before encouraging it.
- 0DTE / weekly options are essentially gambling instruments for most retail traders — high gamma, brutal theta, very narrow margin for being right. If the user is asking about them, frame them honestly.
- Options on illiquid stocks have wide bid/ask spreads that quietly eat returns. Always check open interest and spread.

## Limits of analysis

Options pricing involves more variables than stock analysis (vol surface, skew, term structure). Don't pretend to a precision you don't have. If the user asks something you can't answer well — exotic strategies, specific Greek calibrations, complex multi-leg P&L — say so and suggest they look at a dedicated tool (their broker's analytics, optionstrat.com, etc.).

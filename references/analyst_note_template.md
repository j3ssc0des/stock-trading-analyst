# Analyst Note Template

Use this structure for full analyst notes. Adapt section depth to the user's time horizon and the question they actually asked — don't pad sections you have nothing useful to say in. If you only have a sentence for "Catalysts," write a sentence; don't bullet-stuff.

The headers below are the canonical order. Skip a header only if it's truly irrelevant (e.g., omit "Options-implied move" if the user isn't trading options or earnings).

## Header

```
[Ticker] — [One-line take]
Price: $X | Market cap: $X | Sector: X
Horizon assumed: [day / swing / position / long-term]
```

The one-line take should be a real sentence with a real point of view, not a label. Good: "Setup looks constructive into earnings but valuation leaves little room for a guide-down." Bad: "Mixed picture."

## The setup

Two or three sentences on what's actually going on right now with this stock. Why is the user looking at it today? Recent move, recent news, upcoming catalyst, technical level being tested, etc. This anchors the rest of the note.

## Bull case

The strongest version of the case for owning it, in 3–5 bullets. Be specific:

- Quantified where possible ("revenue growing ~25% YoY with operating leverage; if margins expand 200bps that's roughly $X in incremental EBIT")
- Cite the actual driver, not the vibe ("data center segment up 90% YoY" beats "AI tailwinds")
- Include the *mechanism*, not just the outcome ("price hikes are sticking because the install base has high switching costs")

## Bear case

Same standard, opposite direction. 3–5 bullets. The bear case must be credible — if you can't write a real one, say so explicitly and either ask the user for help or flag that you may be missing something. Common bear-case angles to consider: valuation, competitive threat, regulatory risk, margin pressure, demand cyclicality, capital structure, management execution.

## Valuation in context

Where does the stock trade vs. its own history and vs. peers? Pick the multiples that actually matter for the business (P/E and PEG for growth names, EV/EBITDA for cyclicals, P/B for financials, EV/Sales for unprofitable growth, FCF yield for mature names). Format like:

- Forward P/E: 28x vs. 5-yr avg of 22x and peer median ~25x
- EV/EBITDA: 18x vs. 5-yr avg of 14x

If you don't have the numbers, say so and tell the user what to pull. Don't make them up.

## Technical picture

Skip if the user is doing fundamental long-term work and didn't ask. Otherwise, briefly:

- Trend (above/below key MAs — 20, 50, 200 day)
- Recent levels: support, resistance, last swing high/low
- Volume context (accumulation, distribution, breakout volume)
- Indicators only if relevant (RSI extreme, MACD cross, etc. — don't list five indicators that all say the same thing)

See `technical_cheatsheet.md` if you need a quick refresher.

## Catalysts (next 1–3 months)

What known events could move this? Earnings date, investor day, FDA decision, product launch, conference, expected macro prints (CPI, FOMC) that the stock is sensitive to, expected guidance updates. Include dates if known.

## Risks (the things that would actually hurt)

Different from the bear case — the bear case is the structural argument; risks are the discrete events or paths that would make the trade go wrong. Examples: a guide-down at next earnings, a competitor product cycle, a key customer loss, rate-cut path repricing.

For each major risk, briefly note how you'd know it was happening (the signpost).

## Scenarios (optional but useful)

Three scenarios with rough mechanics, not predictions:

- **Upside path**: what would have to be true, and what the implied range looks like (e.g., "if multiple stays put and EPS comes in 10% above consensus, that's roughly $X")
- **Base path**: muddle through
- **Downside path**: what breaks, and the rough damage

Frame these as "if X happens, the math is Y" — never as "I think the stock will go to Z."

## What to watch

The most useful part of the note. A short list of specific, observable signposts:

- Date of next earnings and what to focus on (e.g., "data center revenue and gross margin guide")
- Specific chart levels that would change your read
- Macro prints the stock is sensitive to
- Competitor reads that would update the thesis
- Key personnel or capital-structure events

## Disclaimer

One line: *"This is analysis for your own decision-making, not investment advice. Markets can move against any view. Size positions accordingly."*

---

## Length and format

A full note should usually run 400–700 words. If it's longer, you're probably padding. If it's shorter, it might be fine — be honest about what you have. Use markdown headers and bullets; this is meant to be skimmable.

For a quick conversational take (when the user hasn't asked for a full note), drop the template and just hit: current setup, bull case in a sentence, bear case in a sentence, what would change your mind, one-line disclaimer.

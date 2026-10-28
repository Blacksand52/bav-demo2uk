# BAV improved demo package

This is the original BAV sandbox with messaging and flow changes aimed at sceptical UK students.

## What changed

### About page (`about/index.html`)
- Hero rewritten: “Most of us spend the rent money by week six…”
- Clearer what it is / isn’t / where it’s at (includes path to real accounts if the idea works)
- Outcome contrast strip (without vs with a hard split)
- How-to steps prioritise the decline moment and single-device use
- Footer states product direction explicitly

### Interactive demo (`index.html`)
- New headline and sub: “try the hard split”
- Intro guide box: 3 steps to feel the point in 2 minutes
- Wallet tabs renamed: “Rent & essentials” / “Spending money”
- Card labels: protected vs capped
- Till copy nudges users toward a large discretionary purchase
- Loan-date section framed as “Make it about your term”
- Links point to the local about page

## How to try it

1. Open `index.html` in a browser (or serve the folder).
2. Firebase is already configured for the live sandbox URL in the original project. Sessions still sync if that backend is up.
3. Follow the intro guide: set a loan date → Till → large spending item → watch the decline.
4. One device is enough: toggle Wallet Card / Till at the top.

## Original assets kept
- `bav-demo.mp4` walkthrough
- `bav-poster.jpg`
- `database.rules.json`

### End-of-session summary (added)
- Appears on Wallet Card and Till after the first approved or declined payment
- Shows essentials left, spending money left, and days until next payment
- Prompt: whether the hard split would have changed last term
- CTA to 1-minute feedback; “Keep trying” dismisses for the rest of the session
- `tx_count` / `summary_dismissed` added to session state (see `database.rules.json`)

## Not changed (on purpose)
- Core payment / decline / freeze logic
- Catalog prices and wallet assignments
- Firebase session model
- Feedback and tester forms (still collect the same fields)

Next product steps (not in this package): personal default loan dates by term, shareable session links in the UI, end-of-session summary card.

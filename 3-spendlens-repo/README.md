<div align="center">

# SpendLens

**Behavioural spend intelligence for Indian households.**

Most money apps tell you what you spent. SpendLens tells you what you must not touch.

[**Live app**](https://akr246.github.io/spendlens-ai-spend-intelligence/) · [**Case study**](https://akr246.github.io/case-studies.html) · [**Portfolio**](https://akr246.github.io)

</div>

---

## The problem

Indian households have more visibility into their spending than ever and less control over it. Budgeting apps categorise the past — they report that ₹9,400 went on food delivery last month, which the user already suspected — and stop there. None of them model the behaviour that produced the number.

The consequence is not that people overspend. It is that discretionary spending quietly outcompetes obligations. Rent gets paid because it must. The emergency fund loses every month to a hundred small decisions that each felt reasonable alone.

## What it does

Every rupee is classified into one of four bands:

| Band | Meaning | Product behaviour |
|---|---|---|
| **RED** · Essential | Shelter, health, food, education | Protected. Shown with funded state and days to due. Never the target of a reduction. |
| **GREEN** · Flexible | Dining, travel, fashion, subscriptions | Measured against an envelope. Leaks named with real transactions. |
| **AMBER** · Undecided | Mixed baskets, cash, self transfers | Genuinely ambiguous. Routed to review rather than guessed. |
| **GROW** | Savings and investments | Counted as progress, never as spend. |

Then it does the part that makes it different: it takes a stated financial goal and returns an honest verdict on whether it is reachable — and where it is not, three trade-offs drawn from the user's own spending, each with the rupees freed and the months saved.

## My role

Sole contributor. Problem framing, requirements, the classification taxonomy, success metrics, and the build — using AI-assisted development.

## Architecture

Six deterministic engines, each with a stated fallback:

```
INTERFACE          what the person actually sees
GUARDRAIL          vetoes an output before delivery
DECISION ENGINES   a model, and a rules fallback
CLASSIFICATION     assigns a label and a confidence
INGESTION          normalise · de-duplicate · reconcile
SOURCE SYSTEMS     raw records arrive
```

**Three decisions worth defending:**

1. **A confidence threshold.** Every classification carries a score. Below 0.6 the transaction goes to a human review queue instead of rendering. A confident wrong answer costs more trust than an honest question, and unlike a missing answer you do not recover from it.

2. **A fallback under every model.** Each model-dependent layer has a rules-based path that ships on its own. The fallbacks were built first — if you cannot ship the fallback alone, you do not have a fallback, you have an outage waiting for a name.

3. **A guardrail with veto power.** A separate service sits between the engines and the interface and blocks any recommendation touching an essential expense. It is deliberately separate code, because a guardrail that lives inside the thing it guards is not a guardrail.

## Stack

React 18 · TypeScript · Vite · Tailwind · hand-rolled SVG charts (no charting dependency) · GitHub Actions → GitHub Pages

Entirely client-side. No server, no account, no network call, no analytics — which is the only honest architecture for a demo that invites you to import a real bank statement.

## What I would change

While writing the PRD I found Ghosh and Huang's work on dynamic budget monitoring. Two of their findings land directly on this build: multiple category budgets *increased* spending where a single overall budget reduced it, and precise figures accelerated spending where ranges did not. This ships both.

Five of the six interventions they tested did work, so the paper became the v2 specification — one envelope, range display, roll-over, shorter windows. Finding that was more useful than any feature I could have added.

## Running it locally

```bash
npm install
npm run dev
```

## Note on the name

The repo says "AI" but the engines here are deterministic — rules and heuristics with confidence scoring, not trained models. That is a sequencing decision: every model in the spec needs a shippable fallback, and building the fallbacks first proves they work. There is no training corpus yet, so a model would be theatre.

---

*Built by [Arya K. Ravi](https://akr246.github.io) · Bengaluru*

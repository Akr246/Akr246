# Projects

A running index of what I've built and what each one was actually for.
Live portfolio: **[akr246.github.io](https://akr246.github.io)** · Case studies: **[akr246.github.io/case-studies.html](https://akr246.github.io/case-studies.html)**

---

## SpendLens — behavioural spend intelligence

**[Live app](https://akr246.github.io/spendlens-ai-spend-intelligence/)** · **[Code](https://github.com/Akr246/spendlens-ai-spend-intelligence)** · **[Case study](https://akr246.github.io/case-studies.html)**

**Problem.** Indian households can see what they spent and still cannot control it. Every budgeting app categorises the past; none model the behaviour that produces the next overspend, and discretionary spending quietly outcompetes obligations.

**My role.** Everything — problem framing, requirements, the classification model, success metrics, and the build itself. React and TypeScript, deployed through GitHub Actions, using AI-assisted development.

**Stack.** React 18 · TypeScript · Vite · Tailwind · hand-rolled SVG charts · zero charting dependencies · static deploy to GitHub Pages. Entirely client-side — no server, no account, no network call.

**Key decisions.**

- *A confidence threshold.* Every classification carries a score; below 0.6 it routes to a human review queue rather than rendering. A confident wrong answer costs more trust than an honest question.
- *A fallback under every model.* Each model-dependent layer has a rules-based path that ships on its own. I built the fallbacks first — if you cannot ship the fallback alone, you do not have one.
- *A guardrail with veto power.* Separate code between the engines and the interface, blocking any recommendation that touches an essential expense.
- *Client-side by necessity.* The product invites you to import a real bank statement. Nothing can leave the device, which ruled out any server architecture.

**What I learned.** While writing the PRD I found experimental evidence that category-split budgets and precise figures both *increase* spending — two findings that land directly on what I built. The paper became the v2 specification rather than an objection. Reading the literature that argues against a product, before the literature that supports it, is now how I start.

---

## Process Modelling & System Implementation

Client onboarding blueprint. Turned business requirements into access-provisioning checklists and milestone-tracking dashboards; automating the document handling cut processing time by 40%.

**Skills.** Requirements gathering · process modelling · workflow automation · stakeholder mapping

---

## Information Flow Optimisation

An LLM-based workflow for generating B2B communications, with data models tracking campaign metrics and response rates through automated CRM pipelines.

**Skills.** Workflow design · LLM application · data modelling · CRM automation

---

## Professional work, written up

These are from employed roles rather than side projects, and are documented as case studies because the reasoning is the interesting part.

| Work | Where | Read |
|---|---|---|
| Billing workflow automation — SAP BW → Snowflake → AWS S3, 20% efficiency gain | Align Technē | [Case study](https://akr246.github.io/case-studies.html) |
| A/B validated safety intervention — 30% risk reduction in high-risk scenarios | Annalect India | [Case study](https://akr246.github.io/case-studies.html) |

---

## In progress

Two projects currently being built:

- **Behavioural teardown series** — behavioural design analysis of three Indian consumer apps: defaults, friction, loss aversion, dark patterns
- **App store review mining** — NLP theme classification of public reviews across three fintech apps, ending in a prioritised fix list

---

*Last updated August 2026*

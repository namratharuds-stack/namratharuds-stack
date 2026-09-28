# Namratha Rudrappa

**Senior Product Manager · Applied AI for CPG Commercial Execution**
7.5 years building enterprise B2B SaaS · 2024 Stevie Award, AI Product of the Year · MBA, IIM Indore

[Portfolio](https://namratharudrappa.com) · [LinkedIn](https://www.linkedin.com/in/namratha-rudrappa-6176a4112) · [FieldIQ live demo](https://fieldiq-pro-pilot.lovable.app) · namratha.ruds@gmail.com

---

I build AI products for the people who sell and execute in CPG: field reps, revenue managers, trade-promotion teams. My work sits where a pricing insight or a shelf gap has to become an action someone takes in the next 30 seconds.

> Field users don't want more dashboards. They want fewer decisions.

## What I'm building now

### FieldIQ: an AI field-selling platform for CPG reps
Solo build, 2026. I took it from problem definition to a shipped prototype: discovery, PRDs, UX, prompt design, evals, and integration.

| Agent | What it does |
|---|---|
| **Draft Order Agent** | Proposes an order with a reason code and the supporting numbers on every line. The rep edits and submits; contract achievement recalculates live. |
| **CommCheck** | Pre-visit intelligence sorted into *Act Today*, *Opportunity*, and *Escalate*. |
| **Territory Pulse** | A ten-second daily read on territory position, trajectory, and concentration. |
| **Closed-loop Loss Analysis** | Turns a rejected order, lost display, dropped listing, or declined promo into a five-factor post-mortem and a next-order adjustment. Nothing feeds back until the rep confirms it. |

**How it's built**
- Model-agnostic gateway with server-side inference. Keys never reach the client.
- A strict JSON contract per agent, with typed fallbacks for rate limits, malformed output, and network errors.
- Gemini 2.5 Flash over a frontier model. Structured drafting on a phone needs fast, rule-following responses more than deep reasoning.
- Guardrails live in code, not in the prompt: no unauthorized SKUs, pack and MOQ rounding, and a hard block on auto-committing an order.

**How I know it works**
- **Draft Order eval:** 26 hand-adjudicated golden cases across 13 categories. Ship gate: zero critical failures and ≥90% pass. The seeded sample scores 22/26 with 3 critical failures, so the gate fails on purpose. Catching those misses is how you know the harness works.
- **CommCheck eval:** 19 cases across schema, rule-adherence, and adversarial layers, including prompt-injection probes. It found a format instruction with 0% compliance across all 19 runs. It also found a failure that turned out to be a bug in my own spec, not the model.

> Prohibitions in a prompt are requests. Format has to be enforced by construction.

### Redline: contract review
[Live app](https://redline-sigma-five.vercel.app) · [Code](https://github.com/namratharuds-stack/redline)
Upload a contract, lease, or freelance agreement. Redline flags the risky clauses, quotes the exact sentence each one came from, and drafts a counter-offer for each.

## What I've shipped before

**Tata Consultancy Services · 2018–2025**
Business Analyst → Product Owner → Product Manager & GTM Lead

- **AI revenue growth management platform.** Won the 2024 Stevie Award for AI Product of the Year. It runs on each customer's own LLM and data through RAG instead of shipping a proprietary model, which answered the data-residency and lock-in objections that were stalling deals. It recommends and never acts on its own: every consequential action goes through a human approval gate. It won four additional deals in six months and reached 10+ customers over two years, with $250M in customer savings across 5+ deployments.
- **56 tools → 1 platform, 22 countries.** A 0→1 mobile sales-execution platform covering ~75% of the client's global revenue. Adoption stalled at 60%. I went into the field, found the global build had dropped functions local markets needed, and rebuilt those as configuration. Adoption reached 70%.
- **Killed an ML pilot.** Salesforce Einstein routed reps by proximity rather than business need. I replaced it with a rules-based scoring model, and reps went from 4 to 7 calls per day.
- **Computer vision for shelf compliance.** Detection → CRM opportunity → field action → verification that the gap actually closed. About 30% more outlets hit SKU-mix targets and about 20% more hit promotion-mix targets.
- **B2B commerce portal on Salesforce Commerce Cloud.** 200K+ business buyers, live in under 9 months. 15% CSAT lift and ~18% repeat-order uplift.

## How I think about AI products

- **Autonomy should match the cost of being wrong.** A wrong autonomous pricing action can breach a contract before anyone notices. The agent drafts and the human approves.
- **Evals test the spec, not just the model.** Underspecified rules don't produce no behavior. They produce unowned behavior.
- **Adoption is a product design problem, not a training problem.**
- **Not every problem needs a model.** Sometimes the rules-based version ships and gets adopted while the ML pilot stalls.

## Toolkit

**Applied AI:** agentic workflows · RAG orchestration · structured outputs · eval & guardrail design · human-in-the-loop governance · model selection on latency and cost
**Product:** 0→1 builds · multi-market platform strategy · JTBD discovery · experimentation · GTM
**Tools:** Salesforce Commerce & Marketing Cloud · SQL · Mixpanel · Figma · Python

## Education

MBA, IIM Indore · B.E. Electrical Engineering, BMSCE Bangalore · Harvard Business School Online, *Winning with Digital Platforms* · Anthropic Academy, Agentic AI · Google AI Essentials

---

📍 New Jersey / NYC metro · Open to Senior PM and AI Product roles in CPG and CPG-vertical SaaS

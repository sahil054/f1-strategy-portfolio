# F1 Strategy Portfolio — Project Plan

**Goal:** Build a portfolio of projects demonstrating race strategy thinking (not just data science) for F1 Strategist/Lead Strategist internship & job applications.

**Core principle:** Every project should answer a racing question first, a technical question second. READMEs lead with "Was Ferrari's 2-stop the right call in Monaco?" not "built with pandas + sklearn."

**Skill level:** Beginner Python, learning as I go.
**Timeline:** Ongoing / long-term. Building depth, not rushing.

---

## Phase 1 (Months 1–2): Foundations + Race Post-Mortems
- Learn: pandas, matplotlib/plotly, FastF1 basics
- **Project 1: "Race Strategy Post-Mortems"** — pick 5–6 strategically interesting races, pull lap times/tires/pit stops via FastF1, plot degradation curves, identify undercut/overcut moments and quantify time gained, write "what I'd have called and why" for each.
- Output: Jupyter notebooks / blog-style write-ups on GitHub.

## Phase 2 (Months 2–4): Modeling
- **Project 2: Tire Degradation Model** — fit regression (linear/quadratic/piecewise) per compound per track. Reusable component for later simulator.
- **Project 3: Pit Stop / Undercut Calculator** — small interactive (Streamlit) tool: given gap + tire ages + degradation, compute the undercut window.

## Phase 3 (Months 4–7): Flagship Project
- **Project 4: Race Strategy Simulator (Monte Carlo)** — given track, tire options, degradation curves, pit loss, safety car probability (computed historically per track), simulate thousands of races per strategy option. Output: recommended strategy + probability distribution of outcomes (not just a single "optimal" answer).
- Backtest against real races from Phase 1 — compare model's recommended strategy vs. what actually happened/won, explain discrepancies.

## Phase 4 (Ongoing): Live Dashboard
- Wrap tools into a Streamlit/React dashboard: strategy simulator with adjustable inputs, degradation curve explorer, live-ish session data pull.
- This becomes the portfolio centerpiece link for resume/GitHub.

---

## Tools/Stack progression
pandas → matplotlib/plotly → FastF1 → scikit-learn (regression) → Monte Carlo/simulation logic → Streamlit

## Data source
- **FastF1** (Python) — telemetry, lap times, tire data (2018+ reliable)
- Built on **Jolpica-F1** API (replaced the now-retired Ergast API)

## Phase 1 races
- **01 — 2019 Hungarian GP** (Hamilton vs. Verstappen): Verstappen overcut too far into a long second stint, losing his time cushion to tire degradation before being forced to pit with nothing left to defend.
- **02 — 2019 German GP / Hockenheim** (Hamilton vs. Vettel): Hamilton's aquaplane/barrier incident cascaded into a 69s repair stop and a 5s penalty; Vettel's clean, error-free execution across 5 stops plus strong closing pace drove a P20→P2 recovery.
- **03 — TBD** (next up: 2021 Turkish GP — Bottas's intermediate-tire gamble)
- **04 — TBD**
- **05 — TBD**

## Phase 1 candidate races (not yet started)
- 2021 Turkish GP — Bottas intermediate tire gamble
- 2021 Azerbaijan GP — red flag / restart strategy
- 2022 British GP — mixed conditions, safety car timing
- 2023 Singapore GP — Sainz strategy win vs Mercedes/Red Bull

---

## Log / Changes
- **[Initial]** — Plan created.
- **[Update]** — Hungary 2019 and Germany 2019 analyses completed and pushed to GitHub.
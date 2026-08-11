# F1 Strategy Portfolio

Race strategy analysis built on real F1 telemetry data, working toward a Monte Carlo race strategy simulator. This is an ongoing project combining a long-standing passion for Formula 1 with data analysis, aimed at pursuing a career in F1 race strategy.

Each analysis leads with a racing question — not a technical one — then uses lap time, tire, and pit stop data to answer it with evidence.

## Race Analyses

| # | Race | Question | Key Finding |
|---|------|----------|-------------|
| 01 | [2019 Hungarian GP](notebooks/01_hungary_2019_undercut.ipynb) | How did Hamilton beat Verstappen without a single overtake? | Verstappen overcut too far into a long second stint, losing his time cushion to tire degradation before being forced to pit with no buffer left. |
| 02 | [2019 German GP](notebooks/02_germany_2019_wet_chaos.ipynb) | Why did Vettel recover from P20 to P2 while pole-sitter Hamilton finished outside the points? | Hamilton's single driving error cascaded into a 69-second repair stop and a time penalty; Vettel's five clean, error-free pit stops and strong closing pace drove the recovery. |

*More races in progress — see [PROJECT_PLAN.md](PROJECT_PLAN.md) for the full roadmap.*

## Roadmap
This is Phase 1 of a four-phase project:
1. **Race post-mortems** (current phase) — strategic case studies using FastF1 telemetry
2. **Tire degradation modeling + undercut calculator**
3. **Monte Carlo race strategy simulator**
4. **Live strategy dashboard**

Full details in [PROJECT_PLAN.md](PROJECT_PLAN.md).

## Tools
- [FastF1](https://github.com/theOehrly/Fast-F1): lap times, tire data, pit stops, race control messages
- Python (pandas, matplotlib)
- Jupyter Notebooks

## About
Built by Sahil Joshi. F1 strategy work is a genuine long-term interest, and this portfolio is an ongoing project, expect it to keep growing.
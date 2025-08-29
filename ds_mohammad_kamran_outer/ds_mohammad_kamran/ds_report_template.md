# Trader Behavior vs Market Sentiment — Findings

**Candidate:** Mohammad_Kamran  
**Date:** 2025-08-29

## 1. Executive Summary (≤ 200 words)
- 2–3 punchline insights with practical implications.

## 2. Data & Methodology
- Sources: Hyperliquid trades; Bitcoin Fear/Greed (daily).
- Cleaning: time parsing, UTC normalization, duplicates handling, missing values.
- Join logic: trade UTC date ↔ daily sentiment.
- Caveats: sampling periods, missing leverage/size, non-stationarity.

## 3. Descriptive Insights
- Volume, leverage, and win rate in **Fear vs Greed**.
- Which **symbols** and **sides** (long/short) out/under‑perform by regime.
- Top/bottom **accounts** and behavioral archetypes.

## 4. Statistical Evidence
- T‑tests / nonparametric checks for Fear vs Greed differences.
- Effect sizes (Cohen’s d) where relevant.

## 5. Predictive Modeling
- Models: Logistic Regression + Random Forest.
- Features: sentiment, leverage, size, side; interactions if any.
- Metrics: AUC, precision/recall; calibration.
- Feature importance + partial interpretations.

## 6. Event Study (Regime Switches)
- Fear→Greed and Greed→Fear windows (±3 days).
- Average PnL dynamics around switches.

## 7. Actionable Playbooks
- Example: "During **Greed**, reduce leverage on shorts; during **Fear**, size down longs on BTC‑perps; prefer mean‑reversion scalps" (replace with your findings).

## 8. Limitations & Next Steps
- Data coverage, survivorship bias, per‑account heterogeneity.
- Next: intraday sentiment, tail‑risk controls, position‑duration analysis, richer features.

## 9. Appendix
- KPI tables and figure thumbnails.

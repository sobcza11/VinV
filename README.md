<h1><p align="center">Value-<i>in</i>-Vogue ~ <i>VinV</i></p></h1>
<h4><p align="center">Dividend Persistence • Value Structure • Regime-Conditioned Equity Behavior</p></h4>

<p align="center">
  <img src="https://github.com/sobcza11/VinV/blob/main/_assets/vinv_m.png" alt="Value in Vogue Banner" width="90%">
</p>

---

## 🧭 **Overview**

**Value-<i>in</i>-Vogue (VinV)** is a **downstream, regime-conditioned equity research system** designed to evaluate **capital behavior of dividend-persistent, value-oriented equities** under **fixed macro-financial regimes**.

VinV is **descriptive, not predictive**.

It applies disciplined statistical & machine-learning methods **only after macro regimes are defined upstream**, translating observed equity behavior into **auditable, reproducible research artifacts** suitable for academic, institutional, & FinTech review.

VinV **does not forecast returns, optimize portfolios, or generate allocation signals**.

---

## 🧱 **System Context & Hierarchy (*Non-Negotiable*)**

VinV operates within a strictly ordered research stack:

1. **the_Spine**  
   Canonical macro-financial data fusion layer  
   *(single source of truth, frequency normalization, locked semantics)*

2. **FT-GMI**  
   Regime-aware macro-financial diagnostics  
   *(defines regimes & stress windows; read-only)*

3. **VinV** *(this repository)*  
   Equity behavior evaluation **conditioned on FT-GMI regimes**

4. **OracleChambers**  
   Interpretive narrative & validation layer only  
   *(no signal creation, no feedback upstream)*

**Dependency is strictly one-way:**  
`the_Spine → FT-GMI → VinV → OracleChambers`

VinV never alters upstream data, regimes, or diagnostics.

---

## 🧠 **What VinV Does (*& Does Not Do*)**

### ✅ VinV Does
- Evaluate equity behavior **within fixed macro regimes**
- Apply **time-respecting walk-forward validation**
- Translate probabilistic outputs into **portfolio-level descriptive outcomes**
- Produce **frozen, audit-ready artifacts**
- Prioritize stability, interpretability, & governance over model complexity

### ❌ VinV Does Not
- Forecast returns
- Time markets
- Optimize allocations
- Generate trading signals
- Feed outcomes back into diagnostics

---

## ⚙️ **Modeling Discipline (*Applied, Governed*)**

VinV uses machine-learning **as an implementation tool**, not an authority.

Modeling follows a deterministic ladder:
- Baselines → Linear → Tree → Boosted
- Leakage-safe preprocessing (X-only)
- Rolling features & winsorization
- Time-respecting walk-forward validation
- Empirical selection (no manual overrides)
- Portfolio-level evaluation (not point forecasts)

No deep learning.  
No novelty chasing.  
**Stability & governance dominate complexity.**

---

## 🗄️ Single Source of Truth (SSOT)

All VinV modeling derives from **frozen, canonical parquet artifacts** produced by the Spine.

```text
the_Spine/vinv/ssot/
├── vinv_ml_ssot_vFinal.parquet
├── vinv_modeling_view_vFinal.parquet
```


## 🏆 **Champion Model (*vFinal*)**

- Champion: tier1_logistic_l2
- Selection basis: highest walk-forward stability
- Final refit cutoff: 2025-11-01

The champion is selected **empirically, not heuristically**.

This reflects **maturity and governance discipline**, not underfitting.

## 🔒 **Final Refit & Freeze (*Audit-Ready*)**
```text
the_Spine/vinv/champion/vinv_champion_freeze_20251215T213325Z/
├── champion_model.joblib
├── champion_freeze_manifest.json
├── freeze_hashes_sha256.json
```

**Controls enforced**:
- Deterministic selection policy
- Timestamped freeze
- SHA-256 hash locking
- Git-tagged release

These artifacts constitute the primary empirical evidence for VinV.

## 🛡️ **CPMAI Alignment**

VinV aligns with **PMI-CPMAI principles**:

- Simpler methods before complexity
- Separation of data, diagnostics, & interpretation
- Full provenance & versioning
- Anti-leakage controls
- Immutable evidence artifacts

This repository intentionally contains:

- Code
- Results evidence
- Governance artifacts

Raw licensed data is excluded by design.

## 🚀 **What VinV Enables (*Post-Freeze*)**

Once FT-GMI is finalized, VinV can support:

- Cross-regime equity comparisons
- Stress-aware evaluation extensions
- Broader universes (e.g., WRDS-backed)
- Interpretive overlays via OracleChambers

All extensions preserve the same governance posture.

## 🎯 Positioning Summary

**VinV is a bounded, governed, regime-conditioned equity research system** that evaluates how equity constructions behave under defined macro contexts.

It is:

- Diagnostic, not predictive
- Applied, not promotional
- Stable, auditable, & review-ready

## ⚖️ **Disclaimer**

This repository is for research and educational purposes only.
It does not constitute investment advice, forecasts, or recommendations.

## 📎 **License**

MIT License


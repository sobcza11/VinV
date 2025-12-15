<h1><p align="center">Value-<i>in</i>-Vogue ~<i>VinV</i></h1>
<h4><p align="center">• Dividend Durability • Value Leadership • Macro-Regime Analysis •</p></h4>

<p align="center">
  <img src="https://github.com/sobcza11/VinV/blob/main/_assets/vinv_m.png" alt="Value in Vogue Banner" width="90%">
</p>


---

## 🧭 Overview
**Value-<i>in</i>-Vogue (<i>VinV</i>)** is a governed, macro-aware machine-learning equity ranking engine that converts **macroeconomic, positioning, factor, and energy signals** into **probabilistic tranche rankings**.

VinV is validated through **walk-forward testing**, translated into **portfolio-level outcomes**, and frozen with **audit-ready artifacts**.  
It is designed to meet **FinTech, institutional, and academic review standards**.

---

## 🧱 System Context & Boundaries

VinV operates within a deliberately modular research stack:

- **the_Spine** — canonical data fusion layer  
  *(SSOT, frequency normalization, availability flags)*

- **VinV** — machine-learning engine *(this module)*

- **QDT (Quantitative Debasement Theory)** — regime labeling only  
  *(contextual, non-blocking)*

- **OracleChambers** — interpretive layer only  
  *(no signal creation)*

**VinV is fully functional and ML-complete without QDT or OracleChambers.**  
Those layers add *context*, not *credibility*.

---

## 🧠 ML Operating Mantra (Non-Negotiable)

> **We establish lift with baselines, prove stability via walk-forward validation, translate probabilities into portfolio outcomes, and govern the entire pipeline with CPMAI controls and audit-ready artifacts.**

This principle governs all modeling decisions.

---

## ⚙️ Modeling Discipline & Controls

VinV follows an intentional, FinTech-grade model ladder:

- **Baselines first:** Dummy → Linear → Tree → Boosted  
- **Leakage control:** all preprocessing applied to **X-only**  
- **Macro stability:** rolling features, winsorization, noise reduction  
- **Validation:** time-respecting walk-forward validation (WFV)  
- **Selection:** empirical, deterministic, no manual overrides  
- **Translation:** evaluation at the **portfolio level**

No deep learning.  
No novelty chasing.  
**Stability and governance are prioritized over complexity.**

---

## 🗄️ Single Source of Truth (SSOT)

All VinV modeling derives from a **frozen, canonical SSOT** built from authoritative macro and market sources.

**Artifacts:**
```text
the_Spine/vinv/ssot/vinv_ml_ssot_vFinal.parquet
the_Spine/vinv/ssot/vinv_modeling_view_vFinal.parquet
```

```text
the_Spine/vinv/champion/vinv_champion_freeze_20251215T213325Z/

├─ champion_model.joblib
├─ champion_freeze_manifest.json
├─ freeze_hashes_sha256.json
```

**Metrics include:**
- AUC (classification quality)  
- Top-decile lift  
- Long/short portfolio Sharpe  
- Stability across folds  

These files constitute the **primary performance evidence** for VinV.

---

## 🏆 Champion Model (vFinal)

- **Champion Model:** `tier1_logistic_l2`  
- **Selection Basis:** highest walk-forward stability on the evaluated universe  
- **Final Refit Cutoff:** **2025-11-01**

The champion is selected **empirically**, not heuristically.  
Given the universe size, **stability and calibration dominated raw complexity**.

This reflects **maturity**, not underfitting.

---

## 🔒 Final Refit & Freeze

The champion model is refit on all data available **up to the final WFV cutoff**, then frozen.

**Freeze artifacts:**
the_Spine/vinv/champion/vinv_champion_freeze_20251215T213325Z/
├─ champion_model.joblib
├─ champion_freeze_manifest.json
├─ freeze_hashes_sha256.json

yaml
Copy code

**Controls enforced:**
- deterministic selection policy  
- timestamped freeze  
- SHA-256 hash locking  
- Git-tagged release  

These artifacts are **audit-ready**.

---

## 🛡️ CPMAI Governance Alignment

VinV explicitly aligns with **PMI-CPMAI** principles:

- simpler methods before complexity  
- separation of data, modeling, and interpretation  
- provenance and versioning  
- anti-leakage controls  
- reviewable, immutable evidence  

The repository intentionally contains:
- **code**
- **results evidence**
- **governance artifacts**

Raw data and heavy binaries are excluded by design.

---

## 🚀 What VinV Enables (Forward-Looking)

VinV provides a governed foundation for:

- regime-conditioned extensions (via QDT)  
- universe expansion (WRDS / broader equity coverage)  
- allocator-specific variants (e.g., long-only)  
- interpretive overlays (OracleChambers)  

All extensions preserve the same validation and governance posture.

---

## 🎯 Final Positioning

**VinV is a fully governed, macro-aware ML equity ranking engine built on authoritative data, validated through walk-forward testing, translated into portfolio outcomes, and frozen with audit-ready artifacts.**

It is ready for **institutional, sponsor, and faculty review**.

---

## ⚖️ Risk & Use Disclaimer
All content is for **research and educational purposes only**.  
This repository does not constitute investment advice or recommendations.  
Past performance does not guarantee future results.

---

## 📎 License
MIT License


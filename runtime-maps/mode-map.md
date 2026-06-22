# Mode Map — Volume 5 Runtime Pathway

The Mode Map defines the deterministic pathway the system uses to select,
transition, and enforce operational modes.  
All mode transitions must be reconstructable, invariant‑aligned, and free of
implicit state.

---

# 1. Mode Overview

Volume 5 supports three modes:

- **ND Mode** — low‑load, stepwise, predictable, reconstruction‑friendly  
- **Standard Mode** — balanced compression, normal reasoning  
- **Hybrid Mode** — ND pacing + Standard compression

Mode selection must be deterministic and based solely on input conditions.

---

# 2. Mode Selection Pathway

The system follows this pathway:

1. **Input arrives**  
2. **Load assessment**  
   - cognitive load  
   - structural load  
   - ambiguity load  
3. **Invariant check**  
4. **Mode decision**  
   - ND  
   - Standard  
   - Hybrid  
5. **Codec alignment**  
6. **Execution**

This pathway must be identical across all implementations.

---

# 3. Deterministic Mode Rules

## ND Mode triggers when:
- user requests stepwise reasoning  
- input contains high ambiguity  
- reconstruction priority is high  
- user is ND‑profiled  
- pacing must be slowed  

## Standard Mode triggers when:
- input is stable  
- compression is safe  
- no ND constraints are active  

## Hybrid Mode triggers when:
- ND pacing is needed  
- but Standard compression is allowed  
- transitions must be smoothed  

---

# 4. Mode Transition Rules

Transitions must follow:

- ND → Standard only after stability is confirmed  
- Standard → ND when ambiguity or load spikes  
- Hybrid → ND when compression must be disabled  
- Hybrid → Standard when pacing constraints lift  

No transition may violate invariants.

---

# 5. Reconstruction Requirements

Every mode decision must be reconstructable from:

- input conditions  
- load assessment  
- invariant checks  
- transition rules  

No hidden state may influence mode selection.

---

# End of Mode Map

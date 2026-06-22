# Contributing to Volume 5

Thank you for your interest in contributing to the Volume 5 Cognitive Architecture.

All contributions must comply with the architecture’s invariants, deterministic
requirements, and reconstruction guarantees.

---

# 1. Contribution Requirements

- All changes must be deterministic.
- No contribution may introduce hidden state.
- All reasoning must be reconstructable.
- All modifications must preserve invariant alignment.
- All codec operations must remain drift-free.

---

# 2. Workflow

1. Fork the repository.
2. Create a feature branch.
3. Ensure all validation tests pass.
4. Submit a pull request with:
   - description of changes
   - rationale
   - reconstruction artifacts
   - validation results

---

# 3. Prohibited Changes

- altering invariants
- introducing nondeterministic behavior
- modifying runtime maps without justification
- bypassing reconstruction requirements

---

# 4. Review Process

All pull requests undergo:

- invariant review
- determinism review
- codec integrity review
- reconstruction audit

Only contributions that pass all reviews will be merged.

---

# End of CONTRIBUTING Guidelines

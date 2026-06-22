# Volume 5 Release Manifest (v1.0)

This manifest defines the required artifacts for a valid Volume 5 release.
All items must be present, complete, and reconstructable.

---

# 1. Core Documents

- README.md
- specification/volume-5.md
- developer-kit/README.md

---

# 2. Runtime Maps

- runtime-maps/mode-map.md
- runtime-maps/codec-map.md
- runtime-maps/reconstruction-map.md

---

# 3. API Layer

- openapi.yaml

---

# 4. Validation Suite

- validation/validation-suite.md

---

# 5. Legal and Contribution Files

- LICENSE
- CONTRIBUTING.md

---

# 6. Release Requirements

A valid release must:

- pass all validation tests
- include all runtime maps
- include reconstruction artifacts
- be deterministic and drift-free
- be fully reconstructable from artifacts alone

---

# 7. Release Packaging

A complete release must include:

- all repository files
- a ZIP archive of the release
- a release tag (v1.0)
- a release description summarizing changes

---

# End of Release Manifest

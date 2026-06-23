[Home](index.md) • [Stability](V6_Stability_Spec.md) • [Governance](V7_Governance_Spec.md) • [Developer Kit](Atlas_Developer_Kit.md) • [Runtime Maps](Runtime_Maps.md) • [Integration Notes](Integration_Notes.md)
---
# Integration Notes


## Purpose
These notes guide external systems, tools, or services integrating with the architecture. They describe how to interact with V5 mechanics, V6 stability constraints, and V7 governance rules without violating boundaries.

## Integration Principles
- **Respect V7 Governance:** All actions must pass governance checks before execution.
- **Respect V6 Stability:** Inputs must be valid, unambiguous, and stable.
- **Use V5 Mechanics via Interfaces:** Do not bypass or embed architecture logic inside tools.

## Integration Steps
1. **Identify Required Operations**  
   Determine which V5 mechanics your system needs to call.

2. **Review Governance Rules (V7)**  
   Ensure the requested operation is permitted.

3. **Review Stability Constraints (V6)**  
   Validate that your inputs and state meet stability requirements.

4. **Implement Calls**  
   Use the documented interfaces or API endpoints.

5. **Add Logging**  
   Log governance decisions, stability outcomes, and execution results.

## Common Integration Patterns
- **Read-Only Clients**  
  Query data without modifying global state.

- **Controlled Mutations**  
  Changes that pass governance and stability checks.

- **Sandboxed Experiments**  
  Isolated environments that cannot affect core governance.

## Anti-Patterns
- Bypassing governance checks.
- Embedding governance logic inside tools.
- Allowing tools to modify stability or governance rules.
- Creating hidden side effects.

## Version Compatibility
- Check V5–V7 versions before integrating.
- Breaking changes will be documented in `CHANGELOG.md`.

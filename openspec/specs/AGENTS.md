<!-- Parent: ../../AGENTS.md -->
<!-- Generated: 2026-03-01 | Updated: 2026-03-07 -->

# OPENSPEC: LIVING SPECS

Inherits root `AGENTS.md`. Covers authoring and maintenance of living subsystem specs under `openspec/specs/`.

## OVERVIEW
Each `specs/<domain>/spec.md` file is the active behavioral contract for that subsystem; requirements must stay normative, observable, and testable.

## WHERE TO LOOK
| Task | Location | Notes |
|------|----------|-------|
| Authoring rules | `../config.yaml` | proposal/task/spec rule set and normative wording |
| Domain contracts | `*/spec.md` | one living spec per subsystem |
| High-churn specs | `render-pipeline/spec.md`, `compositor-capture/spec.md`, `input-forwarding/spec.md` | broad runtime impact areas |
| Change deltas | `../changes/<change-id>/specs/` | staged spec updates before sync |
| Archive boundary | `../changes/archive/` | reference-only, no direct edits |

## CONVENTIONS
- Use RFC-style normative language (`MUST`, `SHOULD`, `MAY`) in requirement blocks.
- Pair each requirement with at least one GIVEN/WHEN/THEN scenario.
- Keep requirements behavior-focused and implementation-agnostic.
- Update `## Purpose` when touching specs that still contain placeholder/TBD text.
- Apply substantial behavior changes through change deltas first, then sync to living specs.

## ANTI-PATTERNS
- Writing implementation steps as requirements without observable outcomes.
- Editing archived change specs instead of current living specs or active deltas.
- Shipping requirement edits without matching scenario updates.
- Bundling unrelated behavior changes into one domain spec edit.

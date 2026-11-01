# Ticket 001: Adopt immutable native governance for campaign admission

- **ID**: ticket-001
- **Owner**: agent:codex
- **Status**: IN_PROGRESS
- **Workflow state**: PUBLICATION
- **Created**: 2026-10-31

## Goal and scope

SESSION_EXECUTION_AUTHORIZATION: user requested executing, merging, testing and repairing the fleet recovery decisions on 2026-10-31. Install the published native governance 0.20.129 at 82fd58dbe175f90146ed49c07fa86fac91de00d5 to replace the incomplete registration scaffold. Preserve original local files in an external digest-bound secret-scanned snapshot. The allocator owns this canonical checkout and ticket identity; only the actual controller lease authorizes implementation.

The wheel must include the governance pytest bridge so the installed pytest
console entry point can import it independently of the working directory.

## Acceptance criteria

- [x] AC-01: Complete pinned governance package and prerequisite files are present.
- [x] AC-02: Product tests and governance checks pass.
- [ ] AC-03: Independent exact-head approval and protected merge are observed.

## Published129 continuation

SESSION_EXECUTION_AUTHORIZATION persists from the user request to execute, test,
repair and merge. Refresh the existing119 adoption candidate to independently
published129. Preserve the old signed review and all its29 unresolved findings;
new source, tests and runtime qualification require fresh independent review.
Use the approved fullWellman d8c7a0a runtime, checkout-local .venv and private
execution scratch. Product code, dependencies and unknown primary scaffolding
remain outside this continuation. The three new managed paths are taken only
from the pinned Goal preview.

## Validation of published 0.20.129

Native Goal reports the package up to date at the exact published revision.
The managed governance gate passes with zero errors and warnings; all two
existing product tests pass. Both Python executions have canonical full Wellman
receipts bound to this checkout and its local environment. The pyproject change
is limited to the standard version and source revision; dependency declarations
and product source are unchanged. OneDev runtime qualification and independent
current-head review remain pending.

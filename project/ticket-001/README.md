# Ticket 001: Adopt immutable native governance for campaign admission

- **ID**: ticket-001
- **Owner**: agent:codex
- **Status**: IN_PROGRESS
- **Workflow state**: PUBLICATION
- **Created**: 2026-10-31

## Goal and scope

SESSION_EXECUTION_AUTHORIZATION: user requested executing, merging, testing and repairing the fleet recovery decisions on 2026-10-31. Install the published native governance 0.20.119 at 07d2cf4c34ea308929a6a2c78497f20901a58b3e to replace the incomplete registration scaffold. Preserve original local files in an external digest-bound secret-scanned snapshot. The allocator owns this canonical checkout and ticket identity; only the actual controller lease authorizes implementation.

## Acceptance criteria

- [x] AC-01: Complete pinned governance package and prerequisite files are present.
- [x] AC-02: Product tests and governance checks pass.
- [ ] AC-03: Independent exact-head approval and protected merge are observed.

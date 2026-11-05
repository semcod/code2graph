# Ticket 002: Adopt git-ancestry ticket activity resolution for scheduled governance

- **ID**: ticket-002
- **Owner**: agent:opencode-deepseek
- **Status**: IN_PROGRESS
- **Workflow state**: EDIT
- **Created**: 2026-11-05

## Goal and scope

SESSION_EXECUTION_AUTHORIZATION: portfolio PLF-19969 / parent PLF-19971 authorizes
bounded adoption of the reviewed governance correction in affected repositories.
This ticket is the native admission for one adopter-local policy choice in
`semcod/code2graph`.

The scheduled `new-project-governance` run fails `GOV-SYNC-001` because a fresh
Git checkout has no clone-external terminal receipt registry. With the managed
default `registry.missingPolicy: status-projection`, `project/ticket-001`
(`IN_PROGRESS`) is projected active even though its delivery is already on
`main`; the no-argument scheduled gate then cannot resolve an adoption base.

The supported, schema-declared remedy for an adopter whose hand-edited statuses
no longer track Git reality is the target-owned
`.governance/ticket-activity.override.json` with `missingPolicy: git-ancestry`.
The managed policy file and generated workflow stay untouched.

## Acceptance criteria

- [x] AC-01: Add only `.governance/ticket-activity.override.json` with the
      documented schema and `missingPolicy: git-ancestry`.
- [x] AC-02: Do not edit `.governance/ticket-activity.json`, the governance
      workflow, pins, credentials or protected checks.
- [x] AC-03: The exact published runtime 0.20.131 (`3926cecf`) evaluates a clean
      checkout with no `--base/--head` as `passed` and no `GOV-SYNC-001`.
- [x] AC-04: The repository governance check and focused tests pass on the
      ticket head; any failure is reported, not waived.
- [x] AC-05: Publish through the declared protected route with exact-head
      independent review; no direct merge.

## Evidence

- Portfolio checkpoint:
  `.planfile/evidence/daily-delivery-plf19969-20261103/resume-20261104T2342Z/`
- Upstream owner findings: wellmanifest/new-project GITHUB-532, GITHUB-537.
- Local runtime reproduction: fresh clone fails with `GOV-SYNC-001`; the same
  tree with the override resolves `ticket-001` via `git-ancestry`.

## Tracking boundary

This directory contains the minimal reviewed intent. Optional participant prose
and raw command logs are not required delivery output.

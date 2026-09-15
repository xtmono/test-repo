---
plan: hold-record-appears
index_family: arabic
pr_units:
  - index: 1
    title: "Record the hold observation"
    type: docs
    depends_on: []
    files:
      - docs/notes.md
    acceptance:
      - id: AC-1-1
        cmd: "test -f docs/notes.md"
        expect: exit0
---

# Observe the required-check hold on a late record

A scratch plan. Shipping it opens a PR on a branch whose ruleset requires
the `changes` status, which nothing posts until the operator does.

## PR 1: Record the hold observation

**Items**:

- [ ] Add `docs/notes.md`

**Design**: One file, no code.

**Tests**: None; the PR exists to be watched.

**Rollback**: Revert the commit.

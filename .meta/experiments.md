---
type: Reference
title: Experiments
description: Experiments being run or considered.
---

## 001 - Sudoku vertical slice

**Question:** Can a small OKF v0.2 knowledge bundle describe enough Sudoku context for a person and an agent to independently derive and test the same behaviour, without first defining a general domain schema?

**Smallest useful slice:** Describe only enough Sudoku knowledge to support one concrete behaviour: when a symbol is assigned to a cell, that symbol is no longer a valid candidate in cells that share a relevant cell-set with it.

The experiment should add only the domain knowledge needed to express and exercise that behaviour. Its structure is part of what the experiment is intended to discover.

**Evidence:**

* The knowledge files required for the slice and the changes made to them while learning.
* Human and agent interpretations of the knowledge, including ambiguities or missing context they encounter.
* At least one independently derived, testable example of the behaviour.
* Any structure that proves necessary to make the knowledge usable.

**Success:** The repository alone provides enough context for both a person and an agent to reach a materially consistent, testable interpretation of the selected behaviour, with no domain-specific schema assumed outside the bundle.

**Failure:** Important interpretation depends on unstated knowledge, human and agent interpretations materially diverge, or the slice requires substantial structure that has not been justified by the experiment.

**Out of scope:**

* A complete Sudoku model or solver.
* A general schema for dimensions, rules, flows, personas, or tests.
* Frontmatter extensions beyond OKF v0.2 requirements.
* Choosing a long-term directory structure for Sudoku knowledge.
* Comparing multiple specification-driven development tools or frameworks.
* Optimising for every possible consumer of the knowledge.

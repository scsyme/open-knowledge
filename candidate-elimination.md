---
type: Reference
title: Sudoku candidate elimination
description: Minimal context for eliminating a candidate after assigning a symbol.
---

# Context

A cell may be assigned a symbol.

An unassigned cell may have candidate symbols: symbols that could still validly be assigned to it.

Cells may share a cell-set. Within a cell-set, the same symbol cannot be assigned to more than one cell.

# Behaviour

When a symbol is assigned to a cell, that symbol is no longer a valid candidate for any other cell sharing a cell-set with it.

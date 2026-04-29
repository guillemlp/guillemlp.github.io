---
title: "gem5 + RTL"
permalink: /research/gem5-rtl/
order: 3
tag: "ICPP '21"
tagline: "A framework that drops Verilog/SystemVerilog RTL models into the gem5 full-system simulator — hardware–software co-simulation across the whole stack."
role: "First author"
venue: "ICPP 2021"
year: 2021
status: "Published · Open source"
collaborators: "BSC"
collaborators_short: "BSC"
paperurl: "https://doi.org/10.1145/3472456.3472461"
bibtex: |
  @inproceedings{lopezparadis2021gem5rtl,
    title     = {gem5+rtl: A Framework to Enable {RTL} Models Inside a Full-System Simulator},
    author    = {L{\'o}pez-Parad{\'\i}s, Guillem and Armejach, Adri{\`a} and Moret{\'o}, Miquel},
    booktitle = {Proceedings of the 50th International Conference on Parallel Processing (ICPP)},
    year      = {2021},
    pages     = {1--11},
    doi       = {10.1145/3472456.3472461}
  }
---

## TL;DR

Architects rely on **gem5** for full-system experimentation — boot a real OS,
run real workloads, study new memory hierarchies and ISAs. But gem5 components
are written in C++, while accelerators and IP blocks are written in
**Verilog/SystemVerilog**. The gap means accelerator research either uses a
hand-coded gem5 model (low fidelity) or a standalone RTL bench (no software
stack).

**gem5+RTL** closes that gap: a generic interface that lets a Verilator-built
RTL block participate in a gem5 full-system simulation as a first-class
component. Boot Linux, run a binary, and have it offload to your real RTL
accelerator — all inside one simulator.

## The problem

Two long-standing pain points in accelerator research:

1. **Fidelity vs. integration.** A C++ behavioural model in gem5 is fast but
   loses the implementation detail (timing, micro-architecture, control
   logic). RTL captures everything but lives outside the OS-aware loop.
2. **Engineering cost.** Every group reinvents its own ad-hoc bridge between
   gem5 and Verilator (sockets, shared memory, custom protocols), often tied
   to a single accelerator and unmaintained.

## Approach

gem5+RTL provides a generic, reusable wrapper:

- **gem5 sees the RTL block as a SimObject** with the standard memory and
  interrupt interfaces.
- **The RTL block runs under Verilator** in lock-step with gem5's clocked
  domain.
- **Memory accesses and control signals** cross the boundary through a thin,
  typed channel — no per-accelerator glue.

This made it possible to evaluate real accelerator designs (HWPF, NMC, custom
RISC-V coprocessors) inside Linux, on real binaries, with gem5's existing
profiling and visualisation.


---
title: "Metro-MPI"
permalink: /research/metro-mpi/
order: 2
tag: "DATE '23"
tagline: "Distributed RTL simulation that parallelises behavioural Verilator with MPI — 1,024 cores, 134× speedup, billion-transistor SoCs become tractable."
role: "First author"
venue: "DATE 2023"
year: 2023
status: "Published · Open source"
collaborators: "BSC, UCSB, TUM"
collaborators_short: "BSC · UCSB · TUM"
paperurl: "https://doi.org/10.23919/DATE56975.2023.10137080"
bibtex: |
  @inproceedings{lopezparadis2023metrompi,
    title     = {Fast Behavioural {RTL} Simulation of {10B} Transistor {SoC} Designs with {Metro-MPI}},
    author    = {L{\'o}pez-Parad{\'\i}s, Guillem and Li, Brian and Armejach, Adri{\`a} and
                 Wallentowitz, Stefan and Moret{\'o}, Miquel and Balkind, Jonathan},
    booktitle = {2023 Design, Automation \& Test in Europe Conference \& Exhibition (DATE)},
    year      = {2023},
    pages     = {1--6},
    doi       = {10.23919/DATE56975.2023.10137080}
  }
---

## TL;DR

RTL simulation of post-tape-out-scale SoCs is one of the longest-standing
bottlenecks in computer architecture research. Behavioural simulators like
**Verilator** are fast per-thread but single-process — and once a design
crosses ~1B transistors, simulation throughput collapses.

**Metro-MPI** restructures the design under simulation as a network of
communicating MPI processes, one per simulator instance, with explicit message
passing on the boundaries between hierarchical blocks. The result: distributed
behavioural RTL simulation that scales to **1,024 cores** with a **134×
speedup**, making **10-billion-transistor SoCs** tractable.

## The problem

Behavioural RTL simulation is sequential by construction. Each simulator
process advances one cycle at a time across the entire design. As designs
grow:

- **Memory footprint** grows linearly with state.
- **Simulator throughput** drops because cache locality is lost.
- **Multi-threading inside one simulator** has poor scaling because of the
  fine-grained synchronisation cost.

The community has tried FPGA emulation, hybrid simulators, and parallel
discrete-event approaches — each with severe usability or fidelity trade-offs.

<figure>
  <svg class="diagram" viewBox="0 0 720 280" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Metro-MPI process partitioning">
    <defs>
      <marker id="arr2" viewBox="0 0 10 10" refX="9" refY="5" markerWidth="6" markerHeight="6" orient="auto">
        <path d="M0,0 L10,5 L0,10 z" class="d-primary-fill"/>
      </marker>
    </defs>
    <text x="20" y="25" class="d-text" font-size="14" font-weight="600">Monolithic Verilator (single process)</text>
    <rect x="20" y="40" width="320" height="90" rx="8" class="d-stroke" stroke-width="1.5"/>
    <text x="180" y="80" text-anchor="middle" font-size="13">10B-transistor SoC</text>
    <text x="180" y="100" text-anchor="middle" font-size="11" class="d-muted">one simulator process · sequential</text>

    <text x="380" y="25" class="d-text" font-size="14" font-weight="600">Metro-MPI (process per tile)</text>
    <g class="d-primary" stroke-width="1.5">
      <rect x="380" y="40" width="60" height="40" rx="4"/>
      <rect x="450" y="40" width="60" height="40" rx="4"/>
      <rect x="520" y="40" width="60" height="40" rx="4"/>
      <rect x="590" y="40" width="60" height="40" rx="4"/>
      <rect x="380" y="90" width="60" height="40" rx="4"/>
      <rect x="450" y="90" width="60" height="40" rx="4"/>
      <rect x="520" y="90" width="60" height="40" rx="4"/>
      <rect x="590" y="90" width="60" height="40" rx="4"/>
    </g>
    <text x="515" y="155" text-anchor="middle" font-size="11" class="d-muted">N processes · MPI on tile boundaries</text>

    <text x="20" y="200" class="d-text" font-size="14" font-weight="600">Scaling</text>
    <line x1="20" y1="240" x2="700" y2="240" class="d-stroke" stroke-width="1"/>
    <line x1="20" y1="220" x2="20" y2="260" class="d-stroke" stroke-width="1"/>
    <text x="20" y="275" font-size="11" class="d-muted">1</text>
    <text x="350" y="275" font-size="11" class="d-muted">256 cores</text>
    <text x="690" y="275" font-size="11" class="d-muted">1024 cores</text>
    <circle cx="20" cy="240" r="3" class="d-primary-fill"/>
    <circle cx="180" cy="232" r="3" class="d-primary-fill"/>
    <circle cx="350" cy="222" r="3" class="d-primary-fill"/>
    <circle cx="520" cy="218" r="3" class="d-primary-fill"/>
    <circle cx="690" cy="216" r="3" class="d-primary-fill"/>
    <path d="M20 240 Q350 220 690 216" class="d-stroke" stroke-width="1.5" fill="none" stroke="var(--c-primary)"/>
    <text x="690" y="208" text-anchor="end" font-size="11" class="d-text">134× at 1024 cores</text>
  </svg>
  <figcaption>Schematic: Metro-MPI partitions a monolithic SoC RTL into per-tile simulator processes that communicate over MPI. Shown right: simulator throughput vs. process count.</figcaption>
</figure>

## Approach

Three architectural decisions made Metro-MPI work where prior parallel-RTL
attempts stalled:

1. **Hierarchical partitioning at natural cut points.** RTL designs already
   have well-defined boundaries (tiles, NoC routers, memory controllers). We
   partition at those interfaces, not at a flat-net level.
2. **Explicit message-passing semantics, not shared state.** Simulator
   processes communicate through MPI calls placed exactly at the interface
   wires — no global locking, no shared memory, no implicit ordering.
3. **Per-process Verilator unchanged.** Each MPI rank still runs vanilla
   Verilator on its piece, so the behavioural fidelity, debug flow, and tool
   support are preserved.

The framework is open source and has been reused for the
[OpenPiton4HPC](/publication/2024-07-01-openpiton4hpc) work and the
[HyperLoops](/research/hyperloops/) modelling effort.

## What's next

The current postdoc track integrates Metro-MPI into mainline
**Verilator** and connects it to **multi-FPGA** environments — letting
researchers mix software simulation and hardware emulation on the same design
without rewriting the testbench. Mentored under GSoC 2025 (FOSSi).

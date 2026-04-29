---
title: "Coherent accelerator framework (ACAI)"
permalink: /research/acai/
order: 4
tag: "SAMOS '23"
tagline: "First public characterisation of Arm's coherent accelerator framework on real SoCs — design trade-offs of putting accelerators inside the cache-coherence domain."
role: "First author"
venue: "SAMOS 2023"
year: 2023
status: "Published"
collaborators: "Arm Research, BSC"
collaborators_short: "Arm Research · BSC"
paperurl: "https://doi.org/10.1007/978-3-031-46077-7_7"
bibtex: |
  @inproceedings{lopezparadis2023acai,
    title     = {Characterization of a Coherent Hardware Accelerator Framework for {SoCs}},
    author    = {L{\'o}pez-Parad{\'\i}s, Guillem and Venu, Balaji and Armejach, Adri{\`a} and Moret{\'o}, Miquel},
    booktitle = {Embedded Computer Systems: Architectures, Modeling, and Simulation (SAMOS)},
    year      = {2023},
    pages     = {91--106},
    publisher = {Springer},
    doi       = {10.1007/978-3-031-46077-7_7}
  }
---

## TL;DR

Coherent accelerator integration — putting an accelerator's caches *inside*
the CPU's cache-coherence domain — is the trend in modern SoCs (CXL, AMBA
CHI, Compute Express Link, Arm's ACAI). It promises a uniform programming
model and zero-copy software, but the architectural cost was poorly
documented in the open literature.

This paper provides the **first public characterisation of Arm's coherent
accelerator framework (ACAI)** on real SoC configurations — what coherence
buys you, what it costs, and where it's worth deploying.

## The problem

Coherence at the accelerator side has the wrong reputation. Designers either
overestimate the cost ("we'll DMA-copy everything to be safe") or
underestimate the impact on the snoop network and directory state. Without a
public characterisation, every team is rediscovering the same trade-off
curves on their own.

## Approach

The work was done during a research collaboration with **Arm Research**
(Cambridge / Austin) and characterises ACAI across:

- **Workload mix** — streaming vs. fine-grained accelerator interactions
- **Coherence granularity** — cache-line vs. region-level coherence
- **Snoop fan-out** — single-tile vs. multi-tile accelerator clusters
- **Directory pressure** — accelerator-driven invalidations and their cost on
  CPU-side miss latency

The paper publishes the trade-off curves the community needed: when the
performance and energy of cache-coherent integration beat the
DMA-and-copy pattern, when they don't, and which architectural knobs matter
most. It became part of my PhD thesis chapter on **coherent accelerator
memory subsystems** and motivated the MPMC queue-based interfaces that I
now use across multiple RISC-V SoC designs at BSC.

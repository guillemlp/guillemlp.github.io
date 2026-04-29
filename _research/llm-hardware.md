---
title: "LLM-driven hardware design"
permalink: /research/llm-hardware/
order: 5
tag: "Ongoing — 2025+"
tagline: "Agent-driven workflows for automated RTL generation, architectural exploration, and hardware–software co-design."
role: "Lead"
venue: "BSC Postdoc research direction"
year: 2025
status: "Ongoing"
collaborators: "BSC, UCSB, Politecnico di Milano"
collaborators_short: "BSC · UCSB · PoliMilano"
---

## TL;DR

The last two years made it obvious that LLM-based agents can write
non-trivial code. Hardware design is *also* code — RTL, testbenches,
configuration scripts, scaling sweeps — but the loop is far slower and the
cost of a bad iteration is far higher than in software.

My new research direction at BSC is to build the **agent infrastructure that
makes hardware design tractable for LLMs**: tools that constrain RTL
generation to synthesisable, verifiable subsets, simulators that close the
feedback loop in seconds rather than hours, and exploration agents that
search architectural design spaces with budgeted experiments.

## The problem

Agentic LLM workflows in software engineering work because the inner loop is
fast and reversible: the model proposes a change, runs the tests, iterates.
Hardware design is none of that:

- A typical full-system RTL simulation can take **hours**.
- A typical synthesis + place-and-route loop can take **days**.
- Bad RTL doesn't just fail tests — it can produce silicon that's
  unmanufacturable or insecure.

Existing LLM-for-RTL work shows the *capability* is real (the models can
write Verilog) but the *infrastructure* — the harness, the tooling, the
verification loop — is still missing.

## Approach

The plan is built on the simulation infrastructure I've spent five years
on:

1. **[Metro-MPI](/research/metro-mpi/)** brings RTL simulation down from days
   to minutes. That changes what an agent can iterate on.
2. **[gem5+RTL](/research/gem5-rtl/)** lets the agent observe its design
   running real software, not just synthetic testbenches.
3. **Coherence and accelerator interface patterns** ([ACAI](/research/acai/),
   MPMC queues) give the agent a constrained, well-understood vocabulary to
   propose new accelerators within.

The agents we're prototyping target three concrete loops:

- **Constrained RTL generation** for accelerator skeletons that compile,
  simulate, and pass an interface conformance suite on first iteration.
- **Architectural exploration** of micro-architecture parameters under a
  fixed simulation budget.
- **Hardware–software co-design** where the agent owns both the accelerator
  RTL and the driver/runtime patches that exercise it.

## Status

Active research direction at BSC, with a team of four (BSc, MSc, PhD, RE)
and ongoing collaborations with **UCSB** and **Politecnico di Milano**.
First-author paper on advanced communication patterns for hardware
accelerators is **under review**.

If you work on agent infrastructure, hardware verification automation, or
LLM-for-EDA — I'd love to talk.
[Get in touch](mailto:guillem.lopez.paradis@gmail.com).

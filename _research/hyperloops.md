---
title: "Data Centre HyperLoops"
permalink: /research/hyperloops/
order: 1
tag: "ISCA '24"
tagline: "Embodied data movement at hyperscale: maglev carts shuttle SSDs at hundreds of m/s along a data-centre track. 114×–646× faster transfers and 1.6×–376× lower energy than 400 Gbps optical networks for PB-scale workloads."
role: "Co-first author"
venue: "ISCA 2024"
year: 2024
status: "Published"
collaborators: "UCSB (Balkind lab)"
collaborators_short: "UCSB · Balkind lab"
paperurl: "https://jbalkind.github.io/docs/dhl_camera_ready.pdf"
bibtex: |
  @inproceedings{lopezparadis2024hyperloops,
    title     = {The Case For Data Centre HyperLoops},
    author    = {L{\'o}pez-Parad{\'\i}s, Guillem and Hair, Isaac M. and Kannan, Sid and
                 Rabbat, Roman and Murray, Parker and Lopes, Alex and Zahedi, Rory and
                 Zuo, Winston and Balkind, Jonathan},
    booktitle = {2024 ACM/IEEE 51st Annual International Symposium on Computer Architecture (ISCA)},
    year      = {2024},
    pages     = {274--289},
    doi       = {10.1109/ISCA59077.2024.00026},
    note      = {Co-first author with Isaac M. Hair}
  }
---

## TL;DR

Modern data centres are kilometres long, and ML training and analytics
workloads now need to move **petabyte-scale** datasets between
nodes. Doing that over a 400 Gbps optical network can take **a week** and
cost **megajoules** of energy.

We re-examine the assumption that data must be *copied* over the network
at all. **Data Centre HyperLoops (DHLs)** are a transport mechanism that
physically moves the storage media: a magnetically levitated cart full of
high-density SSDs travels along a low-friction rail at hundreds of metres
per second between docking stations, using cheap and well-understood maglev
technology.

For PB-scale bulk transfers, DHLs deliver **114×–646× faster transfers**
and **1.6×–376× less energy** than the equivalent 400 Gbps optical path,
and reach **73.3 GB/J** end-to-end transmission efficiency.

<figure>
  <svg class="diagram" viewBox="0 0 720 260" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Data centre with a HyperLoop track running below the false floor between two docking stations, after Fig. 1 of the ISCA'24 paper">
    <!-- Server racks above the false floor -->
    <g class="d-stroke" stroke-width="1.2" fill="none">
      <rect x="80"  y="40" width="46" height="100" rx="3"/>
      <rect x="135" y="40" width="46" height="100" rx="3"/>
      <rect x="190" y="40" width="46" height="100" rx="3"/>
      <rect x="245" y="40" width="46" height="100" rx="3"/>
      <rect x="300" y="40" width="46" height="100" rx="3"/>
      <rect x="375" y="40" width="46" height="100" rx="3"/>
      <rect x="430" y="40" width="46" height="100" rx="3"/>
      <rect x="485" y="40" width="46" height="100" rx="3"/>
      <rect x="540" y="40" width="46" height="100" rx="3"/>
      <rect x="595" y="40" width="46" height="100" rx="3"/>
    </g>
    <g class="d-stroke" stroke-width="0.6" fill="none" opacity="0.6">
      <line x1="80"  y1="55" x2="126" y2="55"/><line x1="80"  y1="70" x2="126" y2="70"/>
      <line x1="80"  y1="85" x2="126" y2="85"/><line x1="80"  y1="100" x2="126" y2="100"/>
      <line x1="80"  y1="115" x2="126" y2="115"/><line x1="80"  y1="130" x2="126" y2="130"/>
    </g>
    <text x="103" y="32" text-anchor="middle" font-size="11" font-weight="700" class="d-text">A</text>
    <text x="618" y="32" text-anchor="middle" font-size="11" font-weight="700" class="d-text">B</text>

    <!-- False floor line -->
    <line x1="40" y1="160" x2="680" y2="160" class="d-stroke" stroke-width="1.5"/>
    <text x="55" y="155" font-size="10" class="d-muted">FALSE FLOOR</text>

    <!-- Docking stations -->
    <rect x="40"  y="172" width="60" height="36" rx="3" class="d-primary" stroke-width="1.5"/>
    <text x="70" y="190" text-anchor="middle" font-size="9" font-weight="600" class="d-text">DOCKING</text>
    <text x="70" y="200" text-anchor="middle" font-size="9" font-weight="600" class="d-text">STATION</text>

    <rect x="620" y="172" width="60" height="36" rx="3" class="d-primary" stroke-width="1.5"/>
    <text x="650" y="190" text-anchor="middle" font-size="9" font-weight="600" class="d-text">DOCKING</text>
    <text x="650" y="200" text-anchor="middle" font-size="9" font-weight="600" class="d-text">STATION</text>

    <!-- DHL rail between the docking stations -->
    <rect x="100" y="184" width="520" height="12" rx="2" fill="none" stroke="var(--c-primary)" stroke-width="1.2"/>
    <g stroke="var(--c-primary)" stroke-width="0.6" opacity="0.7">
      <line x1="115" y1="184" x2="115" y2="196"/>
      <line x1="135" y1="184" x2="135" y2="196"/>
      <line x1="155" y1="184" x2="155" y2="196"/>
      <line x1="175" y1="184" x2="175" y2="196"/>
      <line x1="195" y1="184" x2="195" y2="196"/>
      <line x1="215" y1="184" x2="215" y2="196"/>
      <line x1="235" y1="184" x2="235" y2="196"/>
      <line x1="255" y1="184" x2="255" y2="196"/>
      <line x1="275" y1="184" x2="275" y2="196"/>
      <line x1="295" y1="184" x2="295" y2="196"/>
      <line x1="315" y1="184" x2="315" y2="196"/>
      <line x1="335" y1="184" x2="335" y2="196"/>
      <line x1="395" y1="184" x2="395" y2="196"/>
      <line x1="415" y1="184" x2="415" y2="196"/>
      <line x1="435" y1="184" x2="435" y2="196"/>
      <line x1="455" y1="184" x2="455" y2="196"/>
      <line x1="475" y1="184" x2="475" y2="196"/>
      <line x1="495" y1="184" x2="495" y2="196"/>
      <line x1="515" y1="184" x2="515" y2="196"/>
      <line x1="535" y1="184" x2="535" y2="196"/>
      <line x1="555" y1="184" x2="555" y2="196"/>
      <line x1="575" y1="184" x2="575" y2="196"/>
      <line x1="595" y1="184" x2="595" y2="196"/>
    </g>

    <!-- Cart traveling on the rail -->
    <rect x="345" y="178" width="40" height="22" rx="2" class="d-primary-fill"/>
    <text x="365" y="193" text-anchor="middle" font-size="9" font-weight="700" fill="#fff">CART</text>

    <!-- Ground line -->
    <line x1="40" y1="220" x2="680" y2="220" class="d-stroke" stroke-width="1"/>

    <text x="360" y="245" text-anchor="middle" font-size="11" class="d-muted">A maglev cart of SSDs shuttles between docking stations under the false floor</text>
  </svg>
  <figcaption>After Fig. 1 of <em>The Case For Data Centre HyperLoops</em> (ISCA '24): a maglev cart full of SSDs shuttles bulk datasets along a track under the data-centre false floor, between two docking stations.</figcaption>
</figure>

## The problem

Three trends made bulk data movement a first-class architectural problem:

1. **Datasets exploded.** Modern ML training corpora, scientific data
   acquisition (LHC at 150 TB/s), and routine cloud backups now reach the
   petabyte scale per day.
2. **Data centres got physically bigger.** Hyperscale facilities span
   kilometres, and most of the dataset traffic is between nodes that are
   physically far apart but logically near.
3. **Optical networks scale poorly for bulk.** A 400 Gbps optical link
   moving Meta's 29 PB ML dataset takes ~6 days and burns megajoules of
   transceiver and switching energy. Throwing more parallel optical links
   at the problem doesn't help energy efficiency, and PB-scale transfers
   block the network for everyone else.

The paper argues that for these PB-scale, infrequent, large-block transfers
the right answer isn't a faster network — it's not a network at all.

## Approach

DHL is **embodied data movement**: instead of copying bytes over a wire,
move the disks. The architecture has six components:

1. **Cart** — a magnetically levitated vehicle whose payload is a tightly
   packed grid of high-density M.2 SSDs (hundreds of TB per cart).
2. **Rail** — modular PVC track segments containing the conductive coils
   that levitate the cart and the linear induction motors that drive it.
3. **Accelerator and brake** — linear induction motors at the cart endpoints
   to bring it up to speed and decelerate it for docking.
4. **Docking stations** — server-rack-side endpoints where carts park and
   their SSDs are read or written, with a thin software layer that
   abstracts the DHL away from existing data-centre tooling.
5. **Library** — a centralised parking and maintenance facility for carts
   not currently in transit.
6. **Low-friction enclosure** — vacuum-sealed maglev rails reuse decades
   of work on commercial maglev transport, so the engineering risk is in
   the integration, not the physics.

We modelled DHL end-to-end (energy, time, data-centre footprint) and
benchmarked it on a representative ML training workload — one DLRM
training iteration in the **ASTRA-sim** ML simulator — against parallel
optical links under both **iso-power** and **iso-time** budgets.

## What's next

DHLs open a design space — bulk dataset transport that lives outside the
data-centre network entirely — that I'm continuing to explore as part of my
postdoc research at BSC, with extensions for non-uniform scale-out
collectives and integration with [Metro-MPI](/research/metro-mpi/) for
full-system simulation of HyperLoop-enabled data centres.

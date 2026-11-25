---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<section class="hero" markdown="0">
  <p class="hero__eyebrow">Computer Architecture Researcher · BSC</p>
  <h1 class="hero__name">Guillem López Paradís</h1>
  <p class="hero__tagline">RISC-V CPU and SoC microarchitecture, memory systems, and accelerator integration.</p>
  <p class="hero__lede">Postdoctoral researcher and research lead at the Barcelona Supercomputing Center (BSC). I design RTL microarchitecture for RISC-V cores and accelerator-rich SoCs, take it to silicon and FPGA, analyse performance with TopDown and memory-bandwidth studies, and build the simulation tooling that makes billion-transistor designs tractable.</p>
  <p class="hero__cta">
    <a class="btn btn--primary" href="/files/Guillem_Lopez_Paradis_CV.pdf"><i class="fas fa-file-pdf"></i> Download CV</a>
    <a class="btn btn--ghost" href="/publications/"><i class="fas fa-book"></i> Publications</a>
    <a class="btn btn--ghost" href="https://scholar.google.com/citations?user=ookFZsQAAAAJ&hl=en"><i class="ai ai-google-scholar"></i> Google Scholar</a>
    <a class="btn btn--ghost" href="https://github.com/guillemlp"><i class="fab fa-github"></i> GitHub</a>
  </p>
</section>

<ul class="stats" markdown="0">
  <li class="stat">
    <span class="stat__num">136×</span>
    <span class="stat__label">faster RTL simulation of a 1,024-core SoC with Metro-MPI (DATE ’23)</span>
  </li>
  <li class="stat">
    <span class="stat__num">5.9×</span>
    <span class="stat__label">speedup over software with MPMC hardware queues on coherent memory</span>
  </li>
  <li class="stat">
    <span class="stat__num">7&nbsp;nm</span>
    <span class="stat__label">RISC-V tapeouts I contributed to, from Sargantana-based designs</span>
  </li>
  <li class="stat">
    <span class="stat__num">10×</span>
    <span class="stat__label">measured memory bandwidth after fixing NoC, cache and MC bottlenecks</span>
  </li>
</ul>

About me
======

I am a computer architecture researcher at the Barcelona Supercomputing Center (BSC), working on **RISC-V CPU and SoC microarchitecture**, **memory systems** and **performance analysis**. I received my PhD in Computer Architecture (**Cum Laude**) from BSC–UPC in July 2025, with a thesis on *Efficient Data Movement in Large-Scale Heterogeneous Systems*, advised by Adrià Armejach and Miquel Moretó.

I design RTL microarchitecture (the Sargantana core's FPU and its **512-bit vector unit**, MPMC hardware queue endpoints, hardware scheduler queues), have contributed to **RISC-V tapeouts down to 7 nm**, and evaluate designs with TopDown, gem5, FPGA prototypes and large-scale RTL simulation with [Metro-MPI](/publication/2023-04-01-date23). I spent two research stays at **UC Santa Barbara**, where I co-developed [Data Centre HyperLoops](/publication/2024-06-01-hyperloops) (ISCA ’24).

Today I lead a team of four at BSC. I am BSC's **technical lead for WP6 of the EU project ODE4EC** on open-source EDA tools, lead a student team building the **TMU sparse accelerator** with the **Arm CoE**, and coordinate collaborations with **UCSB** and **Politecnico di Milano**.

What I work on
======

<ul class="cards" markdown="0">
  <li class="card">
    <span class="card__icon"><i class="fas fa-project-diagram"></i></span>
    <h3 class="card__title">Coherent accelerator integration</h3>
    <p class="card__desc">MPMC hardware queues on coherent memory for RISC-V SoCs: up to 5.9× speedup over software in RTL and 3.9× on FPGA, with a 109-LUT NoC load/store unit. Applied to an SoC with six coherent accelerators.</p>
    <p class="card__meta"><a href="/publication/2023-07-01-samos23">SAMOS ’23</a></p>
  </li>
  <li class="card">
    <span class="card__icon"><i class="fas fa-microchip"></i></span>
    <h3 class="card__title">RISC-V cores &amp; silicon</h3>
    <p class="card__desc">Sargantana core (I added its FPU) and its tapeouts down to 7 nm. I extended its vector unit to 512 bits, redesigning the permute, reduction and multiply datapaths to cut LUTs by 50% so a full core fits on one FPGA. Also OpenPiton-based manycores and hardware scheduler queues over the NoC.</p>
    <p class="card__meta"><a href="/publication/2022-08-01-sargantana-dsd">DSD ’22</a> · <a href="/publication/2024-07-01-openpiton4hpc">JETCAS ’24</a></p>
  </li>
  <li class="card">
    <span class="card__icon"><i class="fas fa-server"></i></span>
    <h3 class="card__title">RTL simulation at scale</h3>
    <p class="card__desc">Metro-MPI partitions RTL simulation over MPI: a 10B-transistor, 1,024-core SoC runs 136× faster than sequential Verilator. Its partitioning is now automated inside Verilator (DATE ’27) and being extended to gem5 and multi-FPGA emulation.</p>
    <p class="card__meta"><a href="/publication/2023-04-01-date23">DATE ’23</a> · <a href="/publication/2027-04-01-date27-auto-metro-mpi">DATE ’27</a> · <a href="/publication/2021-08-01-icpp21">ICPP ’21</a></p>
  </li>
  <li class="card">
    <span class="card__icon"><i class="fas fa-cogs"></i></span>
    <h3 class="card__title">Open EDA &amp; LLM-driven design</h3>
    <p class="card__desc">Technical lead of ODE4EC WP6 on open-source EDA tools, and co-advising work that evaluates open-weight LLM agents for RTL design on the CVDP benchmark.</p>
    <p class="card__meta">EU project ODE4EC</p>
  </li>
</ul>

News
======

<ul class="news" markdown="0">
  <li class="news__item">
    <span class="news__date">2026</span>
    <span class="news__text">Serving on the <strong>ISCA ’27</strong> full program committee and the <strong>HPCA ’27</strong> PC, after ISCA ’26, MICRO ’26 and CF ’26, and the artifact evaluation committees of ISCA ’26 and ASPLOS ’26.</span>
  </li>
  <li class="news__item">
    <span class="news__date">2026</span>
    <span class="news__text">Mentoring again for <strong>Google Summer of Code</strong> (FOSSi Foundation): Spike-based Linux checkpointing for RTL simulation and emulation.</span>
  </li>
  <li class="news__item">
    <span class="news__date">2026</span>
    <span class="news__text"><a href="/publication/2027-04-01-date27-auto-metro-mpi">Automatic Partitioning towards Faster Parallel RTL Simulations with Repeated Modules via MPI</a> accepted at <strong>DATE ’27</strong>, the outcome of my GSoC 2025 mentoring project.</span>
  </li>
  <li class="news__item">
    <span class="news__date">Jul 2025</span>
    <span class="news__text">Defended my PhD (<strong>Cum Laude</strong>) at UPC and started as postdoctoral researcher and research lead at BSC.</span>
  </li>
  <li class="news__item">
    <span class="news__date">2025</span>
    <span class="news__text">Invited seminar at <strong>Politecnico di Milano</strong>: <em>Past, Present and Future of Designing, Integrating and Simulating RTL Models</em>.</span>
  </li>
  <li class="news__item">
    <span class="news__date">2024</span>
    <span class="news__text"><a href="/publication/2024-06-01-hyperloops">The Case For Data Centre HyperLoops</a> (co-first author) presented at <strong>ISCA ’24</strong>.</span>
  </li>
</ul>

Get in touch
======

The fastest way to reach me is by [email](mailto:guillem.lopez.paradis@gmail.com). I am open to collaborations on CPU and SoC microarchitecture, memory systems, accelerator integration, RTL simulation and open EDA, and to research and engineering roles in computer architecture. You can also find me on [Google Scholar](https://scholar.google.com/citations?user=ookFZsQAAAAJ&hl=en), [GitHub](https://github.com/guillemlp), [LinkedIn](https://www.linkedin.com/in/guillemlopezparadis/) and [ORCID](https://orcid.org/0000-0002-5323-0761).

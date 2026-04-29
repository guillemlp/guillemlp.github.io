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
  <h1 class="hero__name">Guillem López Paradís</h1>
  <p class="hero__tagline">Computer architect — coherent accelerators, scalable RTL simulation, and LLM-driven hardware design.</p>
  <p class="hero__lede">Postdoctoral researcher and research lead at the Barcelona Supercomputing Center (BSC). I build accelerator-coherent memory systems and the simulation tooling that makes billion-transistor SoCs analysable.</p>
  <p class="hero__cta">
    <a class="btn btn--primary" href="/files/cv_guillem_lopez_paradis.pdf"><i class="fas fa-file-pdf"></i> Download CV</a>
    <a class="btn btn--ghost" href="https://scholar.google.com/citations?user=ookFZsQAAAAJ&hl=en"><i class="fas fa-graduation-cap"></i> Google Scholar</a>
    <a class="btn btn--ghost" href="https://github.com/guillemlp"><i class="fab fa-github"></i> GitHub</a>
    <a class="btn btn--ghost" href="https://www.linkedin.com/in/guillemlopezparadis/?locale=en_US"><i class="fab fa-linkedin"></i> LinkedIn</a>
  </p>
</section>

Selected research
======

<ul class="cards" markdown="0">
  <li class="card">
    <span class="card__tag">ISCA ’24</span>
    <h3 class="card__title"><a href="/publication/2024-06-01-hyperloops">Data Centre HyperLoops</a></h3>
    <p class="card__desc">Accelerator-coherent inter-chip fabric delivering 114×–646× faster data movement than 400 Gbps optical networks for ML workloads in hyperscale environments.</p>
    <p class="card__meta">Co-first author · UCSB collaboration</p>
  </li>
  <li class="card">
    <span class="card__tag">DATE ’23</span>
    <h3 class="card__title"><a href="/publication/2023-04-01-date23">Metro-MPI</a></h3>
    <p class="card__desc">Distributed RTL simulation parallelising behavioural Verilator with MPI — 1,024 cores, 134× speedup, billion-transistor SoCs become tractable.</p>
    <p class="card__meta">First author · Open source</p>
  </li>
  <li class="card">
    <span class="card__tag">SAMOS ’23</span>
    <h3 class="card__title"><a href="/publication/2023-07-01-samos23">Coherent accelerator framework</a></h3>
    <p class="card__desc">Characterisation of Arm’s coherent accelerator framework (ACAI) on SoCs, analysing the design trade-offs of accelerator-side coherence.</p>
    <p class="card__meta">First author · Arm collaboration</p>
  </li>
  <li class="card">
    <span class="card__tag">ICPP ’21</span>
    <h3 class="card__title"><a href="/publication/2021-08-01-icpp21">gem5 + RTL</a></h3>
    <p class="card__desc">Framework that drops RTL models into the gem5 full-system simulator, enabling hardware–software co-simulation across the stack.</p>
    <p class="card__meta">First author · Open source</p>
  </li>
  <li class="card">
    <span class="card__tag">2025 — New direction</span>
    <h3 class="card__title">LLM-driven hardware design</h3>
    <p class="card__desc">Agent-driven workflows for automated RTL generation, architectural exploration, and hardware–software co-design.</p>
    <p class="card__meta">Ongoing · BSC research lead</p>
  </li>
  <li class="card">
    <span class="card__tag">RISC-V</span>
    <h3 class="card__title">Open-source tape-outs</h3>
    <p class="card__desc">Contributor to multiple BSC academic RISC-V SoC tape-outs: Sargantana (22nm FD-SOI), DVINO (65nm), and earlier open-source silicon.</p>
    <p class="card__meta">DSD ’22 · DCIS ’20 / ’22 / ’23</p>
  </li>
</ul>

About me
======

I am a postdoctoral researcher and research lead at the Barcelona Supercomputing Center (BSC), specialising in **RTL simulation scalability**, **coherent accelerator memory systems**, and **scalable MPMC queue‑based communication for accelerators**. I completed my PhD in Computer Architecture (Cum Laude) at BSC–UPC in July 2025, with a thesis on *Efficient Data Movement in Large‑Scale Heterogeneous Systems*. My work has delivered **>100× speedups** in data movement for hyperscale environments (Data Centre HyperLoops, ISCA ’24) and pushed RTL simulation past billion‑transistor SoCs (Metro‑MPI, DATE ’23).

I currently lead a team of four researchers at BSC, coordinating international collaborations with **UCSB** and **Politecnico di Milano**, and I am driving a new research direction on **LLM‑based, agent‑driven workflows for hardware design** — automated RTL generation, architectural exploration, and hardware–software co‑design. I serve on the program committees for **ISCA ’26, MICRO ’26, CF ’26**, and on the artifact evaluation committees for **ISCA ’26** and **ASPLOS ’26**.

I am open to collaborations on accelerator coherence, RTL simulation, Metro‑MPI integrations, and LLM‑driven hardware design.

Education
======

<ul class="cv-list" markdown="0">
  <li class="cv-item">
    <h3 class="cv-item__title">Ph.D in Computer Architecture (Cum Laude)</h3>
    <p class="cv-item__sub">Polytechnic University of Catalonia (UPC) — Barcelona Supercomputing Center</p>
    <p class="cv-item__date">May 2021 – Jul 2025</p>
    <ul class="cv-item__bullets">
      <li>Thesis: <em>Efficient Data Movement in Large‑Scale Heterogeneous Systems</em></li>
      <li>Advisors: Prof. Adrià Armejach &amp; Prof. Miquel Moretó. Collaborators: Prof. Jonathan Balkind (UCSB), Dr. Balaji Venu (Arm)</li>
      <li>Architected Data Centre HyperLoops (DHL), the Metro‑MPI simulation framework, and scalable accelerator communication patterns</li>
      <li>Secured ~€107K in competitive research funding (FI Fellowship, NGI Fellowship, Severo Ochoa, FI Mobility)</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Visiting Scholar — Short-Term Scholar / NGI Fellow</h3>
    <p class="cv-item__sub">University of California, Santa Barbara (UCSB)</p>
    <p class="cv-item__date">Oct 2023 – Feb 2024 · Nov 2024 – May 2025</p>
    <ul class="cv-item__bullets">
      <li>Led a multidisciplinary group of 6 researchers (PhD, MSc, undergraduate) on accelerator coherence and communication fabrics</li>
      <li>Co‑developed Data Centre HyperLoops (ISCA ’24 co‑first author)</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">M.S. in Innovation and Research in Informatics (HPC)</h3>
    <p class="cv-item__sub">Polytechnic University of Catalonia (UPC) — GPA 8.9/10</p>
    <p class="cv-item__date">Feb 2018 – Nov 2020</p>
    <ul class="cv-item__bullets">
      <li>Awarded the <em>Nacho Navarro Grant</em> (top‑2 students in the HPC track)</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">B.S. in Informatics Engineering (Computer Engineering)</h3>
    <p class="cv-item__sub">Polytechnic University of Catalonia (UPC) — GPA 7.65/10</p>
    <p class="cv-item__date">Sep 2013 – Jul 2017</p>
    <ul class="cv-item__bullets">
      <li>BSc mobility exchange at École Polytechnique Fédérale de Lausanne (EPFL), Feb – Jul 2017 — GPA 5/6</li>
      <li><em>Honours in Embedded Systems</em> for an RTL sorting accelerator with &gt;10× speedup; Swiss mobility grant (€3K)</li>
    </ul>
  </li>
</ul>

Experience (Academia & Industry)
======

<ul class="cv-list" markdown="0">
  <li class="cv-item">
    <h3 class="cv-item__title">Postdoctoral Researcher &amp; Research Lead</h3>
    <p class="cv-item__sub">Barcelona Supercomputing Center (BSC) — Barcelona, Spain</p>
    <p class="cv-item__date">Jul 2025 – Present</p>
    <ul class="cv-item__bullets">
      <li>Manage the research agenda for a team of 4 (BSc, MSc, PhD, RE) and coordinate international collaborations with UCSB and Politecnico di Milano</li>
      <li>Lead the integration of Metro‑MPI into Verilator and large‑scale multi‑FPGA environments, and the design of SpMV accelerators in RTL</li>
      <li>Drive new research on LLM‑based, agent‑driven hardware design workflows — automating RTL generation and hardware–software co‑design</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">PhD Researcher</h3>
    <p class="cv-item__sub">Barcelona Supercomputing Center (BSC) — Barcelona, Spain</p>
    <p class="cv-item__date">May 2021 – Jul 2025</p>
    <ul class="cv-item__bullets">
      <li>Designed Data Centre HyperLoops (DHL): inter‑chip communication fabric — 114.8×–646.4× faster data movement vs. 400 Gbps optical networks for ML workloads (ISCA ’24)</li>
      <li>Scaled RTL simulation with Metro‑MPI: distributed framework reaching 1,024 cores with a 134× speedup, enabling billion‑transistor SoC simulations (DATE ’23)</li>
      <li>Implemented MPMC queue‑based accelerator interfaces (RTL + C libraries) with coherent memory subsystems across multiple RISC‑V designs (paper under review)</li>
      <li>Collaborations: EU projects EPI, DRAC, MEEP; industry Arm CoE, Intel; academia UCSB, HM</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Research Master Student</h3>
    <p class="cv-item__sub">Barcelona Supercomputing Center (BSC) — Barcelona, Spain</p>
    <p class="cv-item__date">Mar 2018 – Apr 2021</p>
    <ul class="cv-item__bullets">
      <li>MSc thesis: <em>Towards the Simulation and Emulation of Large‑Scale Hardware Designs</em></li>
      <li>Designed the gem5+RTL framework (ICPP ’21) and engineered NoC tracing for Mont‑Blanc 2020 (DATE ’21)</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Google Summer of Code — Mentor &amp; Student</h3>
    <p class="cv-item__sub">FOSSi (2025, 2021) · PCP (2018) — Remote</p>
    <p class="cv-item__date">2018 · 2021 · 2025</p>
    <ul class="cv-item__bullets">
      <li>Mentor (2025, FOSSi): automated Metro‑MPI in open‑source manycore workflows</li>
      <li>Student (2021, FOSSi): parallelised RTL simulation with MPI (1024 cores, 134× speedup; DATE ’23)</li>
      <li>Student (2018, PCP): production features for Performance Co‑Pilot, agent‑to‑agent data transmission</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Intern, XLABS</h3>
    <p class="cv-item__sub">Xilinx (now AMD) — Dublin, Ireland</p>
    <p class="cv-item__date">Aug 2017 – Feb 2018</p>
    <ul class="cv-item__bullets">
      <li>Evaluated scalability of the ACAP accelerator and maintained nightly regression for the accelerator simulator</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Undergraduate Researcher — EU Project RoMoL</h3>
    <p class="cv-item__sub">Barcelona Supercomputing Center (BSC) — Barcelona, Spain</p>
    <p class="cv-item__date">Jul 2016 – Feb 2017</p>
    <ul class="cv-item__bullets">
      <li>BSc thesis: integrated the Ramulator memory simulator into the trace‑driven simulator TaskSim</li>
      <li>Awarded the Spanish Ministry Beca de Colaboración (€2K)</li>
    </ul>
  </li>
</ul>

Invited Talks
======
* *Past, Present and Future of Designing, Integrating and Simulating RTL Models* — Invited Seminar, Politecnico di Milano, 2025  
* *Exascale Simulation of Next‑Generation Computing Architectures* — Invited Workshop Talk, IISWC 2023

Publications
======
* Advanced Communications Patterns Support for Hardware Accelerators — First author, *under review* (2025)  
* The Case For Data Centre HyperLoops — Co‑first author, ISCA 2024  
* Characterization of a Coherent Hardware Accelerator Framework for SoCs — First author, SAMOS 2023  
* Fast Behavioural RTL Simulation of 10B Transistor SoC Designs with Metro‑MPI — First author, DATE 2023  
* gem5+rtl: A Framework to Enable RTL Models Inside a Full‑System Simulator — First author, ICPP 2021  
* OpenPiton4HPC: Optimizing OpenPiton Toward High‑Performance Manycores — Co‑author, IEEE JETCAS 2024 (extends NoCArc @ MICRO 2023)  
* GenArchBench: A Genomics Benchmark Suite for Arm HPC Processors — Co‑author, Future Generation Computer Systems 2024  
* Sargantana: A 1 GHz+ In‑Order RISC‑V Processor — Co‑author, DSD 2022 (silicon tape‑out follow‑ups: DCIS 2022 / 2023)  
* Mont‑Blanc 2020: Towards Scalable and Power Efficient European HPC Processors — Co‑author, DATE 2021  
* An Academic RISC‑V Silicon Implementation Based on Open‑Source Components — Co‑author, DCIS 2020  
* First‑author posters at ACACES ’21/’19, BSCDS ’23, DAC ’23, and OSDA ’24  

A complete list is available on my [Google Scholar](https://scholar.google.com/citations?user=ookFZsQAAAAJ&hl=en) and [DBLP](https://dblp.org/pid/280/2104.html) profiles.

Academic Service
======
* **Program Committee:** ISCA ’26, MICRO ’26, CF ’26  
* **Artifact Evaluation Committee:** ISCA ’26 AEC, ASPLOS ’26 AEC  
* **External Reviewer:** IPDPS ’24, LATTE ’24, ICPP ’23, ICPP ’22, DATE ’21  
* **Volunteer:** RISC‑V Summit ’23 / ’19, FPL ’19  

Grants and Awards
======
* ~€107K in competitive research funding (undergrad → PhD), including the FI Fellowship, NGI Fellowship, Severo Ochoa, FI Mobility, and a Swiss mobility grant  
* DAC Young Fellow 2023; 2nd place in *PhD Thesis in 4 Minutes* contest at UPC, 2024  
* Nacho Navarro Grant (top‑2 students in the UPC HPC MSc track)  
* Beca de Colaboración (Spanish Ministry undergraduate research grant), 2017  
* Google Summer of Code student (2018, 2021) and mentor (2025)  
* 15+ hackathons with awards: GitHub Octocat Prize (Edinburgh 2018), 3rd place at Hack the Burgh (Edinburgh 2018), finalist at Copenhacks (Copenhagen 2018)  
* Start‑up experience: Forestal e‑bike (hardware–mobile app integration); accepted to Santander undergraduate start‑up programme  
* Co‑organiser of HackUPC, Europe’s largest student hackathon

Skills
======
* **Hardware tools:** gem5, Ramulator, Verilator, Vivado, ModelSim, VCS  
* **Hardware design:** SystemVerilog, VHDL, HLS, FPGAs (Xilinx)  
* **Software:** C/C++ (expert), Python (NumPy, Matplotlib), OpenMP, MPI, Linux kernel/drivers, GitLab CI/CD  
* **Domains:** Hyperscale data movement, coherent memory systems, hardware–software co‑design, SoC integration, RISC‑V, accelerators  

Beyond research
======
* Climbing (max bouldering grade 8a/V11), skiing, mountaineering, table tennis (national‑level competitor)  
* Languages: Catalan (native), Spanish (native), English (advanced — Duolingo 135/160), French (A1)

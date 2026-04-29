---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

[Download CV (PDF)]({{ base_path }}/files/cv_guillem_lopez_paradis.pdf){: .btn .btn--info}

Education
======
* Ph.D in Computer Architecture (Cum Laude), Polytechnic University of Catalonia (UPC), May 2021 – July 2025  
  * Thesis: *Efficient Data Movement in Large‑Scale Heterogeneous Systems*  
  * Advisors: Prof. Adrià Armejach & Prof. Miquel Moretó; collaborators: Prof. Jonathan Balkind (UCSB) & Dr. Balaji Venu (Arm)  
  * Architected the Data Centre HyperLoops (DHL), the Metro‑MPI simulation framework, and scalable accelerator communication patterns  
  * Secured ~€107K in competitive research funding (FI, NGI, Severo Ochoa, FI Mobility)  
* Visiting Scholar (Short‑Term Scholar / NGI Fellow), University of California, Santa Barbara (UCSB), Oct 2023 – Feb 2024 & Nov 2024 – May 2025  
  * Led a multidisciplinary group of 6 researchers (PhD, MSc, undergraduate); co‑developed Data Centre HyperLoops (ISCA ’24)  
* M.S. in Innovation and Research in Informatics (HPC track), Polytechnic University of Catalonia (UPC), Feb 2018 – Nov 2020 — GPA 8.9/10  
  * Awarded the *Nacho Navarro Grant* (top‑2 students in the HPC track)  
* B.S. in Informatics Engineering (Computer Engineering), Polytechnic University of Catalonia (UPC), Sep 2013 – July 2017 — GPA 7.65/10  
  * BSc mobility exchange, EPFL, Feb – July 2017 — GPA 5/6, *Honours in Embedded Systems* for an RTL sorting accelerator with >10× speedup; awarded a Swiss mobility grant (€3K)

Experience (Academia & Industry)
======
* Postdoctoral Researcher & Research Lead, Barcelona Supercomputing Center (BSC), July 2025 – Present  
  * Manage the research agenda for a team of 4 (BSc, MSc, PhD, RE); coordinate international collaborations with UCSB and Politecnico di Milano  
  * Lead the integration of Metro‑MPI into Verilator and large‑scale multi‑FPGA environments; design SpMV accelerators in RTL  
  * Drive new research on LLM‑based, agent‑driven hardware design — automated RTL generation and HW–SW co‑design  
* PhD Researcher, Barcelona Supercomputing Center (BSC), May 2021 – July 2025  
  * Designed Data Centre HyperLoops (DHL): 114.8×–646.4× faster data movement vs. 400 Gbps optical networks for ML workloads (ISCA ’24)  
  * Scaled RTL simulation with Metro‑MPI: distributed framework reaching 1,024 cores with a 134× speedup (DATE ’23)  
  * Implemented MPMC queue‑based accelerator interfaces with coherent memory subsystems across multiple RISC‑V designs (paper under review)  
  * Collaborations: EPI, DRAC, MEEP; Arm CoE, Intel; UCSB, HM  
* Research Master Student, Barcelona Supercomputing Center (BSC), March 2018 – April 2021  
  * MSc thesis: *Towards the Simulation and Emulation of Large‑Scale Hardware Designs*  
  * Designed gem5+RTL (ICPP ’21); engineered NoC tracing for Mont‑Blanc 2020 (DATE ’21)  
* Google Summer of Code — Mentor (2025) & Student (2021, 2018)  
  * Mentor (2025, FOSSi) automated Metro‑MPI; Student (2021, FOSSi) parallelised RTL simulation with MPI; Student (2018, PCP) shipped Performance Co‑Pilot features  
* Intern, XLABS — Xilinx (now AMD), Dublin, August 2017 – February 2018  
  * Evaluated scalability of the ACAP accelerator and maintained nightly regression for the accelerator simulator  
* Undergraduate Researcher (EU Project RoMoL), Barcelona Supercomputing Center (BSC), July 2016 – February 2017  
  * Integrated the Ramulator memory simulator into TaskSim; awarded the Spanish Ministry Beca de Colaboración (€2K)

Invited Talks
======
* *Past, Present and Future of Designing, Integrating and Simulating RTL Models* — Invited Seminar, Politecnico di Milano, 2025  
* *Exascale Simulation of Next‑Generation Computing Architectures* — Invited Workshop Talk, IISWC 2023

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Academic Service
======
* **Program Committee:** ISCA ’26, MICRO ’26, CF ’26  
* **Artifact Evaluation Committee:** ISCA ’26 AEC, ASPLOS ’26 AEC  
* **External Reviewer:** IPDPS ’24, LATTE ’24, ICPP ’23, ICPP ’22, DATE ’21  
* **Volunteer:** RISC‑V Summit ’23 / ’19, FPL ’19  

Grants and Awards
======
* ~€107K in competitive research funding from undergrad → PhD (FI, NGI, Severo Ochoa, FI Mobility, Swiss mobility)  
* DAC Young Fellow 2023; 2nd place, *PhD Thesis in 4 Minutes* contest (UPC, 2024)  
* Nacho Navarro Grant (top‑2 students in the UPC HPC MSc track)  
* Beca de Colaboración (Spanish Ministry undergraduate research grant), 2017  
* Google Summer of Code student (2018, 2021) and mentor (2025)  
* 15+ hackathons: GitHub Octocat Prize (Edinburgh 2018), 3rd place at Hack the Burgh, Copenhacks finalist  
* Forestal e‑bike start‑up; accepted to Santander undergraduate start‑up programme  
* Co‑organiser, HackUPC

Skills
======
* **Hardware tools:** gem5, Ramulator, Verilator, Vivado, ModelSim, VCS  
* **Hardware design:** SystemVerilog, VHDL, HLS, FPGAs (Xilinx)  
* **Software:** C/C++ (expert), Python (NumPy, Matplotlib), OpenMP, MPI, Linux kernel/drivers, GitLab CI/CD  
* **Domains:** Hyperscale data movement, coherent memory systems, hardware–software co‑design, SoC integration, RISC‑V, accelerators  
* **Languages:** Catalan (native), Spanish (native), English (advanced — Duolingo 135/160), French (A1)

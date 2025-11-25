---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

Education
======
* Ph.D in Computer Architecture (Cum Laude), Polytechnic University of Catalonia (UPC), July 2025  
  * Title: Efficient Data Movement in Large‑Scale Heterogeneous Systems  
  * Advisors: Dr. Adrià Armejach & Prof. Miquel Moretó; collaborators: Prof. Jonathan Balkind (UCSB) & Dr. Balaji Venu (Arm)  
  * Contributions: scalable RTL simulation (Metro‑MPI), coherent accelerator memory subsystems, optimisations for OpenPiton, and open‑source RISC‑V tapeouts  
* Visiting Scholar, University of California, Santa Barbara (UCSB), Oct 2023 – Feb 2024 & Nov 2024 – May 2025  
  * Research on accelerator coherence and communication fabrics; co‑developed Data Centre HyperLoops (ISCA’24 co‑first author)  
* M.S. in Innovation and Research in Informatics (HPC), Polytechnic University of Catalonia (UPC), 2020  
* B.S. in Informatics Engineering, Polytechnic University of Catalonia (UPC), 2017  
  * BSc mobility exchange, Ecole Polytechnique Federale De Lausanne (EPFL), 2017 (honors in final RTL accelerator project)

Experience (Academia & Industry)
======
* PhD Researcher, Barcelona Supercomputing Center (BSC), May 2021 – July 2025  
  * Designed coherent accelerator memory subsystems, contributed to open‑source RISC‑V tapeouts, and advanced large‑scale simulation (Metro‑MPI, gem5)  
* Research Master Student, Barcelona Supercomputing Center (BSC), March 2018 – April 2021  
  * MSc thesis: Towards the Simulation and Emulation of Large‑Scale Hardware Designs; integrated RTL models into gem5 (gem5+RTL, ICPP ’21)  
* Google Summer of Code — Mentor (2025) & Student (2021, 2018), Google Summer of Code  
  * Mentored the automatisation of Metro‑MPI; parallelised RTL simulations with MPI (up to 1024 cores, 134× speedup, DATE ’23); delivered production features for PCP  
* Intern, Xilinx Labs (XLABS), Dublin, August 2017 – February 2018  
  * Analysed accelerator scalability on emerging FPGA architectures and maintained nightly regression for the simulator  
* Undergraduate Researcher (EU Project RoMoL), Barcelona Supercomputing Center (BSC), July 2016 – February 2017  
  * Integrated the Ramulator memory simulator into TaskSim; awarded the Spanish Ministry Beca de Colaboración

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Achievements and awards
======
* Secured competitive grants from undergrad to PhD level (∼ €90K), including FI Fellowship, NGI Fellowship, Severo Ochoa, and mobility awards  
* DAC Young Fellow 2023 and 2nd place in “Presenting the PhD thesis in 4 minutes” (UPC, 2024)  
* Google Summer of Code student (2018, 2021) and mentor (2025); participated in 15+ hackathons with awards (GitHub Octocat Prize, Hack the Burgh 3rd place, finalist at Copenhacks)  
* Start‑up experience (Forestal e‑bike): led comms between bike hardware and mobile app; accepted to Santander undergrad start‑up program  
* Beca de Colaboración (Spanish Ministry undergraduate research grant), 2017  
* Active conference involvement: PC member (ISCA’26, CF’26); reviewer (IPDPS’24, WOSET’24, LATTE’24, ICPP’23/’22, DATE’21); volunteer at RISCV Summit and FPL

Skills
======
* Programming: C/C++, Python (ggplot, numpy, matplotlib), Verilog/SystemVerilog, VHDL, Assembly, Bash, Java, JavaScript  
* Tools: Linux, git/GitLab CI, Verilator, Vivado, ModelSim, GHDL, VCS, gem5, Ramulator; Xilinx FPGAs  
* Languages: Catalan (native), Spanish (native), English (advanced), French (basic)

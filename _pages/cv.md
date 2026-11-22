---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

<p class="page__lede" markdown="0">
  Computer architecture researcher (<strong>PhD, BSC–UPC, 2025, Cum Laude</strong>) working on
  <strong>coherent accelerator integration</strong> in <strong>RISC-V manycore SoCs</strong>.
</p>

<p class="cv-actions" markdown="0">
  <a class="btn btn--primary" href="{{ base_path }}/files/cv_guillem_lopez_paradis.pdf"><i class="fas fa-file-pdf"></i> Download CV (PDF)</a>
</p>

Experience
======

<ul class="cv-list" markdown="0">
  <li class="cv-item">
    <h3 class="cv-item__title">Postdoctoral Researcher &amp; Research Lead</h3>
    <p class="cv-item__sub">Barcelona Supercomputing Center (BSC) · Barcelona, Spain</p>
    <p class="cv-item__date">Jul 2025 – Present</p>
    <ul class="cv-item__bullets">
      <li>Advising a PhD student and managing a team of 4 (BSc, MSc, PhD, RE); coordinating collaborations with <strong>UCSB</strong> and <strong>PoliMilano</strong>.</li>
      <li><strong>Technical lead</strong> at BSC for <strong>WP6</strong> of the EU project <strong>ODE4EC</strong> on open-source EDA tools.</li>
      <li><strong>TMU sparse accelerator:</strong> leading a student team implementing the TMU-based SpMV accelerator in RTL with the <strong>Arm CoE</strong>; 2–3× over CPU software (RTL simulation).</li>
      <li><strong>Hardware scheduler queues:</strong> designing RTL for hardware-assisted task scheduling over OpenPiton's NoCs; validated on FPGA and in RTL simulation.</li>
      <li><strong>Accelerator-rich SoC:</strong> designed the MPMC HW queues of a RISC-V SoC with 6 coherent accelerators (1.9–5.5× over SW) and ported it to FPGA.</li>
      <li><strong>Performance analysis:</strong> integrated Mess and TopDown into FPGA/SoC evaluation; found and fixed NoC, cache and memory-controller bottlenecks, improving measured memory bandwidth by <strong>10×</strong>.</li>
      <li>Co-advising a student on <strong>LLM-based hardware design</strong>: evaluating open-weight LLM agents for RTL design on the CVDP benchmark.</li>
      <li>Leading Metro-MPI integration into <strong>Verilator</strong>, <strong>gem5</strong> and multi-FPGA emulation; co-advised a summer intern (with UCSB) on UBQ.</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">PhD Researcher</h3>
    <p class="cv-item__sub">Barcelona Supercomputing Center (BSC) · Barcelona, Spain</p>
    <p class="cv-item__date">May 2021 – Jul 2025</p>
    <ul class="cv-item__bullets">
      <li><strong>Hardware queues for accelerators:</strong> designed MPMC queue endpoints on coherent memory for RISC-V SoCs: up to 5.9× over software in RTL and 3.9× on FPGA, with a minimal 109-LUT NoC LSU.</li>
      <li><strong>RISC-V silicon:</strong> helped design Sargantana (added its FPU); participated in its tapeouts down to 7 nm and in OpenPiton-based ones.</li>
      <li><strong>Metro-MPI (DATE ’23):</strong> simulation of a 10B-transistor, 1,024-core SoC; 136× faster than sequential Verilator (64 cores) with 2.5× less regression energy.</li>
      <li><strong>Data Centre HyperLoops (ISCA ’24):</strong> 1.6–376× less energy and 115–646× faster than 400 Gbps optics when moving a 29 PB ML dataset.</li>
      <li>Collaborations with EU projects (EPI, DRAC, MEEP), industry (Arm CoE, Intel) and academia (UCSB, HM).</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Visiting Scholar (Short-Term Scholar / NGI Fellow)</h3>
    <p class="cv-item__sub">University of California, Santa Barbara (UCSB) · Santa Barbara, USA</p>
    <p class="cv-item__date">Oct 2023 – Feb 2024<br>Nov 2024 – May 2025</p>
    <ul class="cv-item__bullets">
      <li>Led a team of 6 researchers (PhD, MSc and undergraduate students).</li>
      <li>Studied on-chip data movement in OpenPiton manycores and co-developed DHL for off-chip data movement (ISCA ’24).</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Google Summer of Code Mentor</h3>
    <p class="cv-item__sub">FOSSi Foundation · Remote</p>
    <p class="cv-item__date">Summers 2025, 2026</p>
    <ul class="cv-item__bullets">
      <li><strong>2026:</strong> Spike-based Linux checkpointing for RTL simulation and emulation.</li>
      <li><strong>2025:</strong> integrating the Metro-MPI partitioning automation into Verilator (paper accepted at DATE ’27).</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Research Master Student</h3>
    <p class="cv-item__sub">Barcelona Supercomputing Center (BSC) · Barcelona, Spain</p>
    <p class="cv-item__date">Mar 2018 – Apr 2021</p>
    <ul class="cv-item__bullets">
      <li>MSc thesis: <em>Towards the Simulation and Emulation of Large-Scale Hardware Designs</em>.</li>
      <li>Designed the <strong>gem5+RTL</strong> framework (ICPP ’21), enabling co-simulation of RTL accelerators inside a full-system simulator.</li>
      <li>Engineered NoC tracing for Mont-Blanc 2020, enabling on-chip interconnect analysis of Exascale-ready processors (DATE ’21).</li>
      <li>Awarded the <strong>Nacho Navarro Grant</strong>, given to the top 2 students in the HPC track.</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Intern, XLABS (Research &amp; Product Team)</h3>
    <p class="cv-item__sub">Xilinx (now AMD) · Dublin, Ireland</p>
    <p class="cv-item__date">Aug 2017 – Feb 2018</p>
    <ul class="cv-item__bullets">
      <li>Evaluated the scalability of the reconfigurable ACAP on neural-network and networking benchmarks.</li>
      <li>Maintained critical components of the accelerator simulator's nightly regression infrastructure.</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Undergraduate Researcher (EU Project RoMoL)</h3>
    <p class="cv-item__sub">Barcelona Supercomputing Center (BSC) · Barcelona, Spain</p>
    <p class="cv-item__date">Jul 2016 – Feb 2017</p>
    <ul class="cv-item__bullets">
      <li>BSc thesis: integrated the Ramulator DRAM simulator into TaskSim to evaluate future memory technologies in multicore processors.</li>
      <li>Awarded the Spanish Ministry's <strong>Beca de Colaboración</strong> undergraduate research grant (€2k).</li>
    </ul>
  </li>
</ul>

Education
======

<ul class="cv-list" markdown="0">
  <li class="cv-item">
    <h3 class="cv-item__title">PhD in Computer Architecture · Cum Laude</h3>
    <p class="cv-item__sub">Polytechnic University of Catalonia (UPC)</p>
    <p class="cv-item__date">May 2021 – Jul 2025</p>
    <ul class="cv-item__bullets">
      <li>Thesis: <em>Efficient Data Movement in Large-Scale Heterogeneous Systems</em>.</li>
      <li>Advisors: Prof. Adrià Armejach &amp; Prof. Miquel Moretó. Collaborators: Prof. Jonathan Balkind (UCSB) &amp; Dr. Balaji Venu (Arm).</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">MSc in Innovation and Research in Informatics</h3>
    <p class="cv-item__sub">UPC · Specialisation in High-Performance Computing · GPA 8.9/10</p>
    <p class="cv-item__date">Feb 2018 – Nov 2020</p>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">BSc Mobility Exchange</h3>
    <p class="cv-item__sub">École Polytechnique Fédérale de Lausanne (EPFL)</p>
    <p class="cv-item__date">Feb 2017 – Jul 2017</p>
    <ul class="cv-item__bullets">
      <li>Honours in Embedded Systems for an RTL sorting accelerator with &gt;10× speedup; awarded a Swiss mobility grant (€3k).</li>
    </ul>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Bachelor in Informatics Engineering</h3>
    <p class="cv-item__sub">UPC · Specialisation in Computer Engineering</p>
    <p class="cv-item__date">Sep 2013 – Jul 2017</p>
  </li>
</ul>

Invited Talks
======

<ul class="cv-list" markdown="0">
  <li class="cv-item">
    <h3 class="cv-item__title">Past, Present and Future of Designing, Integrating and Simulating RTL Models</h3>
    <p class="cv-item__sub">Invited Seminar · Politecnico di Milano</p>
    <p class="cv-item__date">2025</p>
  </li>
  <li class="cv-item">
    <h3 class="cv-item__title">Exascale Simulation of Next-Generation Computing Architectures</h3>
    <p class="cv-item__sub">Invited Workshop Talk · IISWC</p>
    <p class="cv-item__date">2023</p>
  </li>
</ul>

Publications
======

Full list with links on the [publications page](/publications/). Posters: ACACES ’21/’19, BSCDS ’23, DAC ’23, OSDA ’24.

<ul class="pub-compact" markdown="0">
{% for post in site.publications reversed %}
  <li>
    <span class="pub-compact__year">{{ post.date | date: "%Y" }}</span>
    <span class="pub-compact__body">
      <a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a>
      <span class="pub-compact__venue">{{ post.venue }}{% if post.role %} · <span class="pub-badge">{{ post.role }}</span>{% endif %}</span>
    </span>
  </li>
{% endfor %}
</ul>

Professional Service
======

* **Program Committee:** ISCA ’27 (full PC), HPCA ’27, ISCA ’26, MICRO ’26, CF ’26
* **Artifact Evaluation Committee:** ASPLOS ’26, ISCA ’26
* **Reviewer:** IPDPS ’24, LATTE ’24, ICPP ’23/’22, DATE ’21
* **Volunteer:** RISC-V Summit ’23/’19, FPL ’19

Awards &amp; Achievements
======

* **DAC Young Fellow** (2023)
* **2nd place**, *PhD Thesis in 4 Minutes* communication contest, UPC (2024)
* ~**€107,000** in competitive grants at undergraduate, master and PhD level (2016 – present), including the Beca de Colaboración (2017)
* **Google Summer of Code:** student twice (17% and 27% acceptance rates) and mentor twice (2018 – 2026)
* **15+ hackathons**, including the GitHub Octocat Prize and 3rd place at Hack the Burgh (2018); helped organise HackUPC, Europe's largest student hackathon
* **Start-ups:** led bike–app HW/SW integration at the e-bike start-up Forestal; accepted into Santander's YUZZ programme for young entrepreneurs

Skills
======

<dl class="skills" markdown="0">
  <dt>Hardware</dt>
  <dd>gem5, Ramulator, Verilator, Vivado, ModelSim, VCS · SystemVerilog, VHDL, HLS, FPGAs</dd>
  <dt>Software</dt>
  <dd>C/C++ (expert), Python (NumPy, Matplotlib), OpenMP, MPI, Linux kernel/drivers, GitLab CI/CD</dd>
  <dt>Domains</dt>
  <dd>SoC architecture, coherent accelerator integration, memory hierarchy &amp; coherence, NoCs, RISC-V manycores, HW/SW co-design</dd>
  <dt>Methods</dt>
  <dd>RTL microarchitecture, performance profiling, FPGA prototyping, performance modelling &amp; analysis</dd>
  <dt>Languages</dt>
  <dd>Catalan and Spanish (native), English (fluent, C1), French (A1)</dd>
  <dt>Interests</dt>
  <dd>Climbing (8a/V11 bouldering), skiing, mountaineering, table tennis (national level)</dd>
</dl>

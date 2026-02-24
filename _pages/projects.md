---
layout: page
title: Research
permalink: /research/
description: Professional Experience & Academic Portfolio
nav: true
nav_order: 2
---

<!-- Professional Summary (source: research_master.md [Website Version - English]) -->

### Bridging Academic Rigor and Production-Ready Inspection

I am an Optical Engineer with a Ph.D. from the **Computational Imaging & Instrumentation Laboratory** and **over 3 years of industry R&D** at **Koh Young Technology** (global leader in 3D measurement & inspection, SPI/AOI). My **industrial strength** comes from what I have actually built and led: **simulation-driven concept validation** (Blender, Python) and **inverse design with joint optimization** (Zemax–MATLAB API) for inspection systems — **delivering:** **Active multi-view stereo** and photometric fusion for specular 3D (lead); **extended depth-of-field for wire bonding inspection** (lead); and **multi-wavelength fluorescence imaging for 2 µm pitch RDL with PID** (lead) on 300mm wafers; optimized **digital holography** algorithms for BGA micro-bump inspection. I serve as **technical anchor** for cross-functional teams, own **calibration** and **field support**, and drive products from concept to mass production.

Understanding of **AOI/SPI** including **back-end semiconductor** inspection. I am not "optics-only"; I keep process and manufacturability in mind when working on optical solutions. My academic backbone (Physics-Informed Deep Learning, End-to-End Optimization) supports this execution.

---

## Part I: Professional Experience (Industry)

> **Core Competency:** "Rapid Prototyping, Troubleshooting, and Technical Ownership."

### 1. Computational Inline Inspection System (AOI-AXIA): Multi-view Stereo & Photometry Fusion

**Accelerating Development via Rapid Prototyping**
I initiated this project as a solo proof-of-concept using Blender simulations. Recognizing its potential, the company adopted it as a major next-generation product. My role was to pave the way: I built the physical prototype alone using off-the-shelf components and developed the initial operation software in Python.

**Core Algorithm Development**
Beyond system integration, I led the development of critical computer vision algorithms. I implemented **Active Multi-view Stereo (MVS)** to generate high-precision depth maps in an active structured-light configuration, and pioneered a **Gradient Fusion** technique to successfully reconstruct **specular surfaces**, solving a major inspection challenge for reflective materials.

**The Technical Anchor**
While the Vision group developed the final C++ product code, I provided the "reference standard." I shared my Python reconstruction pipelines and datasets, allowing them to develop software in parallel with my hardware setup. I defined the critical hardware specifications and calibration logic, serving as the technical "go-to" person for the entire inter-departmental team. My deep understanding of the system's "A to Z" significantly shortened the overall development cycle.

<br>

### 2. Interferometry-Based High-Throughput Inspection (ZenStar)

**Reliability Engineering & Troubleshooting**
Leveraging my background in **Multi-wavelength Digital Holography**, I was invited to the ZenStar project to solve persistent technical challenges. I did not design the initial system, but I made it work reliably. I reviewed and optimized the image reconstruction algorithms in Python, which were then ported to C++ by the software team.

**Solving the "Unsolvable"**
My value shone in troubleshooting. I identified and fixed subtle optical issues that plagued performance, such as ghosting in polarization elements and wavelength drift caused by temperature changes. Crucially, I optimized the **wavefront curvature mismatch** in the Mach-Zehnder interferometer, ensuring **uniform reconstruction performance across the entire Field of View (FoV)**, which was critical for meeting the strict accuracy requirements of **BGA (Ball Grid Array) micro-bump** inspection.

<br>

### 3. Extended Depth-of-Field for Micro-Bump Inspection (Fringe Projection)

**Bridging Theory and Industry: Real-Time DoF Extension**
Leveraging my academic background in **Pupil Engineering**, I led a project to overcome the trade-off between depth-of-field and resolution in telecentric imaging system for Optical Character Recognition (OCR) of PCB device and Fringe Projection Profilometry. I applied a **Computational Inverse Design** approach, utilizing Particle Swarm Optimization (PSO) to jointly optimize the pupil filter and coressponding post-processing.

**FPGA Implementation & Innovation**
To ensure the solution was practical for mass production, I successfully transferred the **jointly-optimized post-processing** into the **Camera FPGA**, enabling real-time Depth-of-Field extension with zero additional computational load on the host PC. I also devised a new way to fabricate phase plates, successfully reducing **artifacts inherent to phase filters that appear near metallic specular reflections**—a critical hurdle in industrial inspection.

<br>

### 4. High-Speed Large-Area Topology Measurement Prototype (VSI/WLI)

**Rapid Prototyping for Speed**
Targeting high-speed large-area **micron-scale** topology measurement, I developed a specialized VSI/WLI prototype. I identified that for our specific needs (topology over roughness), a specific light source bandwidth could drastically reduce scanning time. I built the system independently using standard optical components, proving the concept's speed and accuracy through rigorous hands-on testing.

<br>

### 5. High-Speed 300mm Wafer Fluorescence Imaging System

**Leveraging Material Properties for System Innovation**
While analyzing customer wafers, I **observed** that the fluorescence brightness of **Photo Imageable Dielectric (PID)** layers varied significantly due to thickness differences in multi-layer structures, complicating image processing.

**From Observation to Prototype**
Recognizing that different excitation wavelengths have different **penetration depths** (transmittance), I designed a **multi-wavelength line scan fluorescence imaging system** **using commercially available (COTS) optical components**. By combining signals from deep-penetrating and shallow-penetrating wavelengths, I could successfully **disentangle the layer structure** of the PID, overcoming the limitations of single-wavelength inspection. I built this prototype from scratch to scan 300mm wafers, proving that applying physical insights can solve persistent inspection challenges.

---

## Part II: Academic Research Portfolio

> **Core Strategy:** "Deep Theoretical Foundation to support Practical Engineering." (Using AI/Physics knowledge to solve what traditional methods cannot).

### 1. Physics-Informed & Data-Driven Optical Logic (Design Innovation)

**Breaking the Boundary between Hardware and Software**
Traditional optical systems are designed first, and image processing algorithms are developed later to fix their imperfections. I challenged this sequential paradigm by proposing an **End-to-End (E2E) Design Framework**. In my research (`seong2023e2e`), I modeled the physical wave propagation of a **Binary Phase Filter (BPF)** as a differentiable layer in a neural network. This allowed me to "train" the physical shape of the lens and the image reconstruction network **simultaneously**.

**Physics-Informed AI & Mathematical Optimization**
My approach is grounded in both modern AI and classical mathematics. I developed an **"Untrained" network** (`seong2023untrained`) that learns solely from physical consistency (Physics Loss), eliminating the need for labeled data. Furthermore, I successfully adapted **Topology Optimization** methods (`roper2020topology`) to optics. By manipulating the phase in the **Fourier domain** to optimize the **image domain** response, I demonstrated that cross-disciplinary optimization techniques can solve complex optical design problems.

**Versatile Optical Design**
Beyond AI, I possess strong capabilities in designing classical **Diffractive Optical Elements (DOEs)**. I designed specialized **Binary Phase Filters** for Oblique LSFM (`yun2025oblique`) and **Fresnel Zone Plates** for micro-optics research (`han2020direct`), proving my versatility in creating key optical components for diverse imaging modalities.

**Relevant Publications & Patents:**

- {% reference seong2023e2e %} [Link]({{ site.data.project_links.seong2023e2e }})
- {% reference seong2023untrained %} [Link]({{ site.data.project_links.seong2023untrained }})
- {% reference roper2020topology %} [Link]({{ site.data.project_links.roper2020topology }})
- {% reference us12541819 %} [Link]({{ site.data.project_links.us12541819 }})
- {% reference yun2025oblique %} [Link]({{ site.data.project_links.yun2025oblique }})
- {% reference han2020direct %} [Link]({{ site.data.project_links.han2020direct }})

<br>

### 2. Advanced System Instrumentation & Control (System Engineering)

**From Concept to Fully Operational System**
I distinguish myself by my ability to build systems "A to Z." For my LSFM research (`ryu2020light`), I integrated a **Spatial Light Modulator (SLM)** to manipulate the illumination sheet and an **Electrically Tunable Lens (ETL)** in the detection path to extend the imaging volume without moving the sample. I handled the complete control logic using **Python and LabVIEW**.

**System Integration for Industrial & Bio-Imaging**
My system engineering expertise extends to OCT. For industrial battery materials (`us11846587`), I developed an **Inline Spectral Domain OCT (SD-OCT)** using an imaging spectrometer to achieve **micron-level axial resolution**. Conversely, for bio-imaging (`han2025dual`), I built a **Swept-Source OCT (SS-OCT)** equipped with **galvo-scanners** to rapidly image tumor spheroids. In both cases, I constructed the hardware from scratch and established the data acquisition pipelines.

**Relevant Publications & Patents:**

- {% reference ryu2020light %} [Link]({{ site.data.project_links.ryu2020light }})
- {% reference us11846587 %} [Link]({{ site.data.project_links.us11846587 }})
- {% reference han2025dual %} [Link]({{ site.data.project_links.han2025dual }})

---
layout: page
title: Research
permalink: /research/
description: Professional Experience & Academic Portfolio
nav: true
nav_order: 2
---

<!-- Professional Summary -->
### Bridging Theoretical Innovation and Industrial Reality

I am an Optical and Computational Imaging Engineer dedicated to solving complex visibility problems through the fusion of **Physics** and **Artificial Intelligence**. With a Ph.D. in Mechanical Engineering and experience as a Lead Researcher at Koh Young Technology, I possess a unique **"T-shaped" profile**: deep theoretical expertise in **Physics-Informed Deep Learning** backed by the broad practical ability to lead **full-cycle product development**.

My journey spans from inventing **end-to-end deep learning microscopes** that break physical resolution limits to orchestrating the mass production of **next-generation 3D inspection systems** for the semiconductor industry. I don't just simulate ideas; I build robust systems, write production-grade algorithms, and deliver tangible solutions that work in the real world.

---

## Part I: Professional Experience (Industry)

> **Core Competency:** Full-cycle Product Development Leadership (Concept → Prototype → Mass Production)

### 1. Inline Photometric Stereo & Stereo Vision Inspection System (AOI-AXIA)

**From Virtual Simulation to Real-World Inspection**
I spearheaded the development of the AOI-AXIA inline inspection system, a project that exemplifies my ability to drive innovation from a vague concept to a robust industrial product. The journey began in a virtual environment; I utilized **Blender** to generate photorealistic synthetic datasets, allowing me to design the image acquisition pipeline and optimize optical parameters (such as stereo baseline and lighting angles) before spending a single dollar on hardware.

**Prototyping & Technology Adoption**
Moving from simulation to reality, I constructed a proof-of-concept prototype on an optical table using carefully selected off-the-shelf components. I developed the entire operation software in Python, integrating motion stages, cameras, and illumination triggers. The successful demonstration of this prototype convinced stakeholders to adopt this technology as a core feature for the next-generation inspection machine.

**Cross-Functional Leadership & Deployment**
My role extended beyond optics. I acted as a bridge between departments, providing the Software and Vision groups with Python-based reconstruction algorithms and synthetic data early in the process, enabling parallel development. For mass production, I designed comprehensive calibration scenarios (Stereo, Photometric, Camera-Stage alignment) and documented them with executable Python code, ensuring that the transition from R&D to the factory floor was seamless.

<br>

### 2. Interferometry-Based High-Throughput Inspection (ZenStar)

**Reliability Engineering in Advanced Interferometry**
For the ZenStar project, a high-throughput 3D inspection system based on interferometry, I focused on turning a complex optical design into a reliable industrial tool. My primary contribution was in **system optimization and troubleshooting**. I participated in defining the optical specifications and fine-tuned the system settings to accommodate various customer specimen properties.

**Algorithm & Troubleshooting**
I implemented and optimized image reconstruction algorithms for phase unwrapping and noise reduction, ensuring high-precision measurement of semiconductor micro-bumps. Beyond software, I tackled persistent hardware challenges. I successfully identified and resolved critical issues such as ghosting in polarization elements, focal shifts, and wavelength drift caused by external temperature changes. I also analyzed the impact of wavefront curvature in the Mach-Zehnder interferometer on reconstruction performance, ensuring stable operation in the field.

<br>

### 3. Extended Depth-of-Field for Micro-Bump Inspection

**Bridging Theory and Industry: Real-Time DoF Extension**
Leveraging my academic background in **Pupil Engineering**, I led a project to overcome the depth-of-field limitations in Fringe Projection Profilometry for micro-bump inspection. The challenge was not just theoretical but practical: implementing complex image processing without slowing down the inspection cycle.

**FPGA Implementation & Innovation**
I successfully transferred the post-processing algorithms into the **Camera FPGA**, enabling real-time Depth-of-Field extension with zero additional computational load on the host PC. I directly managed the collaboration with FPGA vendors to achieve this integration. Furthermore, I addressed a critical side effect of pupil engineering—artifacts caused by specular reflection. I devised and fabricated a **novel phase plate** design that suppresses these artifacts while preserving the extended depth of field, proving that advanced optical theory can be robustly applied to reflective industrial surfaces.

**Relevant Publications & Patents:**
*   `US 20250207912 A1`: Apparatus for Three-Dimensional Shape Measurement (Patent Application)

<br>

### 4. High-Speed Large-Area Topology Measurement Prototype

**Rapid Prototyping for High-Speed Topology**
Faced with a requirement for a high-speed large-area topology measurement solution, I led the development of a specialized prototype based on **Vertical Scanning Interferometry (VSI/WLI)**. Unlike traditional WLI focused on roughness, our goal was pure topology.

**Smart Engineering**
I strategically selected a specific light source bandwidth to minimize the number of required vertical scanning steps, significantly increasing measurement speed. I built the entire system from the ground up using **off-the-shelf optical elements** (such as Mirau objectives), conducting hands-on sessions to verify that the concept could deliver the required speed and accuracy for large-area inspection.

---

## Part II: Academic Research Portfolio

> **Core Strategy:** Physics-Informed Innovation & Technical Depth

### 1. Physics-Informed & Data-Driven Optical Logic (Design Innovation)

**Breaking Physical Limits with AI-Optics Co-Design**
My academic research centers on breaking the fundamental trade-offs in optics—such as Resolution vs. Depth-of-Field—by integrating **Deep Learning (DL)** and **Machine Learning (ML)** directly into the physical design process. Unlike black-box AI, I advocate for **Physics-Informed AI**, where optical laws guide the learning process.

{% include figure.liquid path="assets/project_figure/e2e-bpf-9.png" class="img-fluid rounded z-depth-1" alt="E2E-BPF microscopy" avoid_scaling=true %}

**End-to-End Deep Learning**
My signature work, the **E2E-BPF Microscope**, utilized an **end-to-end deep learning** framework to design a Binary Phase Filter (BPF) that creates a specific point spread function (PSF) ideally suited for DL-based restoration. This data-driven approach extended the DoF by six times, a feat impossible with conventional design methods. I also explored **Untrained Neural Networks**, proving that physics-guided algorithms can solve complex phase retrieval problems without the need for massive training datasets.

**Relevant Publications & Patents:**
*   `seong2023e2e`: **E2E-BPF Microscope** (Light: Science & Applications)
*   `seong2023untrained`: **Untrained Deep Learning-Based Differential Phase-Contrast Microscopy** (Optics Letters)
*   `US 12,541,819 B2`: Method for Designing Binary Phase Filter (Patent Granted)

<br>

### 2. System Instrumentation & Integration

**Mastery of Precision Instrumentation**
Beyond simulation, I am a builder. I have extensive hands-on experience constructing complex optical systems from scratch. I built **Optical Coherence Tomography (OCT)** systems for analyzing tumor spheroids, developing the entire operation OS to synchronize scanning mirrors and digitizers. I also set up **Light Sheet Fluorescence Microscopy (LSFM)** and **Optical Diffraction Tomography (ODT)** systems, handling everything from optical alignment to the coding of control software.

**Integrating Innovation into Systems**
I didn't just build standard systems; I upgraded them. I integrated **Binary Phase Filters (BPF)** into LSFM to image thicker biological samples (`ryu2020light`) and into OCT systems for inspecting transparent composite films (`US 11,846,587`). This ability to hybridize novel optical elements with established imaging systems allows me to create unique instruments tailored for specific scientific or industrial needs.

**Relevant Publications & Patents:**
*   `ryu2020light`: **LSFM Using Axis-Symmetric Binary Phase Filters** (Biomedical Optics Express)
*   `US 11,846,587 B2`: Tomography Imaging System for Transparent Material Composite Thin Film (Patent Granted)
*   `han2025dual`: Dual-Parameter Tomographic Imaging... in Tumor Spheroids (Theranostics)
*   `yun2025oblique`: Oblique LSFM with Surface Tracking (IEEE TMI)
*   `song2023polarization`: Polarization-Sensitive Intensity Diffraction Tomography (Light: Science & Applications)

<br>

### 3. Computational Metrology & Optimization

**Mathematical Solutions to Optical Problems**
I bridge the gap between optical engineering and mathematical optimization. I applied **Topology Optimization**—typically used in structural mechanics—to Fourier optics, creating non-intuitive phase filter designs that mathematically guarantee optimal depth extension. In industrial applications, I used **Particle Swarm Optimization (PSO)** to find the best phase mask configurations for 3D profilometry, directly solving trade-offs faced by manufacturing inspection systems.

**Relevant Publications & Patents:**
*   `roper2020topology`: **Topology Optimization Implementation for DoF Extension** (Structural and Multidisciplinary Optimization)
*   `han2020direct`: Direct Replication of Micro FZP (Optics Express)

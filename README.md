<h1 align="center">Hi, I'm Kaustubh Dhananjay Das 👋</h1>

<p align="center">
  M.E. Computer Science @ BITS Pilani Goa &nbsp;·&nbsp; Graduating 2027 &nbsp;·&nbsp; CGPA 8.44<br>
  Ex-SDE @ Accenture &nbsp;·&nbsp; Teaching Assistant: Operating Systems &nbsp;·&nbsp; Systems Researcher
</p>

---

## 🔬 Research & Projects

### Accelerating DNN Hardware Mapping with Q-Learning Augmented Genetic Algorithm (GAMMA)
*Systems | Computer Architecture — Dec 2025 – Present*

- Extended GAMMA's genetic-algorithm search for configurable spatial DNN-accelerator hardware mapping (parametric PE array, on-chip L1/L2 buffers, NoC bandwidth) with a Q-learning-gated evaluation filter that learns to skip low-quality genome candidates before expensive MAESTRO cost-model calls
- Designed the filter to preserve genetic algorithm's elitism guarantee: protects elite individuals from being skipped, tracks infeasibility separately, self-calibrates skip threshold relative to best reward per run
- Validated with seeded A/B experiments across 12 named CNN backbones (ResNet18, ResNet50, VGG16, MobileNetV2, SqueezeNet, AlexNet, GoogLeNet, DenseNet, Wide-ResNet50, ResNeXt50, ShuffleNetV2, MNASNet) — matched or beat no-filter baseline in 21/30 (70%) while cutting MAESTRO cost-model calls by ~10% per search (~2,500 candidate mappings evaluated per run)
- [github.com/Kaustubh504/Gamma_frequency](https://github.com/Kaustubh504/Gamma_frequency)

### PintOS — Priority Scheduler with Donation
*Operating Systems — Aug 2025 – Oct 2025 · [github.com/Kaustubh504/Priority_scheduluer](https://github.com/Kaustubh504/Priority_scheduluer)*

- Implemented preemptive priority scheduling with transitive priority donation to eliminate priority inversion in kernel scheduling, verified against PintOS's official test suite (17/17 passing)
- Designed priority donation to correctly handle nested/chained lock dependencies, with interrupt-disabled critical sections and priority-ordered wake logic for locks and semaphores to prevent race conditions
- Built a custom benchmarking harness and reduced priority-inversion wait latency by 34.5%, achieved CPU-time fairness within 2% across equal-priority threads, and improved CPU idle-capacity recovery from 0% to 94%

### Raft Leader Election
*Distributed Systems — Oct 2025 – Nov 2025 · [GitHub Link]()*

- Implemented the leader-election subset of the Raft consensus algorithm from scratch in C++17, coordinating a 5-node cluster
- Designed randomized election timeouts and majority-quorum voting to guarantee at most one leader per term, with term numbers acting as a logical clock that demotes stale leaders after network partitions
- Built a concurrent per-node runtime election-timer thread, per-connection RPC server, and concurrent vote/heartbeat fan-out to all peers synchronized via mutex-guarded term/role/vote state, plus a live HTTP status endpoint and browser dashboard for real-time cluster visualization
- Measured leader-failover recovery across 30 independent trials via automated benchmark harness: 100% successful automatic recovery, median re-election latency of 1.8s, consistent with configured 1.5–3s randomized timeout window

---

## 💼 Work Experience

**Packaged App Development Associate — Accenture** *(Sep 2023 – Aug 2025)*
- Actively contributed across all SDLC phases with strong emphasis on testing: test planning, writing test cases, executing regression suites, defect tracking, and post-deployment validation
- Maintained a clean and organized test codebase using Git, managing test scripts and automation frameworks to facilitate team collaboration
- Collaborated with cross-functional teams (QA, Product Owners, DevOps) to define acceptance criteria and ensure delivery of high-quality solutions; mentored new team members on testing best practices

---

## 🎓 Education & Academics

**M.E. Computer Science** — BITS Pilani Goa *(2027)* | CGPA: 8.44  
**B.E. Computer Engineering** — Pimpri Chinchwad College of Engineering, Ravet *(2023)* | CGPA: 9.29

**Coursework:** Operating System, Computer Architecture, Computer Networks, Compiler Design, Algorithms, Database Management System, Theory of Computations

---

## 👨‍🏫 Teaching & Leadership

**Teaching Assistant — Operating Systems Course, BITS Pilani Goa** *(Aug 2025 – Dec 2025)*
- Reviewed student OS lab assignments and provided technical feedback on scheduling, synchronization, and kernel design principles

**Member — ASCII BITS Goa** *(Aug 2025 – Present)*
- Serve as liaison between department and computer science student community

---

## 🧰 Tech Stack

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=java&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=flat-square&logo=cmake&logoColor=white)
![GDB](https://img.shields.io/badge/GDB-4B8BBE?style=flat-square&logoColor=white)

**Domains:** Systems Optimization · Operating Systems · Kernel Development · Real-time Scheduling · Distributed Consensus · Hardware-Software Co-design · Computer Architecture · Genetic Algorithms · Data Structures

---

📧 **h20250119@goa.bits-pilani.ac.in** &nbsp;·&nbsp; 📱 8275722190

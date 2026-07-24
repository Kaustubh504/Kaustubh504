<h1 align="center">Hi, I'm Kaustubh Dhananjay Das 👋</h1>

<p align="center">
  M.E. Computer Science @ BITS Pilani Goa &nbsp;·&nbsp; Graduating 2027 &nbsp;·&nbsp; CGPA 8.5<br>
  Ex-SDE @ Accenture &nbsp;·&nbsp; TA: Compiler Construction &nbsp;·&nbsp; ML Systems Researcher
</p>


---

## 🔬 Research

### Accelerating DNN Hardware Mapping with Q-Learning Augmented GAMMA
*Machine Learning Systems | Computer Architecture — Dec 2025 – Present*

- Extended GAMMA with a **Q-Learning filter** to skip low-quality genome candidates during genetic search, reducing expensive MAESTRO cost model calls by up to **59% (ALBERT)** across 18 DNN architectures
- Designed four-phase Q-tables (eval/crossover/growth/aging) with µ-greedy exploration and **guided mutation** that protects learned high-quality loop-order structures
- Implemented **per-model auto-threshold calibration** from Gen-1 reward statistics, fixing NLP model incompatibility where reward ranges differ 100× from CNN baselines (BERT, ALBERT, T5)
- Ran 450-experiment ablation sweep: **16.9% avg CPU reduction** overall, **45.8% for NLP models**, with 89% of models maintaining or improving solution quality

---

## 🛠 Projects

### Multilingual NER using mBERT + LoRA Fine-Tuning
*Natural Language Processing — Dec 2025 – Apr 2026*

- Fine-tuned mBERT on WikiANN (EN/HI/MR) using LoRA, training only **0.33% of 177M parameters**, achieving F1: **0.819 / 0.844 / 0.814**
- Designed **Partial Layer Freezing** (bottom 6/12 layers frozen) → +2.1% EN, +4.3% HI, +6.4% MR over LoRA baseline
- Zero-shot transfer to unseen Spanish: F1 = **0.811 vs 0.733** (English-only), confirming cross-lingual generalization

### Kernel Scheduler & Synchronization Development — PintOS
*Operating Systems — Jul 2026 – Present · [github.com/Kaustubh504/Priority_scheduluer](https://github.com/Kaustubh504/Priority_scheduluer)*

- Replaced PintOS's default round-robin scheduler with a **priority-based scheduler**: sorted ready queue via `list_insert_ordered`, immediate preemption when a higher-priority thread becomes ready or the running thread's priority drops below what's waiting
- Implemented **priority donation** to eliminate priority inversion, including transitive donation across nested/chained lock dependencies and correct reversion to the next-highest remaining donation (not straight to base) on lock release
- Ensured thread-safe execution via interrupt-disabled critical sections, locks, and semaphores — including fixing semaphore wake order to release the highest-priority waiter instead of FIFO
- Built a custom benchmark harness with measured results: **34.5% reduction** in priority-inversion wait latency (55→36 ticks) via donation, CPU-time fairness within **2%** across equal-priority threads, and **0%→94%** idle-capacity recovery by replacing a busy-wait timer implementation with proper blocking
- Verified against PintOS's official test suite: 17/17 tests passing with exact assertion-level output matches

---

## 💼 Work Experience

**Packaged App Development Associate — Accenture** *(Sep 2023 – Aug 2025)*
- Contributed across all SDLC phases with focus on testing: test planning, regression suites, defect tracking, post-deployment validation
- Maintained automation frameworks via Git; mentored new team members on testing best practices
- Collaborated with QA, Product Owners, and DevOps to define acceptance criteria and ensure quality delivery

---

## 🧰 Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

**Domains:** ML Systems · Natural Language Processing · DBMS · Kernel Dev · Computer Networks · Compiler Design · Genetic Algorithms · Q-Learning · LoRA · Computer Architecture · Theory of Computation

---

📫 **daskaustubh504@gmail.com** &nbsp;·&nbsp; 📱 9284499227

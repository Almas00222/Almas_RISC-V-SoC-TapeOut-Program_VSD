# 🖥️ RISC-V Reference SoC Tapeout Program VSD
<div align="center">

[![RISC-V](https://img.shields.io/badge/RISC--V-SoC%20Tapeout-blue?style=for-the-badge&logo=riscv)](https://riscv.org/)
[![VSD](https://img.shields.io/badge/VSD-Program-orange?style=for-the-badge)](https://vsdiat.vlsisystemdesign.com/)
![Participants](https://img.shields.io/badge/Participants-3500+-success?style=for-the-badge)
![India](https://img.shields.io/badge/Made%20in-India-saffron?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHJlY3Qgd2lkdGg9IjI0IiBoZWlnaHQ9IjgiIGZpbGw9IiNGRjk5MzMiLz4KPHJlY3QgeT0iOCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjgiIGZpbGw9IiNGRkZGRkYiLz4KPHJlY3QgeT0iMTYiIHdpZHRoPSIyNCIgaGVpZ2h0PSI4IiBmaWxsPSIjMTM4ODA4Ii8+Cjwvc3ZnPgo=)

</div>

---

## 📖 About This Repository

**My Learning Portfolio** — A comprehensive chronicle of my experience in the **VSD SoC Tapeout Initiative**!  

This documentation captures my **incremental learning milestones**, organized by weekly modules with detailed task breakdowns.  

> *This intensive training program guides participants through the complete chip design lifecycle—from behavioral HDL coding to final GDSII layout generation—leveraging entirely open-source toolchains. As a contributor to India's most ambitious collaborative RISC-V silicon project, I join 3500+ engineers collectively advancing our nation's semiconductor self-reliance.*

---

## 🗓️ Week 0 — Environment Configuration

| Assignment | Details | Completion |
|------------|---------|------------|
| [**Assignment 0**](Week0/README.md) | 🔧 [EDA Toolchain Setup](Week0/README.md) — Successfully configured **Icarus Verilog**, **Yosys Synthesizer**, and **GTKWave Viewer** | ✅ Completed |

---

### 💡 Week 0 Insights
- Successfully deployed and validated **open-source digital design tools** on my development system.  
- Acquired foundational knowledge of **workspace configuration** essential for RTL development workflows.  
- Established a ready-to-use environment for subsequent **register-transfer to layout** transformation exercises.

---

## 🗓️ Week 1 — Logic Synthesis & Post-Synthesis Validation

| Assignment | Details | Completion |
|------------|---------|------------|
| [**Assignment 1**](Week1/README.md#-task-1--rtl-synthesis-mux-example) | ⚙️ Multiplexer synthesis via Yosys, SkyWater 130nm library mapping, post-synthesis netlist extraction | ✅ Completed |
| [**Assignment 2**](Week1/README.md#-task-2--constant-dff-mapping--gls) | 🎯 Flip-flop constant optimization (`const4.v`, `const5.v`) with gate-level simulation cross-check | ✅ Completed |
| [**Assignment 3**](Week1/README.md#-task-3--mux-using-for-generate) | 🔄 Parameterized MUX design using `for-generate`, behavioral vs gate-level equivalence verification | ✅ Completed |
| [**Assignment 4**](Week1/README.md#-task-4--demux-using-generate) | 🔀 Demultiplexer implementation via `generate` construct, RTL-to-GLS correlation analysis | ✅ Completed |
| [**Assignment 5**](Week1/README.md#-task-5--ripple-carry-adder-rca) | ➕ Full Adder chain (RCA) synthesis pipeline & post-synthesis functional validation | ✅ Completed |

---

### 💡 Week 1 Insights

* Mastered the **Yosys synthesis workflow**, including RTL elaboration, technology mapping, and netlist export.
* Performed rigorous **behavioral vs structural** simulations to ensure logic equivalence post-synthesis.
* Utilized **ABC optimization** algorithms and validated designs using **Icarus Verilog + GTKWave** debug flows.
* [**Critical Debug:**](Week1/README.md#-task-3--mux-using-for-generate) Resolved synthesis-simulation mismatch by correctly instantiating SkyWater primitives for gate-level testbenches.
* [**Practical Application:**](Week1/project.md) Designed and validated a **Moving Average Filter** in Verilog, synthesized using Yosys, and verified through comprehensive GLS.
* [**Next Steps:**](Week1/project.md##-Future-Work) Scale filter architectures to higher tap counts and prototype on FPGA for real-time DSP applications.

---

## 🗓️ Week 2 — System-on-Chip Architecture Foundations

| Assignment | Details | Completion |
|------------|---------|------------|
| [**Assignment 1**](Week2/README.md#-fundamentals-of-system-on-chip-soc-design) | 📚 Technical documentation on SoC architectural principles | ✅ Completed |
| [**Assignment 2**](Week2/README.md#-vsdbabysoc--a-tiny-but-powerful-risc-v-soc) | 🧩 VSDBabySoC integration analysis | ✅ Completed |
| [**Assignment 3**](Week2/README.md#-the-instruction-program-driving-babysoc) | 🧠 In-depth study of RVMYTH processor core architecture | ✅ Completed |
| [**Assignment 4**](Week2/README.md#-pre_synth_sim-waveform) | 📊 Pre-synthesis waveform generation, analysis & technical interpretation | ✅ Completed |

---

### 💡 Week 2 Insights  

* Developed a thorough conceptual understanding of **SoC design paradigms** including processor cores, memory hierarchies, on-chip buses, and peripheral integration.  
* Explored the **BabySoC educational platform** as a hands-on vehicle for understanding system-level design and validated its operation via **Icarus Verilog simulation + GTKWave analysis**.
* [**Planned Enhancements:**](Week2/README.md#-future-work) Incorporate instruction memory subsystem to enable dynamic program loading; develop toolchain for compiling C programs into memory-loadable hex files for CPU execution.  

---

## Credits & Acknowledgments  

I extend my sincere gratitude to [**Kunal Ghosh**](https://github.com/kunalg123) and the entire **[VSD (VLSI System Design)](https://vsdiat.vlsisystemdesign.com/)** team for providing this invaluable learning opportunity through the **RISC-V SoC Tapeout Initiative**.  

I also recognize the contributions of **RISC-V International**, the **India Semiconductor Mission (ISM)**, **VLSI Society of India (VSI)**, and [**Efabless Corporation**](https://github.com/efabless) whose support has made this program achievable.  

---

## 📊 **Learning Progress Dashboard**

[![Module 0](https://img.shields.io/badge/Module%200-Toolchain%20Setup-success?style=flat-square)](Week0)
[![Module 1](https://img.shields.io/badge/Module%201-Synthesis%20%26%20GLS-success?style=flat-square)](Week1/README.md)
[![Module 2](https://img.shields.io/badge/Module%202-SoC%20Architecture-success?style=flat-square)](Week2/README.md)
![Module 3](https://img.shields.io/badge/Module%203-In%20Progress-yellow?style=flat-square)

---

**🔗 External Resources:**

[![VSD Portal](https://img.shields.io/badge/VSD-Training%20Portal-blue?style=flat-square)](https://vsdiat.vlsisystemdesign.com/)
[![RISC-V Org](https://img.shields.io/badge/RISC--V-Foundation-green?style=flat-square)](https://riscv.org/)
[![Efabless](https://img.shields.io/badge/Efabless-Chipignite-orange?style=flat-square)](https://efabless.com/)

---


# Optimized 8×8 Dadda Multiplier using 4:2 Compressors ⚙️🔢

This project presents the **transistor-level design and simulation of an 8×8 Dadda multiplier** optimized for high-speed and low-power operation using **4:2 compressors**. The design is implemented in **45nm CMOS technology** and verified through **Cadence Virtuoso** simulations.

Developed as part of advanced VLSI coursework at **Purdue University**, this project demonstrates efficiency improvements in terms of **power dissipation, propagation delay**, and **transistor count**.

---

## 📌 Highlights

- ✅ Designed using **static CMOS logic**
- ✅ 3-stage reduction using **4:2 compressors**, full adders, and half adders
- ✅ Implemented using **Cadence Virtuoso**
- ✅ Demonstrated delay: **1.7 ns**, frequency: **500 MHz**
- ✅ Power dissipation as low as **12.35 µW**
- ✅ Transistor count: **2874**

---

## 🧠 Why Dadda Multiplier?

Dadda multipliers are known for:
- Efficient use of adders compared to Wallace tree
- Minimal critical path delay
- Area and power efficiency
- Ideal for **embedded systems** and **low-power applications**

This project leverages those properties and enhances performance with **4:2 compressors**, which optimize the partial product reduction process even further.

---

## 🔧 Architecture Overview

- **Partial Product Generation**: 64 products using AND gates
- **Reduction Stages**:
  - **Stage 1**: 8 compressors, 2 full adders, 2 half adders
  - **Stage 2**: 10 compressors, 1 full adder, 1 half adder
  - **Stage 3**: 13 full adders, 2 half adders
- **Final Stage**: Result generation with minimal delay

🧮 **Total Hardware Elements**:
- 18 Compressors  
- 15 Full Adders  
- 5 Half Adders  
- ➡️ Total: 2874 transistors

---

## 📊 Simulation Results

| Scenario                | Frequency | Delay     | Power Dissipation |
|------------------------|-----------|-----------|-------------------|
| Nominal (8-input)      | 500 MHz   | 1.7 ns    | 12.35 µW          |
| Higher load (11-input) | 500 MHz   | 4.03 ns   | 16.46 µW          |
| Theoretical Estimate   | 500 MHz   | 1.2 ns    | 17.24 µW          |

Simulated in **Cadence Virtuoso** using transient analysis.

---

## 📁 Repository Structure

```
8x8-Dadda-Multiplier/
├── Project_2_report.pdf        # Full report with schematics and waveforms
├── project_ppt.pdf             # Summary presentation slides
├── README.md                   # This file
├── schematics/                 # (optional) Cadence screenshots
└── netlist/                    # (optional) Simulation netlists
```

---

## 🔬 Comparative Analysis

| Multiplier Type | Technology | Power (µW) | Remarks                              |
|-----------------|------------|------------|--------------------------------------|
| Array           | FinFET 10nm| 120        | Simple, large area                   |
| Wallace         | SOI 22nm   | 90         | High-speed, more adders             |
| Dadda (this)    | CMOS 45nm  | **50–12**  | Optimized, fewer stages, low area   |

---

## 📌 Applications

- Digital Signal Processing (DSP)
- Image Processing
- Embedded Systems
- Energy-efficient ASICs
- FPGA-based systems

---

## 👨‍🎓 Author

**Amit Vardhan Suryadevara**  
Department of Electrical Engineering  
Purdue University, Indianapolis  
📧 avsuryad@purdue.edu

---

## 📚 References

1. S. Chanda et al., “An energy efficient 32 bit approximate Dadda multiplier,” IEEE CALCON, 2020.  
2. V. Manu et al., “Low Power and Area Efficient DADDA Multiplier,” 2019.  
3. G. Prithi et al., “Delay and Power Efficient Dadda-Multiplier,” IEEE ICICCS, 2021.

---

## 📷 Visuals

📌 Refer to the report for:
- Dadda Multiplier block architecture  
- 4:2 Compressor and logic schematics  
- Transient waveforms and timing analysis

---

## 📝 License

This project is released for educational and research purposes only. Contact the author for reuse or collaboration.

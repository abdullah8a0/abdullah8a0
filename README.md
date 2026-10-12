### Muhammad Abdullah

M.Eng. student in Computer Science and Engineering at MIT ('27), researching **formal verification of processors** in the MATCHA Lab with Mengjia Yan.
I work where hardware, compilers, and proofs meet: making equivalence checking scale to real out-of-order cores, and making it fast enough to sit inside the design loop.

**Interests:** formal methods for hardware · computer architecture · HW/SW co-design · performance engineering

---

#### Research

- **Compositional verification of out-of-order cores.** Decomposing monolithic proof obligations along RTL module boundaries so whole-core equivalence checks become per-unit ones. Applied to [BOOM](https://github.com/riscv-boom/riscv-boom), it found that mispredicted branches could *commit* when `issueWidth > coreWidth`: a Scala `zip` silently truncated the branch-resolution vector, and dead-code elimination then removed the affected logic during compilation, leaving no trace in the generated netlist. Fix: [riscv-boom#763](https://github.com/riscv-boom/riscv-boom/pull/763).
- **Collapsing Towers for Side-Channel Security.** A staged tower of interpreters in Scala that collapses hardware timing semantics into analyzable C, so Spectre-style leaks fall out of bounded model checking.
  C. Wong, **M. Abdullah**, Y. Yang, M. Yan, A. Chlipala, N. Amin. *PEPM 2025* (short paper).
- **RISC-V TEEs in KVM** (MIT CSAIL, 2022–23). Modified KVM to host trusted execution environments on RISC-V, using PMP to isolate guests from a compromised host.

#### Industry

**Siemens EDA** (2024–25): performance engineering for the SLEC sequential equivalence checking engine. Also built new ordering strategies for CoverCheck that cut SAT calls by 22%, and pruned the engine's parameter space from 3000+ parameters to 250.

#### Projects

- [**one-chan**](https://github.com/abdullah8a0/one-chan): an on-chip neural-network chess analyzer, with move generation and a small TPU in SystemVerilog on an FPGA.
- 1st place, 6.172 Leiserchess tournament (2022) · 2nd place, 6.004 MNIST hardware acceleration · IMO 2020 Honorable Mention

---

[fixpoint.cc](https://fixpoint.cc) · [mabdullah@alum.mit.edu](mailto:mabdullah@alum.mit.edu)

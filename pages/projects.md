---
layout: page
---

#### VAST

I am a code owner and the architect of the [VAST](https://github.com/trailofbits/vast) project. VAST is a versatile library and compiler frontend tailored for the analysis and instrumentation of C/C++ language family. This project provides a foundation for customizable program representation for a broad spectrum of analyses. Leveraging the MLIR infrastructure, VAST provides a toolset to represent C/C++ programs at various stages of the compilation and to transform the representation to the best-fit program abstraction.
The development of this project is undertaken within the R&E Department at Trail of Bits, with funding provided by the DARPA research program known as V-SPELLS.

---

#### Circuitous

[Circuitous](https://github.com/trailofbits/circuitous) comprises a collection of tools and libraries that play a pivotal role in Trail of Bits' involvement in the DARPA SIEVE program, focusing on generating circuits for zero-knowledge proofs of exploits. What sets Circuitous apart is its ability to tailor these circuits to specific binaries. This is achieved by lifting binaries to LLVM and reconstructing instruction decoding through the process of fuzzing. The generated circuits are then lowered to a custom CircIR (an LLVM substrate), with further optimizations applied using an equality saturation-based framework. CircIR is versatile and can produce circuits in various formats, with our preference being Verilog in the context of the SIEVE program.
My primary contributions to this project revolve around optimizations, equality saturation, and the development of benchmarking infrastructure.

---

#### DIVINE

In my research, since 2015, I engage in the development of the verification tool DIVINE. It is a modern, explicit-state model checker. Based on the LLVM toolchain, it can verify programs written in multiple real-world programming languages, including C and C++. The verification core is built on a foundation of high­-per­for­mance algorithms and data structures, scaling all the way from a laptop to a high-end cluster. Discover more on the project [website](https://divine.fi.muni.cz/).

---

#### LART: LLVM Abstraction & Refinement Tool

The results of my Ph.D. research I mainly part of LART: an LLVM instrumentation framework suited for verification tools to integrate techniques like symbolic execution and abstract interpretation techniques.

It is an instrumentation engine that leverages the Clang toolchain to synthesize code that performs abstract execution. To minimize its impact on the original bitcode, LART uses a combination of dataflow, taint, and alias analyses.

It is currently developed as part of [DIVINE](https://divine.fi.muni.cz/).
However, a migration to standalone package is in progress on [github](https://github.com/xlauko/lart).


---

### The Battle for Middle-earth: Reforged

As a fan, I help with the resurrection of an old realtime strategy (The Battle for the Middle-earth). I involve in the development of core game mechanics and engine programming. The project is written on a new unreal engine in C++. Find more about the project on project [website](https://bfmereforged.org/).

---

### DIPOT

A small tool that generates C++ monitors suited for LTL model cheking. It uses [SPOT](https://spot.lrde.epita.fr/) as an underlying library to generate an automata structure. ([github](https://github.com/paradise-fi/dipot))

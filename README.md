# Zero to Kernel Engineer 🔧

> A public, day-by-day documentation of my journey from Software Engineering student to Kernel Engineer —
> covering Core ML, x86-64 Assembly CPU kernels, and CUDA GPU kernels.

**By Muhammad Abdurrehman Bhatti**
`NUTECH — Software Engineering 2024` | `Rawalpindi, Pakistan`

---

## The Goal

Most ML engineers use PyTorch and never think about what happens underneath.

I want to go the other direction.

The plan is to implement machine learning — dot products, matrix multiplication, activation functions, backpropagation — first in **x86-64 assembly with AVX2 SIMD** on the CPU, then as optimized **CUDA kernels** on the GPU.

This is not the easy path. It is the path that builds genuine, deep understanding of how AI systems actually work at the hardware level.

The endgame: **Kernel Engineer** — someone who writes the low-level math that PyTorch, TensorFlow, and every major ML framework secretly depends on.

---

## Why Document This Publicly?

**Writing forces understanding.** If I cannot explain what I learned today in plain language, I have not understood it. The daily log keeps me honest.

**There are almost no public resources showing this exact journey from scratch.** If someone else wants to walk this path, this repo becomes the documentation they needed but could not find.

---

## The Roadmap

| Phase | Focus | Duration | Status |
|-------|-------|----------|--------|
| **Phase 0** | Math Foundations + C Basics | 3–4 months | 🔄 In Progress |
| **Phase 1** | Core ML + NumPy from Scratch | 4–5 months | ⏳ Not Started |
| **Phase 2** | C Deep Dive — Systems Programming | 6–8 weeks | ⏳ Not Started |
| **Phase 3** | x86-64 Assembly + CPU ML Kernels | 4–5 months | ⏳ Not Started |
| **Phase 4** | CUDA C++ + GPU Kernel Engineering | 5–6 months | ⏳ Not Started |

**Total estimated duration:** 18–22 months

---

## Repository Structure

```
zero-to-kernel/
│
├── README.md                    
│
├── daily-log/                   ← written every single day, no exceptions
│   ├── README.md                
│   ├── week-01.md
│   └── ...
│
├── phase-0-math/
│   ├── linear-algebra/
│   │   ├── notes/                ← clean writeup, only once fully understood
│   │   └── numpy-verification/   ← hand-solved problems verified in NumPy
│   ├── calculus/
│   │   ├── notes/
│   │   └── numpy-verification/
│   └── statistics/
│       ├── notes/
│       └── numpy-verification/
│
├── phase-1-ml/
│   ├── notes/
│   ├── numpy-from-scratch/       ← linear/logistic regression, NN, MNIST — no sklearn/PyTorch
│   ├── pytorch-implementations/
│   └── comparisons/
│
├── phase-2-c/
│   ├── notes/
│   ├── pointers/
│   ├── memory/
│   ├── arrays-and-layout/
│   ├── call-stack/
│   └── inline-assembly/
│
├── phase-3-assembly/             ← flagship phase
│   ├── notes/
│   ├── 01-dot-product/
│   ├── 02-matrix-multiply/
│   ├── 03-activation-functions/
│   ├── 04-single-neuron/
│   ├── 05-feedforward-network/
│   ├── 06-backpropagation/
│   └── 07-mnist-assembly/        ← the main project
│
└── phase-4-cuda/                 ← endgame phase
    ├── notes/
    ├── 01-vector-dot-product/
    ├── 02-matrix-multiply/
    ├── 03-fused-kernels/
    ├── 04-softmax/
    ├── 05-layernorm/
    ├── 06-flash-attention/
    └── 07-pytorch-integration/
```

**`daily-log/`** — process. Written the same day, every day. What I studied, what I understood, what confused me. Messy and honest is fine here.

**`notes/`** (inside each phase) — reference. Written only once a topic is fully understood. The clean, distilled explanation I'd re-read before building something that depends on it.

---

## Phase Breakdown

### Phase 0 — Math & C Foundations
Linear Algebra, Calculus, Statistics & Probability, C Programming Basics.

**Primary Resources:** 3Blue1Brown (Essence of Linear Algebra / Calculus), Gilbert Strang — *Introduction to Linear Algebra* + MIT 18.06SC, MIT 18.065 (Matrix Methods for ML), StatQuest, CS50x, *The C Programming Language* — Kernighan & Ritchie.

---

### Phase 1 — Core Machine Learning
Linear/logistic regression, neural networks, backpropagation, optimizers, regularization — theory first, then built from scratch in NumPy, then PyTorch.

**Primary Resources:** Andrew Ng — ML Specialization, Andrej Karpathy — Neural Networks: Zero to Hero, *Hands-On ML* — Aurélien Géron (3rd ed.), *Deep Learning* — Goodfellow, Bengio, Courville.

**Milestone:** Train a neural network on MNIST to >95% accuracy using only NumPy.

---

### Phase 2 — C Deep Dive
Pointers, stack vs heap, memory alignment, row-major vs column-major layout, calling conventions, the compilation pipeline, inline assembly.

**Primary Resources:** *Computer Systems: A Programmer's Perspective* — Bryant & O'Hallaron, Ulrich Drepper — *What Every Programmer Should Know About Memory*.

---

### Phase 3 — x86-64 Assembly + CPU ML Kernels ⭐
Registers, core instructions, the stack, SSE/AVX2 SIMD, FMA, cache optimization, the roofline model.

**Primary Resources:** Kip Irvine — *Assembly Language for x86 Processors*, Ray Seyfarth — *Introduction to 64-Bit Assembly Language*, CS:APP Ch. 3, Agner Fog — *Optimizing Subroutines in Assembly*, Intel Intrinsics Guide.

**Projects:** dot product → matrix multiply → activation functions → single neuron → feedforward network → backpropagation → **MNIST trained entirely with assembly kernels**.

---

### Phase 4 — CUDA C++ + GPU Kernel Engineering 🚀
GPU architecture, thread hierarchy, memory coalescing, shared memory tiling, occupancy, Tensor Cores, profiling.

**Hardware:** NVIDIA GTX 1660 Super — Turing, Compute Capability 7.5, 6GB GDDR6.

**Primary Resources:** Kirk & Hwu — *Programming Massively Parallel Processors*, NVIDIA CUDA C++ Programming Guide, Simon Boehm — *How to Optimize a CUDA Matmul Kernel*.

**Projects:** vector add/dot product → matrix multiply (naive → tiled → register-blocked) → fused kernels → softmax → layernorm → simplified Flash Attention → custom PyTorch operator.

---

## The Most Important Insight

When you write this in Python:

```python
output = torch.matmul(A, B)
```

What actually runs:

```
Python → C++ (LibTorch) → cuBLAS CUDA kernel → GPU assembly (SASS)
```

Most engineers only ever see the Python. I am building the bottom layers.

---

## Connect

`GitHub:` AbdurRehman-debug

---

*Started August 22 2026 . Updated daily.*

*Streak: 3*

> "The engineers who reach this level are not the smartest.
> They are the ones who showed up every day for two years."

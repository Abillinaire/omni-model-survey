<p align="center">
  <img src="https://img.shields.io/badge/Status-Writing%20in%20Progress-yellow?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/Pages-9%2B-blue?style=for-the-badge" alt="Pages">
  <img src="https://img.shields.io/badge/References-50%2B-brightgreen?style=for-the-badge" alt="References">
  <img src="https://img.shields.io/badge/Taxonomy-Build%20%E2%86%92%20Assess%20%E2%86%92%20Apply-purple?style=for-the-badge" alt="Taxonomy">
</p>

<h1 align="center">
  🌐 Omni-Modal Large Language Models
</h1>
<h3 align="center">
  <i>A Comprehensive Survey on Architecture, Training, and Evaluation</i>
</h3>

<p align="center">
  <b>Last Updated:</b> June 2026
</p>

---

## 📖 TL;DR

> **The first comprehensive survey of omni-modal LLMs organized around a *full-lifecycle* taxonomy — Build → Assess → Apply — spanning 6 dimensions, 50+ papers, from GPT-4o and Gemini to Qwen3.5-Omni and ByteDance Seed's Context Unrolling.**

---

## 🧭 Taxonomy: Build → Assess → Apply

```
┌─────────────────────────────────────────────────────────┐
│                 OMNI-MODAL LLM LIFECYCLE                │
├──────────────┬──────────────────┬───────────────────────┤
│    BUILD     │     ASSESS       │       APPLY           │
│  How to      │  What can it do? │  Where does it act?   │
│  construct?  │  Is it safe?     │                       │
├──────────────┼──────────────────┼───────────────────────┤
│              │                  │                       │
│ 🏗️ ARCH     │ 🎯 CAPABILITIES  │ 🤖 AGENTS            │
│ Tokenization │ Cross-modal      │ Agentic perception    │
│ Encoders     │ Any-to-any gen   │ World models          │
│ Fusion       │ Real-time inter. │ Embodied AI           │
│ Generation   │                  │                       │
│ System-level │ 📏 EVALUATION    │                       │
│              │ Benchmarks       │                       │
│ 🏋️ TRAINING │ Omni-specific    │                       │
│ Pre-training │ Comprehensive    │                       │
│ Alignment    │                  │                       │
│ Efficient    │ 🛡️ SAFETY       │                       │
│ Post-train   │ Jailbreak        │                       │
│              │ Guardrails       │                       │
│              │ Cross-modal      │                       │
└──────────────┴──────────────────┴───────────────────────┘
               ↑                                    ↑
          📊 DATASETS & RESOURCES (cross-cutting)   │
                                                    │
          🚀 CHALLENGES & FUTURE DIRECTIONS ─────────┘
```

---

## 📑 Paper Structure

| # | Section | Status | Highlights |
|---|---------|--------|------------|
| 1 | **Introduction** | ✅ | Full-lifecycle taxonomy, 4 contribution bullets, gap analysis vs. 6 prior surveys |
| 2 | **Background** | ✅ | Evolutionary timeline, key definitions, survey comparison matrix |
| 3 | **Taxonomy** | ✅ | Build → Assess → Apply framework (core intellectual contribution) |
| 4 | **Architecture** | ✅ | 5 subsections: Tokenization, Encoders/Decoders, Fusion (4 paradigms), Generation, System-level |
| 5 | **Training** | ✅ | 4 subsections: Pre-training, Alignment, Efficient Training, Post-training (RL collapse, PID) |
| 6 | **Capabilities** | ✅ | 3 subsections: Cross-modal Understanding, Any-to-Any Generation, Real-Time Interaction |
| 7 | **Evaluation** | 🔨 | Understanding & generation benchmarks, omni-specific evaluation |
| 8 | **Safety & Alignment** | 🔨 | Multimodal jailbreak, guardrails, cross-modal value alignment |
| 9 | **Omni-Modal Agents** | 🔨 | Agentic perception, world models, embodied AI |
| 10 | **Datasets & Resources** | 🔨 | Training corpora, benchmark catalog, open-source models |
| 11 | **Challenges & Future** | 🔨 | 10 open problems with actionable research directions |
| 12 | **Conclusion** | 🔨 | Synthesis and outlook |

---

## 🌟 Key Contributions

### 1. Novel Taxonomy
**First full-lifecycle framework** for omni-modal LLMs. Unlike prior surveys that classify by model components (encoders, LLM backbone, etc.), we organize the field by the questions researchers actually face: *How to build? How to assess? How to deploy?*

### 2. Comprehensive Coverage
**50+ papers** systematically reviewed across **6 dimensions**, capturing the latest developments through **mid-2026**:

| Dimension | Exemplar Papers |
|-----------|----------------|
| **Core Models** | GPT-4o, Gemini 2.0/2.5, Qwen3.5-Omni, Seed Omni, Chameleon, Cosmos 3 |
| **Architecture** | MorphoQuant, OmniDrop, Stage-adaptive Token Selection, LatentOmni, FlowInOne |
| **Training** | Staged Post-training, Entrain, SMA, OmniTrace, PID, Modality Collapse |
| **Capabilities** | DuplexOmni, Foley-Omni, Omni-Customizer, VideoWeaver, StreamOV |
| **Safety** | GuardReasoner-Omni, Cross-modal Jailbreak Analysis, Precise Shield |
| **Agents** | OSCAR, Sandboxed Coding Agents, Cosmos Policy, Omni-WorldBench |

### 3. Structured Comparison Tables
Every section includes comparison tables that enable researchers to:
- Quickly situate new work within the broader landscape
- Identify under-explored research directions
- Understand tradeoffs between architectural paradigms

### 4. 10 Open Challenges
Each challenge comes with **concrete, actionable research directions** — not vague hand-waving. Topics include unified architectures, modality imbalance in training, immature evaluation benchmarks, cross-modal safety, and more.

---

## 🔬 Featured Papers We Survey

<details>
<summary><b>Click to expand — 50+ papers organized by taxonomy dimension</b></summary>

### 🏗️ Architecture
| Paper | Key Idea |
|-------|----------|
| Qwen3.5-Omni (2026) | Hybrid Attention MoE, ARIA alignment, 256K context |
| Seed Omni: Context Unrolling (2026) | Cross-modal reasoning across 5+ modalities |
| Chameleon (2024) | Early-fusion with unified discrete tokenization |
| MorphoQuant (2026) | Modality-aware 4-bit quantization for omni LLMs |
| OmniDrop (2026) | Layer-wise token pruning via query guidance |
| Stage-adaptive Token Selection (2026) | Dynamic token budgets across processing stages |
| LatentOmni (2026) | Unified audio-visual latent reasoning |
| Conan-embedding-v3 (2026) | Fusing modality-specific models for omni embeddings |
| FlowInOne (2026) | Unified generation as image-in, image-out flow matching |
| Dynin-Omni (2026) | Omnimodal unified diffusion language model |
| StreamOV (2026) | Streaming omni-video via evidence-guided memory |
| O-MARC (2026) | Memory-augmented compression distillation for video |

### 🏋️ Training
| Paper | Key Idea |
|-------|----------|
| Staged Post-Training (2026) | Visually debiased multi-stage post-training |
| Escape the Language Prior (2026) | Modality-aware policy optimization vs. GRPO collapse |
| Entrain (2026) | Distributed training with modality-aware load balancing |
| PID for Modality Interaction (2026) | Decomposing unique/redundant/synergistic modality contributions |
| OmniTrace (2026) | Generation-time attribution across modalities |
| SMA (2026) | Submodular Modality Aligner for data-efficient training |

### 🎯 Capabilities
| Paper | Key Idea |
|-------|----------|
| DuplexOmni (2026) | Real-time full-duplex multimodal interaction |
| Foley-Omni (2026) | Unified audio synthesis to video soundtrack generation |
| Omni-Customizer (2026) | Multimodal customization for joint A/V generation |
| VideoWeaver (2026) | Agentic long video generation with evolving skills |
| Inference-Time Scaling for A/V (2026) | Training-free quality improvement for joint generation |
| OmniCap-IF (2026) | Instruction-following for omni-video captioning |

### 📏 Evaluation
| Paper | Key Idea |
|-------|----------|
| AVI-Bench (2026) | Human-like audio-visual intelligence benchmark |
| OmniPro (2026) | Proactive streaming video understanding |
| Omni-DuplexEval (2026) | Real-time duplex interaction evaluation |
| TOBench (2026) | Task-oriented omni-modal tool-use benchmark |
| VideoOdyssey (2026) | Ultra-long-context omni video understanding |

### 🛡️ Safety
| Paper | Key Idea |
|-------|----------|
| GuardReasoner-Omni (2026) | Reasoning-based guardrails for all modalities |
| Cross-modal Jailbreak (2026) | Modality-dependent attack surface analysis |
| Sparse Token Jailbreak (2026) | Gradient-optimized audio LM attacks |
| OMNI-LEAK (2026) | Multi-agent data leakage in omni systems |

### 🤖 Agents & World Models
| Paper | Key Idea |
|-------|----------|
| Cosmos 3 (2026) | NVIDIA omnimodal world model for physical AI |
| OSCAR (2026) | Omni-embodiment action-conditioned world model |
| Sandboxed Coding Agents (2026) | Coding agents as competitive omni task solvers |
| Agentic Active Omni Perception (2026) | Multi-hop audio-visual reasoning |
| Omni-WorldBench (2026) | Interaction-centric world model evaluation |

</details>

---

## 📝 Citation

```bibtex
@article{anonymous2026omnisurvey,
  title   = {Omni-Modal Large Language Models: A Comprehensive Survey on Architecture, Training, and Evaluation},
  author  = {Anonymous},
  journal = {arXiv preprint},
  year    = {2026},
  note    = {Work in progress}
}
```

---

## 🙏 Acknowledgments

This survey builds upon the excellent foundation laid by prior surveys, particularly *From Specific-MLLMs to Omni-MLLMs* (Song et al., 2024). We thank the authors of all surveyed papers for advancing the field.

Writing was assisted by Claude Code with [ml-paper-writing](https://github.com/orchestra-research/AI-research-SKILLs) and [research-paper-writing](https://github.com/Master-cai/Research-Paper-Writing-Skills) skills.

---

<p align="center">
  <sub>Built with ❤️ and LaTeX | ICML 2026 Template | Work in Progress</sub>
</p>

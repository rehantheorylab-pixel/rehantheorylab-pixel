# Rehan Muhammad

**Independent Researcher · Systems, Algorithms, AI Agents**

I build low-level systems and the infrastructure that lets AI agents operate real computers:
exact algorithms for NP-complete problems, kernel-level memory management, and browser/desktop
bridges for agent runtimes.

**Rehan Theory Lab** · rehan@rehantheorylab.com

---

## Projects

### [Z++ — exact subset-sum solver](https://github.com/rehantheorylab-pixel/zpp-subset-sum-solver)
![Rust](https://img.shields.io/badge/Rust-DEA584?style=flat-square&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)

A solver that **races published algorithms against original engines** and reports which engine
won on each problem — Schroeppel–Shamir, meet-in-the-middle, BCJ and others running as
baselines, with original GDEP, adaptive core-aware partitioning, and arbitrary-precision
paths competing against them.

- 49 engines; original engines take the majority of the 65-category suite
- Measured n=60 in 524 s on an i3-2100 → **1,649×** vs BCJ's published 864,000 s
- Documented memory floor: ~12 GB at n=60
- Reproducible: `python tests/test_zpp.py`

### [browser-bridge-for-muse](https://github.com/rehantheorylab-pixel/browser-bridge-for-muse)
Unofficial bridge giving an AI agent **consent-based** access to a user's own browser and
desktop. Multi-engine routing (real Chrome profile, CDP, patched driver), session handoff,
MCP server. *Not affiliated with Meta.*

### [MAIK — Multi-Agent Intelligence Kernel](https://github.com/rehantheorylab-pixel/maik)
Agent org chart with specialized routing, self-grading runs, and reproducible benchmarks.
CEO → manager → agent → sub-agent hierarchy with per-node resolved prompts.

### [ZPP Unix](https://github.com/rehantheorylab-pixel/zpp_unix)
Extended the [caffeinix](https://github.com/TroyMitchell911/caffeinix) RISC-V kernel (GPL-3.0)
with a lock-free allocator, arena allocator, and slab allocator.

---

## Focus

`systems programming` · `exact algorithms` · `memory allocators` · `RISC-V` ·
`agent infrastructure` · `browser automation` · `computer use`

## Elsewhere

[ORCID](https://orcid.org/0009-0003-8748-6524) · [Zenodo](https://doi.org/10.5281/zenodo.20399806) · [HuggingFace](https://huggingface.co/12rehdsa)

## Contact

Open to remote contracts in systems programming and agent infrastructure.
**rehan@rehantheorylab.com**

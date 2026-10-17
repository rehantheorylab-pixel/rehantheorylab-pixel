<div align="center">

<img src="assets/hero.svg" alt="Rehan Muhammad — Independent Researcher" width="100%">

<br>

<a href="https://github.com/rehantheorylab-pixel/zpp-subset-sum-solver">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=17&duration=3400&pause=800&color=58A6FF&center=true&vCenter=true&width=820&lines=exact+algorithms+%E2%80%94+49+engines%2C+one+winner;systems+programming+%E2%80%94+allocators%2C+page+tables%2C+RISC-V;agent+infrastructure+%E2%80%94+consent-based+machine+access" alt="exact algorithms — systems programming — agent infrastructure">
</a>

<br><br>

[![Z++](https://img.shields.io/badge/Z%2B%2B-exact_subset_sum-1f6feb?style=for-the-badge&logo=rust&logoColor=white)](https://github.com/rehantheorylab-pixel/zpp-subset-sum-solver)
[![Bridge](https://img.shields.io/badge/browser_bridge-for_agents-1f6feb?style=for-the-badge&logo=googlechrome&logoColor=white)](https://github.com/rehantheorylab-pixel/browser-bridge-for-muse)
[![MAIK](https://img.shields.io/badge/MAIK-multi--agent_kernel-1f6feb?style=for-the-badge&logo=python&logoColor=white)](https://github.com/rehantheorylab-pixel/maik)

<br>

**Rehan Theory Lab**  ·  [rehan@rehantheorylab.com](mailto:rehan@rehantheorylab.com)  ·  Open to remote contracts

</div>

---

<div align="center">
<img src="assets/race.svg" alt="Animated illustration: several engines racing to solve one problem, the fastest engine wins" width="100%">
</div>

I work on two hard problems at once: making **exact computation faster** — NP-complete search,
kernel-level memory management — and making it **safe for AI agents to operate real machines**,
through bridges with an explicit consent model.

---

## What I'm building

<table>
<tr>
<td width="50%" valign="top">

#### [Z++ — exact subset-sum solver](https://github.com/rehantheorylab-pixel/zpp-subset-sum-solver)

Races **49 engines** against each other — published baselines and original work
competing on the same problem — and reports which one won. You get the answer, plus
the evidence for *why* that class of technique solved that class of instance.

```yaml
baselines:  Schroeppel–Shamir · MITM · BCJ · HGJ · Bonnetain
original:   GDEP · adaptive core-aware partitioning · BigUint
measured:   n=60 → 524 s  (i3-2100)     = 1,649× vs BCJ
projected:  n=60 → 24.3 s (Ryzen 9)     = 35,556×
memory:     ~12 GB floor at n=60
```

</td>
<td width="50%" valign="top">

#### [browser-bridge-for-muse](https://github.com/rehantheorylab-pixel/browser-bridge-for-muse)

Gives an AI agent access to the user's **own** browser and desktop — the sessions they
already have — instead of a sterile browser that hits a login wall on every site.
User-initiated, visible, killable.

```yaml
engines:    Chrome profile · CDP · patched driver
interface:  MCP server
consent:    per-session opt-in, visible, scoped
never:      credential export, silent operation
```

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### [MAIK — Multi-Agent Intelligence Kernel](https://github.com/rehantheorylab-pixel/maik)

An agent system organised as a company: identities, managers, notebooks, scoped
permissions, and prompts generated at runtime from each node's own context. Failures
demote the route that caused them.

```yaml
structure:  CEO → manager → agent → sub-agent
routing:    domain → model, chosen from grades
execution:  mouse, keyboard, screen, browser
status:     research prototype — graders are internal
```

</td>
<td width="50%" valign="top">

#### [ZPP Unix](https://github.com/rehantheorylab-pixel/zpp_unix)

A RISC-V kernel extended with **lock-free, arena, and slab allocators** integrated into
an existing memory subsystem. A fork of caffeinix, credited as such in the first line.

```yaml
upstream:   caffeinix · Troy Mitchell · GPL-3.0
added:      lock_free.c · arena.c · slab.c · palloc.c
scope:      ~390 lines into a ~7,500-line kernel
```

</td>
</tr>
</table>

---

## How I work

> **Measure, then claim.** Every number I publish carries the machine it ran on and whether
> it was measured or projected. A ratio computed from two estimates is labelled an estimate.

> **Credit upstream.** A fork says what it is forked from in the first line. Attribution is a
> licence obligation under GPL, and a credibility requirement under everything else.

> **State the limit.** If it isn't tested, the README says so before the reader finds out.
> Limitations sections are cheaper than retractions.

---

## Currently

- Running the head-to-head my benchmarks currently admit is missing: Z++ against published
  baselines, **same machine, same inputs**
- Measuring **thread-count scaling** on the partitioning design — testing whether it holds
  linear, or better, as core count rises
- Keeping the browser bridge's consent model ahead of its capabilities

---

## Stack

<div align="center">

![Rust](https://img.shields.io/badge/Rust-DEA584?style=flat-square&logo=rust&logoColor=black)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![RISC-V](https://img.shields.io/badge/RISC--V-283272?style=flat-square&logo=riscv&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

`allocators` · `page tables` · `trap handling` · `branch & bound` · `meet-in-the-middle` ·
`CDP` · `MCP` · `Chrome extensions` · `QEMU/gdb`

</div>

---

## Elsewhere

<div align="center">

[![ORCID](https://img.shields.io/badge/ORCID-0009--0003--8748--6524-A6CE39?style=flat-square&logo=orcid&logoColor=white)](https://orcid.org/0009-0003-8748-6524)
[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.20399806-blue?style=flat-square)](https://doi.org/10.5281/zenodo.20399806)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-12rehdsa-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co/12rehdsa)

</div>

---

<div align="center">

**Working on something that needs exact search, kernel work, or agent tooling?**
[rehan@rehantheorylab.com](mailto:rehan@rehantheorylab.com)

<sub><a href="https://github.com/rehantheorylab-pixel">github.com/rehantheorylab-pixel</a></sub>

</div>

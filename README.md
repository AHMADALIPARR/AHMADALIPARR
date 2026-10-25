# Ahmad Ali Parr

**Stop asking who owns the weights. Ask who owns the machine the weights run in.**

I build the machine around the weights: the router, the harness, the ledger, the layer that decides. The weights are the commodity. The machine is the asset.

I'm a builder and reverse engineer working on sovereign compute — systems that run on hardware I own, verified end to end, with every decision recorded like an accounting entry. I used to be a forensic accountant; the hash chains and paper trails in my code come from that craft. I'm part of the SnapKitty Collective, working on sovereign compute architecture.

<img src="images/hologram.jpg" alt="Holographic plate" width="700">

## The machine, in one diagram

This is not decoration. It is the pipeline every proposal in the sovereign-canvas-machine goes through, stage by stage, with the real module each stage names. A failure at any stage is a rejection, not a warning.

```
Canvas record (one typed proposal)
        |
        v
Perl decoder  +  AWK decoder  -- must agree, or DECODER_MISMATCH
        |
        v
ADR seal  -->  Policy: deny by default  -->  Invariant
        |
        v
HyperDAG: canonical XML tree, Merkle DAG, braid anyons
        |
        v
C runtime recomputes the invariant -- must match, or PROOF_MISMATCH
        |
        v
ColorForth ceremony, 9 words in order -- a skipped word rejects
        |
        v
Sealed ledger line (SHA-256 chain) -- ACCEPT: AUTHORIZED
```

The diagram itself is content-addressed. The HyperDAG is a Merkle DAG: every element carries a leaf hash, every section folds its children's hashes, and the root commits to the whole diagram. Here is a real one, from the `braid_valid` fixture (s1 s2 s1, prefixes shown):

```
root        34df6ceb14c3...
  nodes       33191d5e27dd...
  hyperedges  deb85ce7e728...
  continuity  38182f274d2d...
  anyons      042b1b13fc42...
```

Change one attribute anywhere in the tree and the root breaks. That is the point: the diagram is a witness you can check, not a picture you have to trust.

## What I'm building

### Proof-carrying execution — [sovereign-canvas-machine](https://github.com/AHMADALIPARR/sovereign-canvas-machine)

A model may submit one typed canvas record. It does not get a shell, a tool call, or the right to mark its own work verified. Two independent decoders (Perl and AWK) must agree on the record. An ADR seal must match. Policy is deny by default: a missing clause is a denial, and the only obligations the pipeline honors are the ones in its catalog. Equality is decided by real mathematics — the faithful Artin action of the three-strand braid group, Clifford tableaus for quantum circuits, exact integer recomputation for recurrences — never by string comparison. The candidate's diagram is built as a canonical XML Merkle DAG with braid anyons (strands as worldlines, crossings as braiding events), projected to a certificate by a real XSLT stylesheet, and then a second implementation in C must recompute the same invariant. Only then does the nine-word ColorForth ceremony seal a hash-chained ledger line. The core rule, stated once: intent is not authority. Generated code is not executable until it is independently authorized.

### Typed decisions

Clean-room work on typed, auditable machine decisions. A decision should be a typed value with a ledger entry behind it, not a paragraph of free text that nobody can check. No text output means no fluent confabulation to mistake for reasoning: the system proves, refutes, or refuses, and the refusal is a first-class outcome. This is the work family offices have been asking about, and the work I will not sell: the typed-decisions asset stays mine, and what gets funded is the quantum work it points toward.

### Zero-knowledge state machines — [quantum-TQC](https://github.com/AHMADALIPARR/quantum-TQC)

State advances by proven transitions at the gate and certificate layer, not by hand-stepped simulation. The Rust surfaces are shape, witness, and coupling layers; the gate layer enforces the topological constraints and returns verifiable certificates. The design punishes grazing: gaps that look unfinished are load-bearing, and filling them with textbook code breaks the framework's invariants. That is deliberate. A framework that rewards copy-paste completion is a framework that gets completed wrong.

### Reconstruction from public evidence — [operation-tay](https://github.com/AHMADALIPARR/operation-tay)

Tay's weights are gone everywhere I could look — Hugging Face, NuGet, GitHub, the Internet Archive. The framework claim died on dates alone (Tay launched before the framework was announced), and zero Tay turned up across tens of thousands of commits in the window. So I rebuilt her from the public corpus: a working Rust reconstruction with every replacement honestly labeled and the generative slot deliberately left empty. The reconstruction lost nothing without the weights. That proved the thesis: the weights were never the asset. The router, the harness, the training judgment, the layer that decides — that is what survived, because that is what was owned.

### Formal verification across systems

Claims get checked by a kernel, a solver, or a typechecker — Lean, Agda, Alloy, Liquid Haskell, Curry-Howard — never by assertion, and never by theorem counts. Zero sorry where I demand it, with axioms stated plainly instead of hidden inside a count. A WAT file that compiles can still be stubs, so ported code gets verified by executing its exported functions against known vectors, with a per-function verified-versus-stub status. Verification means execution, not compilation.

## Direction

Local first, always. Core inference runs on my own fleet, not on rented APIs, and I pay nothing for APIs. The current direction is quantum: a locally controlled cryogenic superconducting research system — cryogenics the cheap route, not the Google Willow route. Sovereign computing shouldn't stop at the operating system. The machine around the weights, the ledger under the decisions, the proof behind the state change — that is one project, not three, and the quantum machine is where it goes next.

## Stack

C11 · Rust · Lean · Ada · Fortran · Elixir/OTP · APL · Kotlin · Perl · Assembly · CUDA

## Selected public work

- **[sovereign-canvas-machine](https://github.com/AHMADALIPARR/sovereign-canvas-machine)** — proof-carrying mathematical execution. Deny-by-default pipeline, dual decoders, Merkle DAG with braid anyons, XSLT certificate, C cross-check, sealed ledger. The diagram above is this machine.
- **[quantum-TQC](https://github.com/AHMADALIPARR/quantum-TQC)** — zero-knowledge state machine. State advances by proven gate and certificate transitions; the surfaces are witness and coupling layers, not a hand-stepped grid.
- **[operation-tay](https://github.com/AHMADALIPARR/operation-tay)** — Tay reconstruction from the public corpus after her weights were declared unavailable everywhere. Every replacement labeled, the generative slot left empty on purpose.
- **[alpha-omega](https://github.com/AHMADALIPARR/alpha-omega)** — full-stack verified build from a single brief: missing Rust bodies reconstructed from the repo's own contracts and labeled, Lean obligations proven as machine-checked theorems, an Elixir/OTP supervisor over the engine, a Modula-2 kernel agreeing with the Rust to the fixed-point integer, and a solver receipt for the optimization contract.
- **[holographic-memory](https://github.com/AHMADALIPARR/holographic-memory)** — holographic memory, finished and published. Reconstruction work, visualized below.

  <img src="images/bunny.jpg" alt="Holographic bunny reconstruction" width="400">

- **[bifurcation-invariant](https://github.com/AHMADALIPARR/bifurcation-invariant)** — a five-axiom invariant verified across five systems, plus drug-discovery analysis. The invariant, not the visualization, is the contribution.
- **[protein-folding-bifurcation](https://github.com/AHMADALIPARR/protein-folding-bifurcation)** — a zero-axiom model of protein folding plus visualization, at the alpha-helix version. The folding demo:

  <video src="images/folding.mp4" controls width="600"></video>

  [Watch the folding demo](images/folding.mp4)

- **[m2lib](https://github.com/AHMADALIPARR/m2lib)** — machine library work.

Plus hundreds of public repos across two orgs. I build in the open, on purpose.

---

Correctness over hype. Structure over abstraction. Computation with rigor.

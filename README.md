# The Big Unfolding — Vacuum Curvature Simulator

Interactive N-body simulation demonstrating that cosmic web structure emerges naturally from two fundamental forces in tension:

- **Gravity** — attractive, ∝ 1/r² (standard Newton)
- **Vacuum curvature** — repulsive, ∝ r (geometric, from the Newtonian limit of GR with Λ)

## The Claim

The cosmic web (filaments, voids, galaxy clusters) is not a mystery requiring exotic physics. It is the **default equilibrium** of any system with an attractive force that weakens with distance and a repulsive force that strengthens with distance. Structure forms at the crossover scale where these forces balance.

## What You'll See

| Panel | Forces | Result |
|---|---|---|
| **Left (orange)** | Gravity only | Collapse to single blob |
| **Right (magenta)** | Gravity + curvature | Stable cosmic web with filaments, voids, and clusters |

Both panels start with identical initial conditions (Gaussian cluster + Hubble flow velocities). The **only** difference is the curvature force in the right panel.

## Physics Model (v0.04)

- **Pure Newtonian** — no prescribed expansion, no Hubble drag, no mysterious forces
- **H(t) is measured**, not prescribed — expansion rate emerges from particle dynamics
- **Curvature decay**: ε(t) = ε₀/(1 + t/τ)² — matching the Λ ∝ 1/t² scaling from Running Vacuum Models (Özer & Taha 1987, Solà Peracaula 2022)
- **5 physics parameters**: H₀ (initial Hubble flow), Radius₀ (initial cluster size), G (gravity), ε₀ (curvature strength), ε_decay (curvature persistence)

## Versions

| File | Description |
|---|---|
| `vacuum-curvature-sim.html` | v0.01 — Initial prototype with prescribed H(t) |
| `vacuum-curvature-sim-v02.html` | v0.02 — Explicit ε₀/ε_decay parameters |
| `vacuum-curvature-sim-v03.html` | v0.03 — Pure Newtonian rewrite, measured H(t) |
| `vacuum-curvature-sim-v04.html` | v0.04 — Fullscreen mode, 1/t² decay, text inputs, expanded charts |

## Usage

Open any `.html` file directly in a modern browser. No dependencies, no build step. Self-contained.

- **Scroll wheel** on canvases to zoom
- **Click + drag** to pan
- **⛶ Fullscreen** button under each canvas for full-screen viewing
- **Text inputs** accept values outside slider ranges (press Enter to apply)

## Theoretical Foundation

Based on peer-reviewed literature:

- **Padmanabhan (2002)** — Derivation of g_Λ = ⅓Λc²r as the weak-field Newtonian limit
- **Bianchi & Rovelli (2010)** — Λ belongs on the geometric side of the EFE, not as a fluid
- **Solà Peracaula (2022)** — Vacuum density evolves as O(H²), yielding Λ ∝ 1/t²
- **Özer & Taha (1987)** — Λ ∝ a⁻² solves flatness/horizon problems without inflaton

## License

Private research. All rights reserved.

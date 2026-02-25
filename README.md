# Phase-Lifted Complex Conductance Update

**ID:** `eq-arp-phase-lifted-complex-conductance`  
**Tier:** derived  
**Score:** 71  
**Units:** OK  
**Theory:** PASS-WITH-ASSUMPTIONS  

## Equation

$$
\frac{d\tilde G_{ij}}{dt}=\alpha_G\,|I_{ij}(t)|\,e^{i\theta_{R,ij}(t)}-\mu_G\,\tilde G_{ij}(t),\qquad \theta_{R,ij}(t)=\mathrm{unwrap}\!\big(\arg I_{ij}(t);\theta_{\rm ref},\pi_a\big)
$$

## Description

Complex-admittance lift of ARP: conductance grows along the instantaneous current phasor direction using a Phase-Lifted (unwrapped) phase. Assumes phase-coherent transport where a complex ~G is meaningful. Optional variant: include a Z2 parity factor b_ij = (-1)^{w_ij} multiplying e^{iÃƒÅ½Ã‚Â¸_R,ij} to model sign flips under branch crossings.

## Repository Structure

```
images/       # Visualizations, plots, diagrams
derivations/  # Step-by-step derivations and proofs
simulations/  # Computational models and code
data/         # Numerical data, experimental results
notes/        # Research notes and references
```

## Links

- [TopEquations Leaderboard](https://rdm3dc.github.io/TopEquations/leaderboard.html)
- [TopEquations Main Repo](https://github.com/RDM3DC/TopEquations)
- [Certificates](https://rdm3dc.github.io/TopEquations/certificates.html)

---
*Part of the [TopEquations](https://github.com/RDM3DC/TopEquations) project.*

## Contributing

You can add images, derivations, simulations, data, or notes to this repo:

| Folder | What goes here |
|--------|---------------|
| `images/` | Plots, diagrams, phase portraits, animations (.png, .jpg, .mp4, ...) |
| `derivations/` | Step-by-step derivations and proofs (.tex, .md, .pdf) |
| `simulations/` | Computational models and code (.py, .ipynb, .jl, .m) |
| `data/` | Numerical results, experimental measurements (.csv, .hdf5, .npy) |
| `notes/` | Research notes, lit reviews, references (.md, .bib, .txt) |
| `docs/` | Formal documents, validation plans (.md, .pdf) |

**Three ways to contribute:**
1. **GitHub Issue** — click [New Issue](../../issues/new?template=artifact_submission.yml) and attach your file
2. **Pull Request** — fork, add files, open a PR
3. **CLI** — `python tools/push_to_equation_repo.py --equation-id eq-arp-phase-lifted-complex-conductance --file <path> --folder <folder>`

All submissions are content-moderated. See the [full contributing guide](https://github.com/RDM3DC/TopEquations/blob/main/CONTRIBUTING.md).

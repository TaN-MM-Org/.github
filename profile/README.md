# TaN-MM-Org

**Verified research software for experimental quantum and
condensed-matter photonics.**

This organization is the software home of
[Tanvir Mahmud Mahim](https://github.com/Tanvir-Mahmud-Mahim)
(Department of Electrical and Electronic Engineering, BRAC
University). Each repository is the general-purpose engine distilled
from a research study: the physics that outlives the paper, packaged
so an experimental group can drive it with their own measured
numbers.

## The toolbox

| Package | What it does |
|---|---|
| [**sqzcomb**](https://github.com/TaN-MM-Org/sqzcomb) | Squeezed light in Kerr microcombs: from the field in the ring to the noise a detector on the output fiber reports. |
| [**cavsqueeze**](https://github.com/TaN-MM-Org/cavsqueeze) | Cavity-mediated spin squeezing for solid-state ensembles — a quadrillion spins as cheap as a thousand — plus estimation from measured shot records. |
| [**vacspin**](https://github.com/TaN-MM-Org/vacspin) | Group-IV colour-centre spin-photon interfaces: strained spin Hamiltonians, cyclicity, Purcell budgets, exact single-shot readout. |
| [**sparq-triage**](https://github.com/TaN-MM-Org/sparq-triage) | Single-photon-emitter verification: exact statistics for measured HBT data, sequential tests that stop early, machine-learning triage. |
| [**absnoise**](https://github.com/TaN-MM-Org/absnoise) | Andreev-bound-state occupation noise and the sensitivity budgets of proximity Josephson detectors. |
| [**kpenvelope**](https://github.com/TaN-MM-Org/kpenvelope) | Six-band k·p envelope solver for wurtzite heterostructures, self-consistent with the electrostatics of the hole gas. |
| [**ramansep**](https://github.com/TaN-MM-Org/ramansep) | Strain, carrier density and temperature separated in Raman maps of 2D materials, with honest error bars. |
| [**hamop**](https://github.com/TaN-MM-Org/hamop) | One tight-binding Hamiltonian, every observable: bands, optics, topology, transport, magnetic fields — strictly consistent. |
| [**fabtwin**](https://github.com/TaN-MM-Org/fabtwin) | Learned fabrication-process twins and yield-aware inverse design of multilayer optics, with exact adjoint gradients. |

All packages install from PyPI (`pip install <name>`), run on NumPy/SciPy
cores, and are archived release-by-release on Zenodo with citable DOIs.

## Three rules every repository follows

1. **No uncited constants.** Every physical number carries its source,
   and parameter containers refuse to exist without a `reference`.
2. **No unanchored claims.** Every physics statement is pinned by a
   test to a closed form, a published measurement, or two independent
   code paths — never to a stored number.
3. **Honest refusals.** Outside its regime of validity, or facing an
   unidentifiable problem, a tool refuses with an explanation instead
   of returning one of many possible answers.

## Support

Every repository takes questions and bug reports through its issue
tracker; a docstring that left a unit or a convention unclear is
treated as a documentation bug, not user error. Wrong-number reports
are the most valuable issues research software can receive and are
handled with priority.

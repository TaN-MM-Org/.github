# TaN-MM-Org

**Tested research software for experimental quantum,
condensed-matter and high-frequency physics.**

This organization is the software home of
[Tanvir Mahmud Mahim](https://github.com/Tanvir-Mahmud-Mahim)
(Department of Electrical and Electronic Engineering, BRAC
University). Each repository takes the reusable part of a research
study and packages it so that any lab can run it with its own
measured numbers.

## The toolbox

| Package | What it is for |
|---|---|
| [**ramansep**](https://github.com/TaN-MM-Org/ramansep) | Raman maps of atomically thin materials: separates strain from extra electric charge (and can read temperature), with honest error bars. |
| [**kpenvelope**](https://github.com/TaN-MM-Org/kpenvelope) | Holes (missing electrons) trapped in thin layered nitride semiconductors such as GaN: energy levels and masses, solved together with the electrostatics of the trapped charge. |
| [**sqzcomb**](https://github.com/TaN-MM-Org/sqzcomb) | Squeezed light from tiny ring resonators: how much quieter-than-normal light a real detector will actually see, after every loss. |
| [**absnoise**](https://github.com/TaN-MM-Org/absnoise) | Built-in noise of superconducting junctions, and what it means for using them as ultra-sensitive thermometers and energy detectors. |
| [**cavsqueeze**](https://github.com/TaN-MM-Org/cavsqueeze) | Huge ensembles of spins in a resonator driven into a quieter "squeezed" state for better clocks and sensors; the cost depends on the ensemble's shape, not its size. |
| [**sparq-triage**](https://github.com/TaN-MM-Org/sparq-triage) | Screening candidate single-photon sources: analyses photon-timing data, decides when enough has been measured, and can learn the screening strategy. |
| [**vacspin**](https://github.com/TaN-MM-Org/vacspin) | Defects in diamond that act as quantum memories linked to light: energy levels under strain and field, light collection with a cavity, single-shot readout. |
| [**hamop**](https://github.com/TaN-MM-Org/hamop) | One simple model of electrons hopping between atoms, and every property computed from it: energy bands, light absorption, current flow, topology, magnetic fields. |
| [**fabtwin**](https://github.com/TaN-MM-Org/fabtwin) | Optical coatings made of many thin layers: learns a deposition machine's real errors from its logs and redesigns the coating so that even bad runs work. |
| [**fracpll**](https://github.com/TaN-MM-Org/fracpll) | Frequency synthesizers (phase-locked loops that turn one clean clock into a precise, adjustable frequency): stability, noise, timing jitter, lock-in and unwanted tones, from your measured parts. |
| [**lockkernel**](https://github.com/TaN-MM-Org/lockkernel) | The moment a crowd of different oscillators starts beating together: exact onset and growth, and fits of measured data with error bars. |
| [**labplan**](https://github.com/TaN-MM-Org/labplan) | Plan, fit and document a calibration of any model you can write as a Python function: which settings to measure, how many repeats, honest error bars, an audit-ready record. |

Every package also works with a lab's own measurements. Most can plan
a measurement before it is taken (which settings to measure, and how
many repeats a target error bar will cost) and then fit the measured
data with honest error bars. **labplan** is that planning-and-fitting
layer on its own.

Each package installs from PyPI (`pip install <name>`). All are
built on NumPy, most also on SciPy, and a few add a small extra
package (for example mpmath in lockkernel); heavier tools such as
QuTiP, JAX or PyTorch are optional extras. Every release is archived
on Zenodo with its own citable DOI.

## How the tools are checked

1. **Sources for numbers.** Built-in physical constants and parameter
   sets carry a citation to where they come from, and in most
   packages a parameter set cannot be created without a `reference`.
2. **Tests against something independent.** The main results are
   checked by automated tests, run publicly on every change, against
   textbook formulas, published measurements, or a second calculation
   done a different way.
3. **Refusals instead of guesses.** When a question falls outside what
   a model can answer reliably, or the data cannot determine what was
   asked, the tool stops with an explanation instead of returning a
   number that looks fine but is not.

In September 2026 every package's README was rewritten in plain
language, with worked examples whose printed output is checked by
running them. Checking each README line by line against its code also
found real bugs. Each one is fixed, with a new test, in a patch release
of every package, and each release's notes and changelog list them.

## Support

Questions and bug reports are welcome in each repository's issue
tracker. A docstring that leaves a unit or a convention unclear is
treated as a documentation bug, not user error. Reports of a wrong
number are the most valuable issues research software can receive and
are handled first.

## Sponsor this work

Everything here is open source under Apache-2.0 and always will be.
If these tools save your lab time and you would like to support their
development, you can sponsor the work on
[Patreon](https://www.patreon.com/u40002728). It funds the
maintenance, the checking of every shipped constant against the
literature, and the automated tests that keep the releases honest.
Citing the tools in your publications (each repository carries
citation metadata and a Zenodo DOI) helps just as much.

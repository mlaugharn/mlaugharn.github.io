### Marc Laugharn
#### data compression / machine learning researcher & software engineer

- researcher @ [granica.ai](https://granica.ai)

- BS from harvey mudd college, *cs + math major, with finance concentration*


---
other stuff
---

#### *Thermal and contaminant dynamics profiling of the James Webb Space Telescope (2019-2021)*


[Numerical study of water ice and molecular contamination build up during JWST deployment by Lubos Brieda, **Marc Laugharn**, Michael Woronowicz, Kelly Henderson-Nelson, Christopher May, Eve Wooldridge in Proc.SPIE, Vol. 12224, Page 1222403, 2022](https://doi.org/10.1117/12.2635238) [![DOI:10.1117/12.2635238](https://zenodo.org/badge/DOI/10.1117/12.2635238.svg)](https://doi.org/10.1117/12.2635238)

Lead by Lubos Brieda, in collaboration with teams at NASA, I contributed to an assessment of the deployment cycle of the James Webb Telescope. I extended the functionality of [Particle-in-Cell](https://www.particleincell.com/)'s simulation platform [CTSP](https://www.particleincell.com/ctsp/). 

JWST uses very sensitive infrared-based imaging systems, and our goals were to ensure:
  1. temperature-sensitive imaging systems would operate within defined bounds, and not be negatively impacted by low temperatures in outer space
  2. contaminant deposition/adsorption/emission levels would be acceptable
  
My contributions:
- co-development of state tracking between simulated JWST deployment stages.
  - deployment was over 17 stages (= 17 geometry meshes, each 1M+ vertices)) over 180 days.
  - our system tracked thermal and contamination states between stages, across varying timescales, and between changing geometric configurations

- implementation of
  - extended support for the .TSS (Thermal Synthesizer System) file format, allowing broader conformance of the spec
  - alignment between new, updated geometry meshes and prior materials assignments
  
- enhancements to:
  - coordinate-system & geometry representations
  - parser performance, allowing efficient loading of multi-gigabyte meshes
  - numerical stability of particle-mesh interactions

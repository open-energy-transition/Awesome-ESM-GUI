<!--
SPDX-FileCopyrightText: 2025 Open Energy Transition (OET)

SPDX-License-Identifier: CC0-1.0
-->

# Awesome Energy System Modelling (ESM) Graphical User Interfaces (GUIs)

A curated collection of graphical user interfaces for creating, running, and analysing energy system models.

This list includes both open-source and proprietary GUIs, for both open-source and proprietary modelling tools.

[![Check Links](https://github.com/open-energy-transition/Awesome-ESM-GUI/actions/workflows/link-check.yml/badge.svg)](https://github.com/open-energy-transition/Awesome-ESM-GUI/actions/workflows/links.yml)

## Disclaimer

This repository is for educational and research use only.
We do not host, own, or guarantee the availability of any linked GUIs.
Some GUIs may require proprietary software (e.g., GAMS, PLEXOS) or commercial licenses to access or use.
Inclusion of such GUIs does not imply endorsement, affiliation, or sponsorship by any software vendor.
All trademarks are the property of their respective owners and are used here solely for identification and interoperability purposes.
Users are responsible for obtaining appropriate software licenses and complying with all applicable terms.
For GUI-specific inquiries, contact the original data providers.

We group GUIs by:

- whether they are open-source or proprietary;
- the modelling framework they leverage to create the model, if it is a general framework independent of the GUI itself; and
- whether the GUI can be used for:
  - creating validated input files for a given modelling framework.
  - analysing input/output data of a given modelling framework.
  - creating, running, and analysing a model in one.

## Table of contents

- [Disclaimer](#disclaimer)
- [Contribution Guide](#contribution-guide)
  - [Contribution Tips](#contribution-tips)
  - [How to Contribute](#how-to-contribute)
- [Open-Source GUIs](#open-source-guis)
- [Proprietary GUIs](#proprietary-guis)

## Contribution Guide

### Contribution Tips

- Prefer official or well-maintained sources.
- Ensure the GUI is available for download (or add any additional relevant instructions).
- Avoid duplicate entries.
- If a GUI is no longer available, feel free to open an issue or submit a PR to remove or update the link.

### How to Contribute

1. **Fork the Repository**
   Click the "Fork" button at the top right of this page to create your own copy.
2. **Create a Branch**Create a new branch for your contribution (replace `my-gui-addition` with your own branch name):

   ```bash
   git checkout -b my-gui-addition
   ```

3. **Add or Update Content**

   - Add new GUIs to the tables in the appropriate section (open-source / proprietary).
   - Include a short description and a direct link to the GUI source.
   - Where possible, use git source code repository URLs when providing links.

4. **Follow Formatting**

   - Use the existing Markdown style for consistency.
   - Place new entries in alphabetical or logical order within each section.

5. **Commit and Push**Again replace `my-gui-addition` with your own branch name.

   ```bash
   git add README.md
   git commit -m "Add [GUI name] to [section]"
   git push origin my-gui-addition
   ```

6. **Open a Pull Request**

   - Go to your fork on GitHub and click "Compare & pull request".
   - Provide a clear description of your changes in your pull request, then create the pull request for review.

---

## Open-source GUIs

| GUI | Modelling framework | Usage |
| --- | --- | --- |
| [Antares Web](https://github.com/AntaresSimulatorTeam/AntaREST) | [Antares](https://github.com/AntaresSimulatorTeam/Antares_Simulator) | build-run-analyse |
| [Cairn Viewer](https://cea-liten.github.io/CairnOpen/hmi_guide/build_a_problem.html) | [CairnOpen](https://github.com/CEA-Liten/CairnOpen) | build-run-analyse |
| [calligraph](https://github.com/calliope-project/calligraph) | [Calliope](https://github.com/calliope-project/calliope/) | analyse |
| [Electrisim Community Edition](https://github.com/electrisim) | [OpenDSS](https://www.epri.com/pages/sa/opendss) / [pandapower](https://github.com/e2nIEE/pandapower) | build-run-analyse |
| [MUIO](https://github.com/OSeMOSYS/MUIO) | [OSeMOSYS](https://github.com/OSeMOSYS/OSeMOSYS) | build-run-analyse |
| [NLR Engage](https://engage.nlr.gov/en/login/?next=/en/) | [Calliope](https://github.com/calliope-project/calliope/) | build-run-analyse |
| [OpenDSS](https://www.epri.com/pages/sa/opendss) | N/A | build-run-analyse |
| [PowerGenome](https://github.com/PowerGenome/PowerGenome) | [GenX](https://github.com/genxproject/genx.jl) | build |
| [PyPSA-App](https://github.com/PyPSA/pypsa-app) | [PyPSA](https://github.com/PyPSA/pypsa) | run-analyse |
| [pypsa-explorer](https://github.com/open-energy-transition/PyPSA-Explorer) | [PyPSA](https://github.com/PyPSA/pypsa) | analyse |
| [Spine Toolbox](https://github.com/spine-tools/Spine-Toolbox) | [SpineOpt](https://github.com/spine-tools/SpineOpt.jl) | build-run-analyse |
| [VeraGrid](https://github.com/SanPen/VeraGrid) | N/A | build-run-analyse |

## Proprietary GUIs

| GUI | Modelling framework | Usage |
| --- | --- | --- |
| [Convexity](https://www.bayesian.energy/convexity) | [PyPSA](https://github.com/PyPSA/pypsa) | build-run-analyse (licensed) |
| [Electrisim](https://electrisim.com/) | [OpenDSS](https://www.epri.com/pages/sa/opendss) / [pandapower](https://github.com/e2nIEE/pandapower) | build-run-analyse (licensed) |
| [GridCog](https://www.gridcog.com/) | N/A | build-run-analyse (licensed) |
| [HOMER Pro](https://homerenergy.com) | N/A | build-run-analyse (licensed) |
| [PHOS-UK](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6751106) | N/A | build-run-analyse (unavailable) |
| [Scenario builder](https://www.transitionzero.org/products/scenario-builder) | [PyPSA](https://github.com/PyPSA/pypsa) / [OSeMOSYS](https://github.com/transition-zero/tz-osemosys) | build-run-analyse (free) |
| [STELLAR](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2121429&reg=3&lang=2) | N/A | build-run-analyse (unavailable) |
| [tera-joule](https://tera-joule.com/) | N/A | build-run-analyse (licensed) |
| [VAMOS](https://www.tugraz.at/fileadmin/user_upload/tugrazExternal/4778f047-2e50-4e9e-b72d-e5af373f95a4/files/pr/Session_C2/321_PR_Wiedner.pdf) | N/A | build-run-analyse (unavailable) |
| [VEDA](https://github.com/kanors-emr/Veda2.0-Installation) | [TIMES](https://github.com/etsap-TIMES/TIMES_model) | build-run-analyse (licensed) |
| [xendee](https://xendee.com/) | N/A | build-run-analyse (licensed) |
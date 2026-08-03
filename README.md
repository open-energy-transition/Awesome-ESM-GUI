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
- [Column key](#column-key)
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

## Column key

### Modelling framework

Under the hood, some GUIs wrap modelling frameworks that can be accessed independently as software packages with their own API.

### Usage

We define our GUIs as covering three usage categories:

- **build**: the GUI can be used to construct an energy/power system model from scratch.
- **run**: the GUI can be used to run a built energy/power system model optimisation/simulation.
- **analyse**: the GUI can be used to inspect the input data and the results of running an energy/power system model.

### Focus area

Although the GUIs (and underlying modelling frameworks) are usually marketed towards certain audiences, they tend to fall into two broader focus areas:

- **system planning**: Supporting investment and market participation decisions for systems across spatial scales, from smart home energy systems to international power systems.
  The underlying frameworks usually run a linear cost minimising optimisation, sometimes to co-optimise investment and operation decisions and sometimes only operation (usually under conditions of uncertainty such as for resource adequacy or limited foresight market participation decisions).
- **power flow analysis**: Ensuring the safe and stable operation of existing or planned power systems.
  The underlying frameworks usually run nonlinear simulations iteratively to convergence, to ensure that the power system can supply its load under normal, steady state or transient, dynamic operation.

These two focus areas can overlap, particularly when considering (linearised) optimal power flow.

---

## Open-source GUIs

| GUI | Modelling framework | Usage | Focus area
| --- | --- | --- | ---
| [Antares Web](https://github.com/AntaresSimulatorTeam/AntaREST) | [Antares](https://github.com/AntaresSimulatorTeam/Antares_Simulator) | build-run-analyse | system planning
| [Cairn Viewer](https://cea-liten.github.io/CairnOpen/hmi_guide/build_a_problem.html) | [CairnOpen](https://github.com/CEA-Liten/CairnOpen) | build-run-analyse | system planning
| [calligraph](https://github.com/calliope-project/calligraph) | [Calliope](https://github.com/calliope-project/calliope/) | analyse | system planning
| [Electrisim Community Edition](https://github.com/electrisim) | [OpenDSS](https://www.epri.com/pages/sa/opendss) / [pandapower](https://github.com/e2nIEE/pandapower) | build-run-analyse | power flow
| [MUIO](https://github.com/OSeMOSYS/MUIO) | [OSeMOSYS](https://github.com/OSeMOSYS/OSeMOSYS) | build-run-analyse | system planning
| [NLR Engage](https://engage.nlr.gov/en/login/?next=/en/) | [Calliope](https://github.com/calliope-project/calliope/) | build-run-analyse | system planning
| [OpenDSS](https://www.epri.com/pages/sa/opendss) | N/A | build-run-analyse | power flow
| [PowerGenome](https://gschivley.github.io/PowerGenome-tools/web_app/) | [GenX](https://github.com/genxproject/genx.jl) | build | system planning
| [PyPSA-App](https://github.com/PyPSA/pypsa-app) | [PyPSA](https://github.com/PyPSA/pypsa) | run-analyse | system planning
| [pypsa-explorer](https://github.com/open-energy-transition/PyPSA-Explorer) | [PyPSA](https://github.com/PyPSA/pypsa) | analyse | system planning
| [Ragnarok](https://github.com/iam-hongsanghyun/project-Ragnarok) | [PyPSA](https://github.com/PyPSA/pypsa) | build-run-analyse | system planning
| [Spine Toolbox](https://github.com/spine-tools/Spine-Toolbox) | [SpineOpt](https://github.com/spine-tools/SpineOpt.jl) | build-run-analyse | system planning
| [VeraGrid](https://github.com/SanPen/VeraGrid) | N/A | build-run-analyse | power flow

## Proprietary GUIs

| GUI | Modelling framework | Usage | Focus area
| --- | --- | --- | ---
| [Convexity](https://www.bayesian.energy/convexity) | [PyPSA](https://github.com/PyPSA/pypsa) | build-run-analyse (licensed) | system planning
| [Electrisim](https://electrisim.com/) | [OpenDSS](https://www.epri.com/pages/sa/opendss) / [pandapower](https://github.com/e2nIEE/pandapower) | build-run-analyse (licensed) | power flow
| [GridCog](https://www.gridcog.com/) | N/A | build-run-analyse (licensed) | system planning
| [HOMER Software](https://homerenergy.com) | N/A | build-run-analyse (licensed) | system planning
| [OptGen](https://www.psr-inc.com/en/software/optgen/) | N/A | build-run-analyse (licensed) | system planning
| [PHOS-UK](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6751106) | N/A | build-run-analyse (unavailable) | system planning
| [PlanOS](https://www.gevernova.com/consulting/planos) | N/A |  build-run-analyse (licensed) | system planning & power flow
| [PLEXOS](https://www.energyexemplar.com/plexos) | N/A | build-run-analyse (licensed) | system planning
| [PowerFactory](https://www.digsilent.de/en/powerfactory.html) | N/A | build-run-analyse (licensed) | power flow
| [PSS E](https://www.siemens.com/en-gb/products/pss-software/psse/) | N/A | build-run-analyse (licensed) | power flow
| [Scenario builder](https://www.transitionzero.org/products/scenario-builder) | [PyPSA](https://github.com/PyPSA/pypsa) / [OSeMOSYS](https://github.com/transition-zero/tz-osemosys) | build-run-analyse (free) | system planning
| [SDDP](https://www.psr-inc.com/en/software/sddp/) | N/A | build-run-analyse (licensed) | system planning
| [STELLAR](https://youtu.be/p3z8ecdU0IY) | N/A | build-run-analyse (unavailable) | system planning
| [VAMOS](https://www.tugraz.at/fileadmin/user_upload/tugrazExternal/4778f047-2e50-4e9e-b72d-e5af373f95a4/files/pr/Session_C2/321_PR_Wiedner.pdf) | N/A | build-run-analyse (unavailable) | system planning
| [VEDA](https://github.com/kanors-emr/Veda2.0-Installation) | [TIMES](https://github.com/etsap-TIMES/TIMES_model) | build-run-analyse (licensed) | system planning
| [xendee](https://xendee.com/) | N/A | build-run-analyse (licensed) | system planning

# LM

![license](https://img.shields.io/badge/license-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-laptops-lightgrey)

> Anticloud-hardened packaging of the upstream project `LM` in category **LAPTOPS**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** LAPTOPS · **Upstream:** https://github.com/lmstudio-ai/lms · **Upstream pin:** `dcefd5aa69f56b503ae118a7a7ba91cb378a8479` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

<p align="center">
  <br/>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://files.lmstudio.ai/lms-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="https://files.lmstudio.ai/lms-light.png">
    <img alt="lmstudio cli logo" src="https://files.lmstudio.ai/lms-light.png" width="180">
  </picture>
  <br/>
  <br/>
</p>

<p align="center"><bold><code>lms</code> - Command Line Tool for <a href="https://lmstudio.ai/">LM Studio</a></bold></p>
<p align="center">Built with <bold><code><a href="https://github.com/lmstudio-ai/lmstudio.js">lmstudio.js</a></code></bold></p>

# Installation

`lms` ships with [LM Studio](https://lmstudio.ai/) 0.2.22 and newer.

If you have trouble running the command, try running `npx lmstudio install-cli` to add it to path.

To check if the bootstrapping was successful, run the following in a **👉 new terminal window 👈**:

```shell
lms
```

# Usage

You can use `lms --help` to see a list of all available subcommands.

For details about each subcommand, run `lms <subcommand> --help`.

Here are some frequently used commands:

- `lms status` - To check the status of LM Studio.
- `lms server start` - To start the local API server.
- `lms server stop` - To stop the local API server.
- `lms ls` - To list all downloaded models.
  - `lms ls --json` - To list all downloaded models in machine-readable JSON format.
- `lms ps` - To list all loaded models available for inferencing.
  - `lms ps --json` - To list all loaded models available for inferencing in machine-readable JSON format.
- `lms load` - To load a model
  - `lms load <model path> -y` - To load a model with maximum GPU acceleration without confirmation
- `lms unload <model identifier>` - To unload a model
  - `lms unload --all` - To unload all models
- `lms create` - To create a new project with LM Studio SDK
- `lms log stream` - To stream logs from LM Studio

# Contributing

The CLI is part of the [lmstudio.js monorepo](https://github.com/lmstudio-ai/lmstudio.js) and cannot be built standalone.

## Building and Testing the CLI

```bash
# source and build the entire monorepo
git source https://github.com/lmstudio-ai/lmstudio-js.git --recursive
cd lmstudio-js
npm install
npm run build

# Test your CLI changes
node publish/cli/dist/index.js <subcommand>
```

**Example:**

```bash
node publish/cli/dist/index.js --help
node publish/cli/dist/index.js status
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for more information.

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Node.js / npm** (manifests: package.json; scanned in UPSTREAM_CLONE)
- Top-level source layout: `src/`
- Snapshot size: **112 files**, **16264 lines of code** (measured; see Benchmarks)
- Primary languages: `.ts` (92), `.tsx` (10), `(none)` (4), `.json` (4), `.md` (2)
- Upstream commit pinned for this packaging: `dcefd5aa69f56b503ae118a7a7ba91cb378a8479`

---

## Installation

`lms` ships with [LM Studio](https://lmstudio.ai/) 0.2.22 and newer.

If you have trouble running the command, try running `npx lmstudio install-cli` to add it to path.

To check if the bootstrapping was successful, run the following in a **👉 new terminal window 👈**:

```shell
lms
```

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

You can use `lms --help` to see a list of all available subcommands.

For details about each subcommand, run `lms <subcommand> --help`.

Here are some frequently used commands:

- `lms status` - To check the status of LM Studio.
- `lms server start` - To start the local API server.
- `lms server stop` - To stop the local API server.
- `lms ls` - To list all downloaded models.
  - `lms ls --json` - To list all downloaded models in machine-readable JSON format.
- `lms ps` - To list all loaded models available for inferencing.
  - `lms ps --json` - To list all loaded models available for inferencing in machine-readable JSON format.
- `lms load` - To load a model
  - `lms load <model path> -y` - To load a model with maximum GPU acceleration without confirmation
- `lms unload <model identifier>` - To unload a model
  - `lms unload --all` - To unload all models
- `lms create` - To create a new project with LM Studio SDK
- `lms log stream` - To stream logs from LM Studio

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

</picture>
  <br/>
  <br/>
</p>

<p align="center"><bold><code>lms</code> - Command Line Tool for <a href="https://lmstudio.ai/">LM Studio</a></bold></p>
<p align="center">Built with <bold><code><a href="https://github.com/lmstudio-ai/lmstudio.js">lmstudio.js</a></code></bold></p>

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Node.js / npm |
| Manifests detected | package.json |
| Files in snapshot | 112 |
| Lines of code | 16264 |
| Dependency references | 32 |
| Dependencies by ecosystem | npm: 32 |
| Upstream license | MIT |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| npm | @commander-js/extra-typings | ^14.0.0 | package.json |
| npm | @inquirer/prompts | ^8.0.1 | package.json |
| npm | @lmstudio/immer-with-plugins | ^10.1.1 | package.json |
| npm | @lmstudio/lms-common | ^0.9.0 | package.json |
| npm | @lmstudio/lms-common-server | ^0.3.0 | package.json |
| npm | @lmstudio/lms-es-plugin-runner | ^0.0.21 | package.json |
| npm | @lmstudio/lms-isomorphic | ^0.5.0 | package.json |
| npm | @lmstudio/lms-lmstudio | ^0.0.33 | package.json |
| npm | @lmstudio/sdk | ^2.0.0 | package.json |
| npm | chalk | ^4.1.2 | package.json |
| npm | columnify | ^1.6.0 | package.json |
| npm | fast-glob | ^3.3.2 | package.json |
| npm | fuzzy | ^0.1.3 | package.json |
| npm | ink | ^6.5.1 | package.json |
| npm | react | ^19.2.0 | package.json |
| ... | (17 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- `package.json`

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# Contributing to `lms`

First off, thank you for considering contributing to our open source projects! 👾❤️

`lms` is LM Studio’s command line utility tool. It is an open-source project under the MIT license. We welcome community contributions.

There are many ways to help, from writing tutorials or blog posts, improving the documentation, submitting bug reports and feature requests or contributing code which can be incorporated into `lms` itself.

## Communication

- **The best way to communicate with the team is to open an issue in this project**
- For bug reports, include steps to reproduce, expected behavior, and actual behavior
- For feature requests, explain the use case and benefits clearly

## Before You Contribute

- **If you find an existing issue you'd like to work on, please comment on it first and tag the team**
- This allows us to provide guidance and ensures your time is well spent
- **We discourage drive-by feature PRs** without prior discussion - we want to make sure your efforts align with our roadmap and won't go to waste

## Creating Good Pull Requests

### Keep PRs Small and Focused

- Address one concern per PR
- Smaller PRs are easier to review and more likely to be merged quickly

### Write Thoughtful PR Descriptions

- Clearly explain what the PR does and why
- When applicable, show before/after states or screenshots
- Include any relevant context for reviewers
- Reference the issue(s) your PR addresses with GitHub keywords (Fixes #123, Resolves #456)

### Quality Expectations

- Follow existing code style and patterns
- Include tests for new functionality
- Ensure all tests pass
- Update documentation as needed

## Code Review Process

- Maintainers will review your PR as soon as possible
- We may request changes or clarification
- Once approved, a maintainer will merge your contribution

## Contributor License Agreement (CLA)

- We require all contributors to sign a Contributor License Agreement (CLA)
- For first-time contributors, a bot will automatically comment on your PR with instructions
- You'll need to accept the CLA before we can merge your contribution
- This is standard practice in open source and helps protect both contributors and the project

## Q&A

- **How does `lms` communicate with LM Studio**

  For the most part, `lms` communicates with LM Studio through the `lmstudio.js` SDK. You can find the source code for the SDK [here](https://github.com/lmstudio-ai/lmstudio.js/tree/main). `lmstudio.js` is in pre-releas

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: MIT** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
MIT License

Copyright (c) 2024 LM Studio

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original MIT terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `MIT` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `LM` (category: LAPTOPS)
- **Upstream URL:** https://github.com/lmstudio-ai/lms
- **Pinned commit (SHA):** `dcefd5aa69f56b503ae118a7a7ba91cb378a8479`
- **Branch:** main
- **Pin provenance:** GitHub API commits/main. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`0947d704948182596ad67070f0ea69ee70574c9d55bb1cdaafcdf93f5b21a2de`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.


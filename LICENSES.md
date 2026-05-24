# ExploreStars Envision&trade; - Data & Software Attributions

**Copyright &copy; 2026 Wes McDonald. All rights reserved.**

ExploreStars Envision&trade; is provided as a compiled binary for personal
use with the Explore Scientific&trade; PMC-Eight&trade; mount. The source
code is not publicly distributed. Redistribution of the unmodified binary
is permitted; modification, reverse engineering, decompilation, and source
extraction are not. The software is provided "as is," without warranty of
any kind.

## Trademarks

- **ExploreStars Envision&trade;** is a trademark of Wes McDonald.
- **Explore Scientific&trade;**, **ExploreStars&trade;**, and
  **PMC-Eight&trade;** are trademarks of Explore Scientific, LLC, and are
  used here with acknowledgement.

## Independence and endorsement

ExploreStars Envision&trade; is an independent application that controls
Explore Scientific&trade; PMC-Eight&trade; telescope mounts. The
application code and project materials are authored and owned by Wes
McDonald except where third-party credits are listed below. If Explore
Scientific, LLC recommends, endorses, promotes, or distributes the app,
that endorsement should be understood as support for use of an
independently authored application within the PMC-Eight ecosystem, not as
Explore Scientific authorship or ownership of the app.

## About this document

This document credits every external data source, license, and software
dependency bundled with ExploreStars Envision&trade;. It is the canonical
attribution record. The bundled user manual section
**Credits & Data Sources** summarizes this information for end users; this
file is the authoritative version.

---

## Constellation lines (`constellation_lines.json`)

> Constellation stick-figure line data based on IAU / Sky & Telescope
> figures created by Alan MacRobert et al.; machine-readable transcription
> by Dominic Ford, from `dcf21/constellation-stick-figures`, used under
> CC BY 4.0.

- **License:** Creative Commons Attribution 4.0 International (CC BY 4.0)
  &mdash; <https://creativecommons.org/licenses/by/4.0/>
- **Source:** <https://github.com/dcf21/constellation-stick-figures>
- **Modifications:** the original `.dat` source has been re-encoded into
  JSON form with HIP-pair endpoints for use by ExploreStars Envision. No
  intended changes were made to the underlying stick-figure line choices.

CC BY 4.0 requires that we credit the creators and indicate any changes
we made to the licensed material. We have done both above. The
`constellation_lines.json` file also carries an embedded `"source"`
metadata block recording the same credits and license.

---

## Object catalog (`catalog.csv`) provenance

Portions of the original object database were derived from the **Explore
Scientific&trade; ExploreStars&trade;** database and are used with
permission from Explore Scientific. The bundled ExploreStars Envision
catalog has since been curated, normalized, corrected, and augmented using
public astronomical catalogues and reference services, including ESA
Hipparcos/Tycho, the Yale Bright Star Catalog where applicable, RNGC/IC,
SIMBAD/CDS, and other public astronomical resources.

The sections that follow record the specific external sources contributing
to the curated catalog.

---

## Star data &mdash; ESA Hipparcos / Tycho-II

Stellar entries in `catalog.csv` and the chart's `stars_mag6.json` are
derived from the European Space Agency (ESA) **Hipparcos** and
**Tycho-II** catalogues, used in accordance with the ESA data policy.

- **Credit:** ESA / Hipparcos / Tycho
- **Catalogue references:**
  - Hipparcos Catalogue (1997): VizieR I/239
  - Tycho-II Catalogue (2000): VizieR I/259

Cross-reference identifiers used to label catalogue entries &mdash;
**Bayer**, **Flamsteed**, **SAO**, **HD / Harvard**, **DM**,
**BD / CD / CPD**, **GSC** &mdash; are public-domain naming systems and
require no additional attribution. They are listed here for transparency.

---

## Deep-sky objects &mdash; RNGC / IC

Non-stellar entries in `catalog.csv` originated with the legacy
ExploreStars catalog and trace to the **Revised New General Catalogue
(RNGC)** and the **Index Catalogue (IC)** &mdash; both in the public
domain.

---

## Object thumbnails &mdash; astrophotography

Object thumbnail images shown on the Target page are sourced from:

- **Explore Scientific** &mdash; original ExploreStars project images
  (Messier objects, NGC, solar system), used with permission.
- **Jim McKee** &mdash; astrophotographs marked "Jim McKee" in the
  Target-page caption, used with permission. See more of his work on
  AstroBin: <https://app.astrobin.com/u/mckeejh>
- **NASA / JPL** &mdash; specific solar-system and deep-sky imagery
  (e.g., Pluto from New Horizons, PIA19857; Christmas Tree Cluster
  wide-field), public domain.
- **Chuck Ayoub** &mdash; Crescent Nebula (NGC 6888) photograph
  obtained via Wikimedia Commons under the **Creative Commons CC0 1.0
  Universal Public Domain Dedication**. The author has dedicated the
  work to the public domain by waiving all copyright; no permission is
  required to use, modify, or redistribute it. The photographer credit
  is retained on the Target page as a courtesy.
  CC0 1.0: <https://creativecommons.org/publicdomain/zero/1.0/>

---

## Planetary, solar, and lunar positions

Positions are computed from algorithms in:

> Jean Meeus, *Astronomical Algorithms*, 2nd ed., Willmann-Bell, 1998.

The mathematics is in the public domain; credit is retained here as a
courtesy to the author whose presentation made the implementation
practical.

---

## Acknowledgments

The catalog has been augmented with cross-references and additional
entries curated using **SIMBAD** (operated at CDS, Strasbourg, France)
and other public astronomical resources.

- SIMBAD: <https://simbad.u-strasbg.fr/simbad/>

SIMBAD's published acknowledgment line is intended for academic
publications; this courtesy credit is included here for transparency
about how the catalog was curated.

Thanks to **Jerry Hubbell** of Explore Scientific, LLC, for fruitful
discussions during development and assistance with field testing.

Thanks to **Ignazio Pillitteri** for contributing the Linux/macOS PWA
server bash script (`start-servers.sh`) and Caddyfile cross-platform
improvements that enable ExploreStars Envision to run on Linux and
macOS hosts in addition to Windows.

---

## Software dependencies

ExploreStars Envision&trade; depends on the following open-source
libraries. License texts are bundled with the .NET runtime and the
corresponding NuGet packages installed at build time.

| Component | License |
|---|---|
| MudBlazor | MIT |
| Microsoft.Maui.Controls | MIT |
| Microsoft.AspNetCore.Components.WebView.Maui | MIT |
| .NET 9 runtime + Blazor | MIT |
| System.IO.Ports | MIT |
| Caddy server (development-only HTTPS proxy) | Apache 2.0 |
| Node.js (development-only mount-proxy) | MIT |

---

## Application code

The ExploreStars Envision&trade; application &mdash; Razor pages,
services, JavaScript chart engine (Star Seeker), build scripts, and
supporting tooling &mdash; is the work of **Wes McDonald** and is
released under the all-rights-reserved binary terms stated at the top of
this document.

A separate private grant covers Explore Scientific, LLC's source-level
rights of use, modification, internal distribution, binary distribution,
endorsement / promotional use, and any ES-specific changes or ecosystem
integration work; that grant is documented outside this file.

---

*Document version: 2026-05-23 (aligned with Explore Scientific licensing
proposal draft)*

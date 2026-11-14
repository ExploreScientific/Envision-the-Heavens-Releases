# Envision the Heavens&trade; - Data & Software Attributions

**Copyright &copy; 2026 Wes McDonald. All rights reserved.**

Envision the Heavens&trade; is provided as a compiled binary for personal
use with the Explore Scientific&trade; PMC-Eight&trade; mount. The source
code is not publicly distributed. Redistribution of the unmodified binary
is permitted; modification, reverse engineering, decompilation, and source
extraction are not. The software is provided "as is," without warranty of
any kind.

## Trademarks

- **Envision the Heavens&trade;** is a trademark of Wes McDonald.
- **Explore Scientific&trade;**, **ExploreStars&trade;**, and
  **PMC-Eight&trade;** are trademarks of Explore Scientific, LLC, and are
  used here with acknowledgement.

## Independence and endorsement

Envision the Heavens&trade; is an independent application that controls
Explore Scientific&trade; PMC-Eight&trade; telescope mounts. The
application code and project materials are authored and owned by Wes
McDonald except where third-party credits are listed below. If Explore
Scientific, LLC recommends, endorses, promotes, or distributes the app,
that endorsement should be understood as support for use of an
independently authored application within the PMC-Eight ecosystem, not as
Explore Scientific authorship or ownership of the app.

## About this document

This document credits every external data source, license, and software
dependency bundled with Envision the Heavens&trade;. It is the canonical
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
  JSON form with HIP-pair endpoints for use by Envision. No
  intended changes were made to the underlying stick-figure line choices.

CC BY 4.0 requires that we credit the creators and indicate any changes
we made to the licensed material. We have done both above. The
`constellation_lines.json` file also carries an embedded `"source"`
metadata block recording the same credits and license.

---

## Object catalog (`catalog.csv`) provenance

Portions of the original object database were derived from the **Explore
Scientific&trade; ExploreStars&trade;** database and are used with
permission from Explore Scientific. The bundled Envision
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

Star positions, proper motions, magnitudes and HIP / HD / HR
cross-references of about 250 entries were corrected against the **HYG
database v4.0** (David Nash, astronexus; CC BY-SA 4.0;
https://codeberg.org/astronexus/hyg), itself compiled from Hipparcos,
Yale Bright Star and Gliese (`tools/fix_catalog_from_hyg.py`).

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

Object images shown on the Target page and the Star Seeker chart are sourced from:

- **Explore Scientific** &mdash; original ExploreStars project images
  (Messier objects, NGC, solar system), used with permission.
- **Jim McKee** &mdash; astrophotographs marked "Jim McKee" in the
  Target-page caption, used with permission. The California Nebula
  (`NGC1499.jpg`) has its faint oxygen layer brought out for display, with
  his OK (stars and hydrogen as he processed them). See more of his work on
  AstroBin: <https://app.astrobin.com/u/mckeejh>
- **Wes McDonald** &mdash; the Lagoon Nebula (M8), the app author's own
  photograph.
- **Ryan Wecker** &mdash; the Hercules Cluster (M13), taken on an iEXOS-100-2,
  used with permission; cropped to the cluster and scaled to 500 × 500.
- **Sean M McHenry** &mdash; LDN 1251, the Angler Fish Nebula, taken on an
  iEXOS-100-2. `images/LDN1251.jpg` (a crop around the nebula, for the Target
  page) and `images/LDN1251-wide.jpg` (his full field, for the Star Seeker
  chart), both scaled to 500 × 281 and letterboxed. Permission, in his words
  (2026-10-26): "I hereby allow the company known as Explore Scientific,
  specifically Wes McDonald, the right to use my image of LDN 1251, the Dark
  Nebula known as the Angler Fish Nebula for the purposes of their programming,
  advertising, and outreach with credit to me, Sean M McHenry, the owner of this
  artwork/image."
  - **His wide fields for the Star Seeker chart**, all on the iEXOS-100-2 with an
    SVBony SV535 lens and a ZWO ASI 585MC Pro: `images/NGC6883-wide.jpg` (Tulip
    to NGC 6883 and WR 134), `images/NGC7822-wide.jpg` (NGC 7822 and Cederblad
    214), `images/NGC7000-wide.jpg` (North America and Pelican) and
    `images/Sh2-114-wide.jpg` (the Flying Dragon) and `images/Sadr-wide.jpg` (Sadr),
    each scaled to 1400 px on its longer side, except Sadr: his 6° field, scaled from
    5376 × 3024 to 2000 × 1125. Some are lightly edited for presentation, as Sean
    allowed ("rotate and adjust the colors as needed").
  - **Target page pictures from those fields:** `images/NGC7822.jpg` (the whole
    NGC 7822 frame), and crops placed with his plate solves: `images/Ced214.jpg`
    (0.9° around NGC 7822's bright rim) and `images/Sh2-104.jpg` (0.45°, from the
    Tulip field); each scaled to 500 × 500. (`images/WR134.jpg` was a crop of the
    Tulip field until 2026-11; it is now Jim McKee's own picture of the WR 134 ring.)
  - **Permission, in his words (2026-10-30, adding Sadr to his 2026-10-26 list):** "I
    hereby allow Explore Scientific and Wes McDonald the right to use my images
    (listed specifically below) for the purposes of their programming, advertising,
    and outreach, with credit to me, Sean M McHenry, the owner of these images. I
    grant the above permission to use the following images which I have submitted by
    email: 1. LDN 1251 the Dark Nebula known as the Angler Fish Nebula 2. Tulip
    Nebula to NGC 6883 and the WR 134 ring (Cygnus) 3. NGC 7822 with Cederblad 214
    (Cepheus) 4. North America and Pelican Nebulae (Cygnus) 5. The Flying Dragon,
    Sh2-114, around HIP 105561 (Cygnus) 6. The Sadr Region, 105mm wide dual band
    image"
- **Steve Lang** &mdash; the War and Peace Nebula (NGC 6357), taken on an
  Explore Scientific G11, used with permission; the Star Seeker chart's wide
  field (`images/NGC6357-wide.jpg`, scaled to 1400 × 1031). The
  Target page keeps Jim McKee's close-up.
  - **The Vela Supernova Remnant**, on the G11 with an ES 80mm FCD100 APO
    (`images/VelaSNR-wide.jpg`), used with
    permission: his SHO version (2026-10), lightly edited for presentation, scaled
    to 920 × 1400 for the Star Seeker chart (`VelaSNR-wide.jpg`)
    and to 328 × 500, letterboxed, for the Target page (`VelaSNR.jpg`).
  - **The Carina Nebula** (`images/NGC3372.jpg`, `images/NGC3372-wide.jpg`), used with
    permission: lightly edited for presentation, scaled to 1400 × 1134 for the Star Seeker
    chart and to 500 × 405, letterboxed, for the Target page.
- **NASA / JPL** &mdash; specific solar-system and deep-sky imagery
  (e.g., Pluto from New Horizons, PIA19857; Christmas Tree Cluster
  wide-field), public domain. The Sombrero Galaxy (M104) is NASA/ESA and
  the Hubble Heritage Team (STScI/AURA), release opo0328a, via Wikimedia
  Commons, public domain. The Crab Nebula close-up (`images/M1.jpg`) is NASA,
  ESA, J. Hester and A. Loll (Arizona State University), via Wikimedia Commons,
  public domain; Jim McKee's Crab is `M1-wide.jpg`.
- **Chuck Ayoub** &mdash; Crescent Nebula (NGC 6888) photograph
  obtained via Wikimedia Commons under the **Creative Commons CC0 1.0
  Universal Public Domain Dedication**. The author has dedicated the
  work to the public domain by waiving all copyright; no permission is
  required to use, modify, or redistribute it. The photographer credit
  is retained on the Target page as a courtesy.
  CC0 1.0: <https://creativecommons.org/publicdomain/zero/1.0/>
- **Taavi Niittee** &mdash; "Heart and Soul" (`images/IC1848-wide.jpg`, the
  Star Seeker chart's wide field for the Soul Nebula; the Target page keeps
  Jim McKee's close-up), from Wikimedia Commons under **CC0 1.0**:
  <https://commons.wikimedia.org/wiki/File:Heart_and_soul.jpg>. Scaled from
  6302 × 9720 to 324 × 500 and padded to 500 × 500. Credited as a courtesy.
- **Adam Block / Mount Lemmon SkyCenter / University of Arizona** &mdash;
  two photographs from Wikimedia Commons:
  - "FoxFur Nebula from the Mount Lemmon SkyCenter Schulman Telescope"
    (`images/FoxFur.jpg`):
    <https://commons.wikimedia.org/wiki/File:FoxFur_Nebula_from_the_Mount_Lemmon_SkyCenter_Schulman_Telescope_courtesy_Adam_Block.jpg>
  - "Cone Nebula from the Mount Lemmon SkyCenter Schulman Telescope"
    (`images/Cone.jpg`, the Target page's close-up):
    <https://commons.wikimedia.org/wiki/File:Cone_Nebula_from_the_Mount_Lemmon_SkyCenter_Schulman_Telescope_courtesy_Adam_Block.jpg>
  - **Licence:** Creative Commons Attribution-ShareAlike 4.0 International
    (CC BY-SA 4.0): <https://creativecommons.org/licenses/by-sa/4.0/>
  - **Changes:** scaled to fit 500 × 500 (Fox Fur from 1200 × 791 to 500 × 330,
    Cone from 900 × 949 to 474 × 500) and padded in black, like the app's other
    object images.
  - **Share-alike:** our modified copies, `FoxFur.jpg` and `Cone.jpg`, are offered
    under the same CC BY-SA 4.0 licence. It covers those images only, not the app.
- **Andreigusan** &mdash; the Iris Nebula (NGC 7023 and LBN 487), from Wikimedia
  Commons: <https://commons.wikimedia.org/wiki/File:Iris_Nebula_-_NGC_7023_-_Caldwell_4.jpg>.
  CC BY-SA 4.0. `images/NGC7023.jpg`, the close-up: cropped to the middle half of
  the frame (1973 × 1592 of 3946 × 2654), scaled to 500 × 403 and letterboxed; our
  copy is offered under the same licence. Jim McKee's Iris is `NGC7023-wide.jpg`.
- **David (Deddy) Dayag** &mdash; the Trifid Nebula (M20), from Wikimedia Commons:
  <https://commons.wikimedia.org/wiki/File:Trifid_Nebula_by_Deddy_Dayag.jpg>.
  CC BY-SA 4.0. `images/M20.jpg`: scaled from 3920 × 2822 to 500 × 360 and
  letterboxed; our copy is offered under the same licence.
- **ESO** &mdash; the Tarantula Nebula (NGC 2070), from Wikimedia Commons:
  <https://commons.wikimedia.org/wiki/File:NGC_2070_ESO.jpg> (from
  <https://www.eso.org/public/images/tarantula/>). Credit: ESO/IDA/Danish 1.5 m/R.
  Gendler, C. C. Thöne, C. Féron, and J.-E. Ovaldsen. Licence: Creative Commons
  Attribution 4.0 International (CC BY 4.0): <https://creativecommons.org/licenses/by/4.0/>.
  `images/NGC2070.jpg`: cropped from 1600 × 1200 to a square around the nebula and
  scaled to 500 × 500. It was in the app's first set of pictures without a credit;
  the user traced it to this image (10/2026).
- **Chuck Ayoub** &mdash; Omega Centauri (NGC 5139), "Omega Centauri Stars", from Wikimedia
  Commons: <https://commons.wikimedia.org/wiki/File:Omega_Centauri_Stars.png>. CC0 1.0.
  `images/NGC5139.jpg` (the Target page) is the middle of it; `images/NGC5139-wide.jpg`
  (the chart) is his whole frame, scaled from 2248 × 2248 to 1400 × 1400. Traced with
  `tools/image_credit_trace.py` (10/2026): the first set of pictures had no credit.
- **Chuck Ayoub** &mdash; M35 and NGC 2158, from Wikimedia Commons:
  <https://commons.wikimedia.org/wiki/File:M35_and_NGC_2158.png>. CC0 1.0.
  `images/M35.jpg` came with the app's first set of pictures, without a credit: turned
  about 99&deg;, cropped and colour-adjusted from his 2405 &times; 2092 frame, scaled to
  500 &times; 500, and since 11/2026 with a darker black point so it blends on the chart.
  Traced 11/2026 (a rotation search matched the star field).
- **Kevinmloch** &mdash; the Large Magellanic Cloud rendered from Gaia EDR3, from Wikimedia
  Commons: <https://commons.wikimedia.org/wiki/File:Large_Magellanic_Cloud_rendered_from_Gaia_EDR3.png>.
  CC BY-SA 4.0. `images/LMC.jpg` (the Target page): cropped to a square and scaled to
  500 × 500; our copy is offered under the same licence. Traced as above.
- **ESO/VMC Survey** &mdash; "The Large Magellanic Cloud revealed by VISTA" (eso1914a), from
  Wikimedia Commons: <https://commons.wikimedia.org/wiki/File:The_Large_Magellanic_Cloud_revealed_by_VISTA.jpg>.
  CC BY 4.0: <https://creativecommons.org/licenses/by/4.0/>. `images/LMC-wide.jpg` (the
  chart's wide field): from Commons' 3840 × 4289 rendering of the 28638 × 31985
  original, scaled to 1253 × 1400.
- **Fabian Rodriguez Frustaglia** &mdash; Messier 18, from Wikimedia Commons:
  <https://commons.wikimedia.org/wiki/File:Messier_18.jpg>. CC BY-SA 4.0.
  `images/M18.jpg`: scaled from 835 × 620 to 500 × 371 and letterboxed; our copy is
  offered under the same licence. It replaces an uncredited first-set picture.
- **ESO** &mdash; Messier 66, a colour composite from the VLT's FORS1 and FORS2 (eso0338c),
  from Wikimedia Commons: <https://commons.wikimedia.org/wiki/File:Phot-33c-03-fullres.jpg>.
  CC BY 4.0. `images/M66.jpg`: scaled from 4961 × 4965 to 500 × 500. Placed on the chart
  with ESO's own astrometry (the AVM metadata in the file). It replaces Spitzer's
  infrared M66.
- **NOIRLab/NSF/AURA** &mdash; Messier 14 (noao-m14), from Wikimedia Commons:
  <https://commons.wikimedia.org/wiki/File:Messier_14.jpg>. CC BY 4.0. `images/M14.jpg`:
  scaled from 2048 × 2048 to 500 × 500, placed with NOIRLab's AVM astrometry. It
  replaces an uncredited CC BY-SA 3.0 picture (Hewholooks).
- **NASA/Voyager 2, calibrated by Ardenau4** &mdash; Neptune in true colour ("Neptune Voyager2
  color calibrated"), from Wikimedia Commons:
  <https://commons.wikimedia.org/wiki/File:Neptune_Voyager2_color_calibrated.png>. CC0 1.0.
  `images/Neptune.jpg`: scaled from 1200 × 1200 to 500 × 500.
- **ESO** &mdash; Messier 61 face-on (potw1901a), from Wikimedia Commons:
  <https://commons.wikimedia.org/wiki/File:Messier61_-_ESO_-_Potw1901a.tif>. CC BY 4.0.
  `images/M61.jpg`: scaled from 1457 × 1486 to 490 × 500 and letterboxed; placed with
  ESO's AVM astrometry (`tools/imagescale/avm_place.py`).
- **RubinObs/NOIRLab/SLAC/NSF/DOE/AURA** &mdash; M61 with NGC 4301, from the Vera C. Rubin
  Observatory (noirlab2521ak), via Wikimedia Commons:
  <https://commons.wikimedia.org/wiki/File:Portion_of_Virgo_Cluster_(without_asteroids)_(noirlab2521ak).jpg>.
  CC BY 4.0. `images/M61-wide.jpg`: scaled from 2380 × 1810 to 1400 × 1065.
- **DESI Legacy Imaging Surveys/LBNL/DOE & KPNO/CTIO/NOIRLab/NSF/AURA** &mdash; Messier 96
  (noirlab2620a; processing M. Rodriguez, J. Miller, T.A. Rector, M. Zamani), via Wikimedia
  Commons: <https://commons.wikimedia.org/wiki/File:Messier_96_as_Seen_with_DESI_Legacy_Survey_(noirlab2620a).jpg>.
  CC BY 4.0. `images/M96.jpg`: scaled from 3000 × 3000 to 500 × 500. It replaces ESO/Oleg
  Maliy's M96 (CC BY 3.0).
- **Juan lacruz** &mdash; Messier 109 (NGC 3992), J87 Observatory, from Wikimedia Commons:
  <https://commons.wikimedia.org/wiki/File:M109_NGC_3992.png>. CC BY 4.0. `images/M109-wide.jpg`
  (the chart): scaled from 2998 × 2023 to 1400 × 945; `images/M109.jpg` (the Target page): a
  crop around the galaxy, 500 × 500. It replaces Hewholooks' M109 (CC BY-SA 3.0).
- **ESO/PESSTO/S. Smartt** &mdash; Messier 74, "PESSTO Snaps Supernova in Messier 74", from
  Wikimedia Commons: <https://commons.wikimedia.org/wiki/File:PESSTO_Snaps_Supernova_in_Messier_74.jpg>.
  CC BY 4.0. `images/M74.jpg`: scaled to 500 × 500. In the first set of pictures without a
  credit; traced with `tools/image_credit_trace.py` (10/2026).
- **NASA, ESA** &mdash; Arp 116, Messier 60 with NGC 4647, Hubble (heic1213a), from Wikimedia
  Commons: <https://commons.wikimedia.org/wiki/File:Arp116_Hubble.jpg>. CC BY 3.0:
  <https://creativecommons.org/licenses/by/3.0/>. `images/M60.jpg`: scaled from 7373 × 6220 to
  500 × 422 and letterboxed. Placed by matching its stars against a Legacy Survey DR10 cutout
  (it carries no AVM and is under the solver's 8′). It replaces an overexposed crop of the same
  picture that had no credit.
- **Public domain, traced to Wikimedia Commons** (`tools/image_credit_trace.py`, 10/2026), each
  scaled to 500 × 500: M9, 2MASS (UMass/IPAC-Caltech),
  <https://commons.wikimedia.org/wiki/File:Messier_object_009.jpg>; M58, NASA/JPL-Caltech
  (Spitzer), <https://commons.wikimedia.org/wiki/File:M58s.jpg>; NGC 3132, NASA, ESA, CSA, STScI
  (Webb NIRCam), <https://commons.wikimedia.org/wiki/File:Southern_Ring_Nebula_(NIRCam_Image).png>;
  NGC 6210, ESA/Hubble and NASA, <https://commons.wikimedia.org/wiki/File:NGC_6210_HST.tif>;
  Vesta, NASA/JPL-Caltech/UCLA/MPS/DLR/IDA (Dawn),
  <https://commons.wikimedia.org/wiki/File:Dawn_vesta_image_071711.jpg>.
- **ESO and others** &mdash; Centaurus A (NGC 5128), eso0903a: ESO/WFI (optical); MPIfR/ESO/APEX/
  A. Weiss et al. (submillimetre); NASA/CXC/CfA/R. Kraft et al. (X-ray). From Wikimedia Commons:
  <https://commons.wikimedia.org/wiki/File:ESO_Centaurus_A_LABOCA.jpg>. CC BY 4.0.
  `images/NGC5128.jpg`: scaled to 500 × 500.
- **Minnastronomer** &mdash; NGC 6910, the Inchworm Cluster ("Inchworm Cluster July 15 2025"), from
  Wikimedia Commons: <https://commons.wikimedia.org/wiki/File:Inchworm_Cluster_July_15_2025.png>.
  CC BY 4.0. `images/NGC6910.jpg` (the Target page): enlarged from 301 × 301 to 500 × 500 and
  lightly edited for presentation.
- **Yann Sainty** &mdash; the Seahorse Nebula (LDN 1082, Barnard 150), from Wikimedia
  Commons: <https://commons.wikimedia.org/wiki/File:Seahorse_nebula.png>.
  CC BY-SA 4.0. `images/LDN1082.jpg`, the close-up: scaled from 1996 × 3000 to
  333 × 500 and letterboxed; our copy is offered under the same licence.
  - Credited as "Adam Block, CC BY-SA 4.0" on the Target page and the chart.

---

## Planetary, solar, and lunar positions

Positions are computed from algorithms in:

> Jean Meeus, *Astronomical Algorithms*, 2nd ed., Willmann-Bell, 1998.

The mathematics is in the public domain; credit is retained here as a
courtesy to the author whose presentation made the implementation
practical.

---

## Comets, meteor showers, and Earth's position

**Comets.** Orbital elements: **IAU Minor Planet Center** (`CometEls.txt`,
<https://www.minorplanetcenter.net/iau/MPCORB/CometEls.txt>). The app downloads
the file and refreshes it weekly; nothing from it ships with the app. Comet
positions and estimated magnitudes are computed on the device from these
elements.

**Earth's position** for comet positions: the **VSOP87** planetary theory,
P. Bretagnon and G. Francou, *Astronomy and Astrophysics* 202, 309 (1988),
series VSOP87A as published by IMCCE (Paris Observatory), cut to its larger
terms (`tools/comets/vsop87_earth.py`).

**Meteor showers.** Shower dates, radiants, drift, speeds and rates come from
the **International Meteor Organization**'s Working List of Visual Meteor
Showers (<https://www.imo.net/>), built into a yearly file the app downloads.

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
improvements that enable Envision to run on Linux and
macOS hosts in addition to Windows.

---

## Software dependencies

Envision the Heavens&trade; depends on the following open-source
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

The Envision the Heavens&trade; application &mdash; Razor pages,
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

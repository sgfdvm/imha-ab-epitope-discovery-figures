# imha-ab-epitopediscovery-figures

Figures from a flow cytometry pilot for an IMHA immunoprecipitation study
(canine red blood cells incubated with IMHA serum 9030, healthy serum 9046, or no
serum; stained anti-dog IgG-biotin → streptavidin-PE; acquired 30 April 2026,
before and after hypotonic ghosting). Figures only; the analysis lives elsewhere.

**PE values are not comparable between pre-ghost (PE PMT 381–382 V) and
post-ghost test tubes (PE PMT 291 V).** Every figure keeps one voltage per axis.

Gates: pre-ghost "intact main" and post-ghost "tight cluster", each found per file
on log FSC-A × log SSC-A (except the 2026-09-27 common-gate figures, below). PE axes are arcsinh (cofactor 150) with raw-value ticks;
medians are raw values.

## Slide figures (1200 × 800 px, three panels: IMHA 9030 · Healthy 9046 · No serum)

| Figure | What it shows | Raw URL |
|---|---|---|
| FSC-A × PE-A, pre-ghost | intact cells; PE 382 V, FSC 450 V; gated events blue, median dashed | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/slide_density_PE-A-vs-FSC-A_pre-ghost_PE382V_144658.png |
| FSC-A × PE-A, post-ghost | ghosts; PE 291 V, FSC 500 V; gated events blue, median dashed | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/slide_density_PE-A-vs-FSC-A_post-ghost_PE291V_144658.png |
| SSC-A × PE-A, pre-ghost | intact cells; PE 382 V, SSC 240 V | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/slide_density_PE-A-vs-SSC-A_pre-ghost_PE382V_144658.png |
| SSC-A × PE-A, post-ghost | ghosts; PE 291 V, SSC 255 V | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/slide_density_PE-A-vs-SSC-A_post-ghost_PE291V_144658.png |
| FSC-A × SSC-A, pre-ghost | scatter with intact-main gate outlined; FSC 450 / SSC 240 V | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/slide_density_SSC-A-vs-FSC-A_pre-ghost_FSC450V-SSC240V_144658.png |
| FSC-A × SSC-A, post-ghost | scatter with tight-cluster gate outlined; FSC 500 / SSC 255 V | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/slide_density_SSC-A-vs-FSC-A_post-ghost_FSC500V-SSC255V_144658.png |
| PE histogram, pre-ghost | intact-main gate, three sera overlaid, PE 382 V | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/slide_PE_pre-ghost_382V_143930.png |
| PE histogram, post-ghost | tight-cluster gate, three sera overlaid, PE 291 V | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/slide_PE_post-ghost_291V_143930.png |

## Slide figures, FSC-A × PE-A, per-stage axes (2026-09-27, current)

| Figure | Raw URL |
|---|---|
| FSC-A × PE-A, pre-ghost (PE 382 V, FSC 450 V) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_PE-A-vs-FSC-A_pre-ghost_PE382V_commongate_stageaxes_124050.png |
| FSC-A × PE-A, post-ghost, events with FITC-A > 2,000 excluded (PE 291 V, FSC 500 V, FITC 432 V) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_PE-A-vs-FSC-A_post-ghost_PE291V_commongate_stageaxes_FITCgt2000excluded_124050.png |

These are presentation versions. The analysis itself still uses per-file gates; only
the display changes here.

- **Axes are set per stage.** The three panels within a stage share identical
  limits; the two stages do not share limits (and their PE and FSC voltages differ
  anyway). Each range is the union of the three tubes' 0.05–99.95 percentile spans of
  the plotted events, padded 6%. The FSC range is then widened about its centre, never
  narrowed, until a decade is the same length on both axes (the PE axis is arcsinh,
  so this holds above a few hundred). Events outside the range are drawn at the axis
  edge rather than dropped: pre-ghost 42 / 10 / 13, post-ghost 1 / 1 / 0.
  - Pre-ghost: FSC 10^3.56–10^6.09; PE about −1,300 to 26,000.
  - Post-ghost, after the exclusion: FSC 10^3.54–10^5.89; PE about −150 to 30,000.
- **One gate per stage.** Each stage has a single FSC/SSC gate, built from its three
  tubes pooled with equal weight using the same peak / watershed / 10%-of-peak rule as
  the per-file gates. Gated events are blue. The gate outlines are in the FSC × SSC
  figures listed in the superseded section below; the gates themselves are unchanged.
  Under each panel: gated events and their % of the events plotted.
- **One threshold per stage.** The dashed line is the no-serum tube's 95th percentile
  within the common gate, at the same height in all three panels of that stage: 152
  pre-ghost, 624 post-ghost (with the exclusion). The key is in the bottom-left corner,
  and headers show the gated median.
- **Post-ghost exclusion.** Events with FITC-A > 2,000 are dropped before the
  threshold, medians, gated counts, axis range and the plot are computed: 1,218 of 5,032
  events for IMHA (24.2%), 1,201 of 6,230 for healthy (19.3%) and 1,370 of 4,554 for no
  serum (30.1%). The bottom-right corner of the figure states this.
- **The FITC cut works as a PE ceiling.** In all three tubes, FITC/PE settles at 0.10
  for events brighter than about 10,000. That is consistent with uncompensated PE
  spilling into the FITC detector. Real anti-IgG / SA-PE staining of intact cells shows
  the same proportionality: 0.018–0.021 in the pre-ghost IMHA tube, at PE 382 V. So
  FITC-A > 2,000 works as a PE cap. The brightest event kept is PE 21,016 / 20,916 /
  21,733, and everything brighter is removed whatever it is. The case for treating
  these events as non-antibody is that they are most frequent in the no-serum tube,
  not their FITC/PE ratio.

Post-ghost, common gate, with and without the exclusion. The line is the no-serum 95th
percentile within the gate: 102,295 without the exclusion, 624 with it.

| Tube | Median, all events | Median, excluded | % above line, all events | % above line, excluded |
|---|---|---|---|---|
| IMHA 9030 | 304 | 288 | 0.1 | 8.3 |
| Healthy 9046 | 260 | 254 | 0.4 | 4.0 |
| No serum | 271 | 182 | 5.0 | 5.0 |

Pre-ghost, common gate (no exclusion; FITC-A > 2,000 is at most 3 events per
pre-ghost tube). The line is 152.

| Tube | Gated (%) | Median | % above line |
|---|---|---|---|
| IMHA 9030 | 132,743 (66.4) | 428 | 62.9 |
| Healthy 9046 | 131,912 (66.0) | −4 | 6.4 |
| No serum | 136,559 (68.3) | 11 | 5.0 |

**Why the post-ghost no-serum median is 271 with the pooled gate and 203 with the
per-file gate.** The pooled gate takes in more of the bright component than the
per-file gate did. Of the no-serum tube's gated events, 176 of 773 in the pooled gate
have FITC-A > 2,000, against 68 of 633 in the per-file gate. With those events
excluded, the two medians are 182 (pooled) and 173 (per-file).

Common gate compared with per-file gate, all events, both stages:

| Stage | Tube | Gated, common | Gated, per-file | Median, common | Median, per-file |
|---|---|---|---|---|---|
| pre-ghost, 382 V | IMHA 9030 | 132,743 | 131,917 | 428 | 424 |
| pre-ghost, 382 V | Healthy 9046 | 131,912 | 131,830 | −4 | −4 |
| pre-ghost, 382 V | No serum | 136,559 | 137,825 | 11 | 11 |
| post-ghost, 291 V | IMHA 9030 | 1,447 | 1,366 | 304 | 302 |
| post-ghost, 291 V | Healthy 9046 | 2,576 | 2,338 | 260 | 258 |
| post-ghost, 291 V | No serum | 773 | 633 | 271 | 203 |

## Superseded 2026-09-27 versions (one axis range across both stages)

These use a single FSC, SSC and PE range for all panels of both stages. The
post-ghost bright component reaches 2.7 × 10⁷, which pushed the PE ceiling to 10⁷ for
the pre-ghost panels too and left most of each plot empty. The FSC × SSC figures are
still the reference for what the common gates look like.

| Figure | Raw URL |
|---|---|
| FSC-A × PE-A, pre-ghost | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_PE-A-vs-FSC-A_pre-ghost_PE382V_commongate_sharedaxes_122903.png |
| FSC-A × PE-A, post-ghost, all events | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_PE-A-vs-FSC-A_post-ghost_PE291V_commongate_sharedaxes_122903.png |
| FSC-A × PE-A, post-ghost, FITC-A > 2,000 excluded | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_PE-A-vs-FSC-A_post-ghost_PE291V_commongate_sharedaxes_FITCgt2000excluded_123643.png |
| FSC-A × SSC-A, pre-ghost, common gate outlined (FSC 450 / SSC 240 V) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_SSC-A-vs-FSC-A_pre-ghost_FSC450V-SSC240V_commongate_sharedaxes_122903.png |
| FSC-A × SSC-A, post-ghost, common gate outlined, all events (FSC 500 / SSC 255 V) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_SSC-A-vs-FSC-A_post-ghost_FSC500V-SSC255V_commongate_sharedaxes_122903.png |

## Analysis figures

| Figure | What it shows | Raw URL |
|---|---|---|
| Scatter gates, all 10 tubes | FSC-A × SSC-A per file with every population found; voltages in panel titles | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_scatter_gates_113244.png |
| PE histograms, 381–382 V | pre-ghost intact cells incl. unstained and SA-PE-only; post-ghost controls in a separate panel | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_PE_381-382V_113244.png |
| PE histograms, 291 V | post-ghost tight cluster and low-FSC cloud, three sera | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_PE_291V_113244.png |
| Follow-up 1 | pulse width and FSC: tight cluster vs intact cells (ghosts vs beads check) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_followup1_width_115600.png |
| Follow-up 2 | events just above the FSC threshold; FITC × PE of the low-FSC cloud at 291 V | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_followup2_low_cloud_115600.png |
| Follow-up 3 | pre-ghost IMHA events with PE < −200: over acquisition time, scatter, pulse width | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_followup3_negatives_115600.png |

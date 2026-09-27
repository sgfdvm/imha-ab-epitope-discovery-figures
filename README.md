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

## Slide figures, common gate and shared axes (2026-09-27)

Presentation versions of the FSC-A × PE-A figures. The analysis itself still uses
per-file gates; these figures change only how the data are displayed.

- **Shared axes.** All 12 panels across the four figures use the same axis limits:
  FSC-A 10^3.57–10^7.02, SSC-A 10^3.20–10^6.56, and PE-A −2.84 to 12.81 in arcsinh(x/150)
  display units, which is about −1,300 to 2.7 × 10^7. Each range is the union of the six
  tubes' 0.05–99.95 percentile spans, padded 3%. Events outside the range are drawn at
  the axis edge rather than dropped:
  - FSC × PE: pre 29 / 6 / 10, post 2 / 4 / 0
  - FSC × SSC: pre 64 / 41 / 17, post 3 / 4 / 2
- **PE voltages still differ.** The PE axis has the same limits in both stages, but the
  PMT voltage is not the same: 382 V pre-ghost and 291 V post-ghost, as the y-axis label
  says. **Do not compare PE heights across the two figures.**
- **One gate per stage.** Each stage has a single FSC/SSC gate, built from its three tubes
  pooled with equal weight using the same peak / watershed / 10%-of-peak rule as the
  per-file gates. The gate is outlined in the FSC × SSC figures and appears as blue
  events in the PE figures. Under each panel: gated events and their % of all events.
- **One threshold per stage.** The dashed line is the no-serum tube's 95th percentile
  within the common gate, at the same height in every panel of that stage. Headers
  show the gated median.

| Figure | Raw URL |
|---|---|
| FSC-A × PE-A, pre-ghost (PE 382 V, FSC 450 V) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_PE-A-vs-FSC-A_pre-ghost_PE382V_commongate_sharedaxes_122903.png |
| FSC-A × PE-A, post-ghost (PE 291 V, FSC 500 V) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_PE-A-vs-FSC-A_post-ghost_PE291V_commongate_sharedaxes_122903.png |
| FSC-A × SSC-A, pre-ghost, common gate outlined (FSC 450 / SSC 240 V) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_SSC-A-vs-FSC-A_pre-ghost_FSC450V-SSC240V_commongate_sharedaxes_122903.png |
| FSC-A × SSC-A, post-ghost, common gate outlined (FSC 500 / SSC 255 V) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_SSC-A-vs-FSC-A_post-ghost_FSC500V-SSC255V_commongate_sharedaxes_122903.png |

Common gate compared with per-file gate. Medians are raw PE values. The threshold is
the no-serum 95th percentile within the common gate: 152 pre-ghost, 102,295 post-ghost.

| Stage | Tube | Gated, common (%) | Gated, per-file | Median, common | Median, per-file | % above threshold |
|---|---|---|---|---|---|---|
| pre-ghost, 382 V | IMHA 9030 | 132,743 (66.4) | 131,917 | 428 | 424 | 62.9 |
| pre-ghost, 382 V | Healthy 9046 | 131,912 (66.0) | 131,830 | −4 | −4 | 6.4 |
| pre-ghost, 382 V | No serum | 136,559 (68.3) | 137,825 | 11 | 11 | 5.0 |
| post-ghost, 291 V | IMHA 9030 | 1,447 (28.8) | 1,366 | 304 | 302 | 0.1 |
| post-ghost, 291 V | Healthy 9046 | 2,576 (41.3) | 2,338 | 260 | 258 | 0.4 |
| post-ghost, 291 V | No serum | 773 (17.0) | 633 | **271** | **203** | 5.0 |

The post-ghost threshold (102,295) is set by a bright component, not by background
staining. 176 of the 773 gated no-serum events (23%) belong to that component
(FITC-A > 2,000), and it also appears in the serum tubes. The line therefore marks
the edge of that component rather than a cutoff for antibody binding. The next
figure excludes the component.

**Why the post-ghost no-serum median is 271 with the pooled gate and 203 with the
per-file gate.** The pooled gate takes in more of the bright component than the
per-file gate did. Of the no-serum tube's gated events, 176 of 773 in the pooled
gate have FITC-A > 2,000, against 68 of 633 in the per-file gate. With those events
excluded, the two medians are 182 (pooled) and 173 (per-file).

### Post-ghost FSC-A × PE-A with the bright component excluded

| Figure | Raw URL |
|---|---|
| FSC-A × PE-A, post-ghost, events with FITC-A > 2,000 excluded (PE 291 V, FSC 500 V, FITC 432 V) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-27/slide_density_PE-A-vs-FSC-A_post-ghost_PE291V_commongate_sharedaxes_FITCgt2000excluded_123643.png |

- **What was excluded.** Events with FITC-A > 2,000 are dropped before the threshold,
  medians, gated counts and the plot are computed: 1,218 of 5,032 events for IMHA
  (24.2%), 1,201 of 6,230 for healthy (19.3%) and 1,370 of 4,554 for no serum (30.1%).
  The note in the bottom-right corner of the figure says so.
- **What stays the same.** The common gate and the shared axes are unchanged; the
  gate is the one built from all events and outlined in the post-ghost FSC × SSC
  figure above. Gated % under each panel is of the events left after exclusion.
- **The cut works as a PE ceiling.** In all three tubes, FITC/PE settles at 0.10 for
  events brighter than about 10,000. That is consistent with uncompensated PE
  spilling into the FITC detector. Real anti-IgG / SA-PE staining of intact cells
  shows the same proportionality: 0.018–0.021 in the pre-ghost IMHA tube, at PE
  382 V. So FITC-A > 2,000 works as a PE cap. The brightest event kept is PE 21,016 /
  20,916 / 21,733, and everything brighter is removed whatever it is. The case for
  treating these events as non-antibody is that they are most frequent in the
  no-serum tube, not their FITC/PE ratio.

Common gate, with and without the exclusion. The line is the no-serum 95th
percentile within the gate: 102,295 without the exclusion, 624 with it.

| Tube | Median, all events | Median, excluded | % above line, all events | % above line, excluded |
|---|---|---|---|---|
| IMHA 9030 | 304 | 288 | 0.1 | 8.3 |
| Healthy 9046 | 260 | 254 | 0.4 | 4.0 |
| No serum | 271 | 182 | 5.0 | 5.0 |

## Analysis figures

| Figure | What it shows | Raw URL |
|---|---|---|
| Scatter gates, all 10 tubes | FSC-A × SSC-A per file with every population found; voltages in panel titles | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_scatter_gates_113244.png |
| PE histograms, 381–382 V | pre-ghost intact cells incl. unstained and SA-PE-only; post-ghost controls in a separate panel | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_PE_381-382V_113244.png |
| PE histograms, 291 V | post-ghost tight cluster and low-FSC cloud, three sera | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_PE_291V_113244.png |
| Follow-up 1 | pulse width and FSC: tight cluster vs intact cells (ghosts vs beads check) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_followup1_width_115600.png |
| Follow-up 2 | events just above the FSC threshold; FITC × PE of the low-FSC cloud at 291 V | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_followup2_low_cloud_115600.png |
| Follow-up 3 | pre-ghost IMHA events with PE < −200: over acquisition time, scatter, pulse width | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_followup3_negatives_115600.png |

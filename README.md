# imha-ab-epitopediscovery-figures

Figures from a flow cytometry pilot for an IMHA immunoprecipitation study
(canine red blood cells incubated with IMHA serum 9030, healthy serum 9046, or no
serum; stained anti-dog IgG-biotin → streptavidin-PE; acquired 30 April 2026,
before and after hypotonic ghosting). Figures only; the analysis lives elsewhere.

**PE values are not comparable between pre-ghost (PE PMT 381–382 V) and
post-ghost test tubes (PE PMT 291 V).** Every figure keeps one voltage per axis.

Gates: pre-ghost "intact main" and post-ghost "tight cluster", each found per file
on log FSC-A × log SSC-A. PE axes are arcsinh (cofactor 150) with raw-value ticks;
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

## Analysis figures

| Figure | What it shows | Raw URL |
|---|---|---|
| Scatter gates, all 10 tubes | FSC-A × SSC-A per file with every population found; voltages in panel titles | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_scatter_gates_113244.png |
| PE histograms, 381–382 V | pre-ghost intact cells incl. unstained and SA-PE-only; post-ghost controls in a separate panel | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_PE_381-382V_113244.png |
| PE histograms, 291 V | post-ghost tight cluster and low-FSC cloud, three sera | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_PE_291V_113244.png |
| Follow-up 1 | pulse width and FSC: tight cluster vs intact cells (ghosts vs beads check) | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_followup1_width_115600.png |
| Follow-up 2 | events just above the FSC threshold; FITC × PE of the low-FSC cloud at 291 V | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_followup2_low_cloud_115600.png |
| Follow-up 3 | pre-ghost IMHA events with PE < −200: over acquisition time, scatter, pulse width | https://raw.githubusercontent.com/sgfdvm/imha-ab-epitopediscovery-figures/main/figures/2026-09-26/ip_pilot_followup3_negatives_115600.png |

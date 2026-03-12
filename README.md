# Ground Reality — City Index

A liveability index for 51 cities across 6 regions, built as a considered argument rather than an algorithm. Every score is a position, not a calculation from a spreadsheet.

Currently covers **South Asia (22), East Asia (6), Africa (4), Europe (7), North America (8), and Latin America (4)**. More cities will be added in future versions.

Live at: **[nadika-nadja.github.io/city-index](https://nadika-nadja.github.io/city-index)**

---

## What it measures

Eight scored dimensions at equal weight, plus Ecology and Climate at half weight each:

- **Transport** — network coverage, cost as a fraction of minimum wage, first/last mile, all-class access
- **Public Space** — free access, walking distance, shade, class diversity of actual users
- **Cleanliness** — visible hygiene, drain function, waste management in non-showcase areas
- **Cost vs Life** — PPP-adjusted median rent/wage ratio, public healthcare, food, schooling
- **Economy** — Scale (size, depth, global reach) + Resilience (sector diversity, shock absorption)
- **Leisure** — entertainment breadth and access across income levels
- **Openness** — women's safety, minority experience, LGBTQ+ rights, press freedom, social mixing
- **Heritage** — civilisational depth, continuity, living vs museum quality; bias-corrected for systematic undervaluation of Dravidian and non-Mughal South Asian heritage

**🌿 Ecology (½ weight)** — river and water body health, groundwater trajectory, green cover change, annual PM2.5 burden. Scored on present reality, not historical audit.

**🌦 Climate (½ weight, from v7a)** — Present Liveability (monthly temperature and humidity burden, wildfire smoke, flood disruption) and Trajectory (direction of travel over 20 years: sea level risk, groundwater stress, temperature trend). Government policy scoring comes in v7b.

### Score formula

```
total = ((8 × base_score) + (0.5 × ecology) + (0.5 × climate)) / 9.0

base_score = mean of 8 dimensions
economy    = (Scale + Resilience) / 2
climate    = (present_liveability + trajectory) / 2
```

---

## Views

- **List** — expandable city cards with verdict, marketing gap analysis, and per-dimension notes
- **Heatmap** — full 51-city colour matrix across all dimensions
- **Climate** — climate-focused grid sorted by climate score, with monthly temperature charts
- **Scatter** — plot any two dimensions against each other
- **Regions** — centroid averages by region

---

## A note on methodology

Scores are argued positions. Heritage is corrected for the systematic bias in standard rankings that overweight Mughal-era aesthetics and photogenic tourism sites. Openness is scored on lived experience, not legal frameworks alone — Paris's laïcité friction and Delhi's minority targeting are scored alongside Amsterdam's genuine record. Ecology and climate scores carry a colonial context note: the worst present scores and worst trajectories are concentrated in post-colonial cities for reasons that are not accidental, even though present residents breathe present air regardless of historical cause.

The Marketing Gap indicator (Low / Medium / High) flags where a city's promotional narrative diverges most from the ground reality the index is trying to describe.

---

## Version history

| Version | Cities | What changed |
|---------|--------|-------------|
| v1–v4 | 22 | Indian city index, methodology developed |
| v5a | 32 | Expanded to Asia + Africa |
| v5b | 19 | Europe + Americas |
| v6 | 51 | Combined global index, scatter and centroid views added |
| v7a | 51 | Climate dimension added: present liveability + trajectory |
| v7b | 51 | Government climate policy scoring *(planned)* |
| v8 | 51 | Multi-region comparison mode *(planned)* |

Older versions are preserved in the repository and accessible at their own URLs (e.g. `v6.html`).

---

## Planned

- Government climate policy scoring (v7b)
- Multi-region comparison mode — select South Asia + East Asia, South Asia + Europe, etc. (v8)
- Additional cities across all regions in future versions — the index is intentionally incomplete and will grow
- Climate policy dimension
- Eventually: how built environment (transit, shade, public space design) mitigates climate effects — the question of what a city can actually *do* about the weather it has

---

*Scores reflect conditions as of early 2026. This is a living index.*

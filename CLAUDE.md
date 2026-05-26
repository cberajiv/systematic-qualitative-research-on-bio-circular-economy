# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **Claude Code skill** (`SKILL.md`) for conducting systematic qualitative research on **Circular Bio Economy initiatives** — organizations that take biological waste or byproducts as inputs and produce high-value goods, energy, or materials through biological or standard physicochemical treatment. The defining principle is closing the biological loop: turning waste into value while minimizing residual waste. It provides structured methodology for identifying, classifying, and analyzing 25+ such initiatives using the Quintuple Helix framework.

## Skill Invocation

This skill is invoked when users need to:
- Research 20+ Circular Bio Economy initiatives (biological waste/byproduct → high-value output)
- Classify organizations by Quintuple Helix actor type (G/I/A/C/E) within the Circular Bio Economy ecosystem
- Produce structured JSON research databases for thesis or policy work on Circular Bio Economy
- Build interactive dashboards for stakeholder presentations on Circular Bio Economy pathways

## Core Frameworks

### Quintuple Helix Classification
Five actor types identify institutional roles in innovation ecosystems:
- **G** — Government (policy bodies, regulatory agencies, public subsidies)
- **I** — Industry (private companies, social enterprises, commercial ventures)
- **A** — Academia (universities, research institutes, technical training)
- **C** — Civil Society (NGOs, community organizations, women's groups)
- **E** — Environment (environmental NGOs, ecosystem stewardship, carbon programs)

Classifications combine actors: `G-I`, `I-C-E`, `G-I-C-E`, etc. More actors = more coordinated ecosystem. See `references/quintuple-helix-guide.md` for the decision tree.

### Sector Taxonomy (Circular Bio Economy)
Eight sectors defined in `references/sector-taxonomy.md`: Biogas/Bio-Energy, Composting, Waste Valorization, Biorefining, Alternative Materials, Bio-Products, Waste-to-Feed/Food, Multi-Pathway. Each sector has defined key processes, typical actors, and expected public content levels.

### Coordination State
Three states: **Formal** (documented partnerships/MOUs), **Informal** (loose networks), **Isolated** (standalone operation). Single-actor initiatives are typically Isolated; 3+ actor initiatives are typically Formal.

### Public Content Level
Six levels (Very High → Low) that assess documentation availability for qualitative analysis. Minimum recommended for thesis analysis: Medium-High.

## Data Structure

Each researched initiative follows this JSON schema (all fields defined in `SKILL.md`):

```json
{
  "id": 1, "name": "", "type": "", "location": "", "pathway": "", "pathwayLabel": "",
  "established": 2011, "inputs": "", "outputs": "", "keyFact": "",
  "evidenceStrength": 5, "sources": [], "sourceUrls": [], "newsLinks": [],
  "co2": null, "jobs": null, "womenPct": null, "wasteHandled": null,
  "description": "200-300 word narrative",
  "quintuple_helix": "I-C-E", "sector": "composting",
  "coordination_state": "Formal", "public_content_level": "High"
}
```

## Research Workflow

Five phases (detailed in `references/research-protocol.md`):
1. **Planning** — Define domain, target 25+ initiatives, set minimum content level
2. **Identification** — Web, YouTube, government portals, NGO directories, academic DBs, social media
3. **Data Extraction** — Fill all JSON fields; minimum 2–3 independent sources per initiative
4. **Verification** — Check official website, news, academic papers, video, government records, social media
5. **Synthesis** — JSON database → interactive dashboard (React/Vue) with filters and visualizations

Recursive search is critical: when finding one initiative, extract partner/competitor names and search each separately.

## Reference Files

- `references/research-protocol.md` — Search query templates, extraction checklists, QA process, reporting metrics
- `references/quintuple-helix-guide.md` — Actor definitions with examples and classification decision tree
- `references/sector-taxonomy.md` — Eight sector definitions with processes, actors, impact metrics, and examples

## Scripts & Templates

- `scripts/example.py` — Placeholder; replace with data validation or report generation scripts
- `templates/example_template.txt` — Placeholder; replace with React component or HTML dashboard templates

## Dashboard Output

The end deliverable is an interactive HTML/React dashboard with:
- Filterable project cards (by Quintuple Helix, sector, coordination state, content level)
- Visualizations: bar charts (sector distribution), pie charts (actor involvement), radar charts
- Clickable news/media links per initiative
- CSV export for thesis bibliography
- Timeline of establishment dates and media coverage

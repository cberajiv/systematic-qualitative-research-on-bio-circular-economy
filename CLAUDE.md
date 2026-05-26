# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **Claude Code skill** (`SKILL.md`) for conducting systematic qualitative research on **Circular Bio Economy (CBE) initiatives** — organizations that take biological waste or byproducts as inputs and produce high-value goods, energy, or materials through biological or standard physicochemical treatment. The defining principle is closing the biological loop: turning waste into value while minimizing residual waste. It provides structured methodology for identifying, classifying, and analyzing 25+ such initiatives using the Quintuple Helix framework.

The skill supports a thesis investigating how fragmented CBE activities in Nepal can be understood, analyzed, and coordinated through orchestration mechanisms to support ecosystem emergence under conditions of limited state capacity. Comprehensive initiative mapping is the foundation; the mapped data is then used to identify barriers, analyze coordination gaps, and propose a context-sensitive orchestration model.

## Skill Invocation

This skill is invoked when users need to:
- Research 25+ Circular Bio Economy initiatives (biological waste/byproduct → high-value output)
- Classify organizations by Quintuple Helix actor type (G/I/A/C/E) within the CBE ecosystem
- Identify barriers constraining CBE activities (financial, policy, capacity)
- Analyze coordination gaps and orchestration potential of actors
- Produce structured JSON research databases for thesis or policy work on Circular Bio Economy
- Build an interactive dashboard as an intermediary visualization tool during the research process

## Core Frameworks

### Quintuple Helix Classification
Five actor types identify institutional roles in innovation ecosystems:
- **G** — Government (policy bodies, regulatory agencies, public subsidies)
- **I** — Industry (private companies, social enterprises, commercial ventures)
- **A** — Academia (universities, research institutes, technical training — as **active participants** in CBE initiatives, not merely sources of academic literature)
- **C** — Civil Society (NGOs, community organizations, women's groups)
- **E** — Environment (environmental NGOs, ecosystem stewardship, carbon programs)

Classifications combine actors: `G-I`, `I-C-E`, `G-I-C-E`, etc. More actors = more coordinated ecosystem. See `references/quintuple-helix-guide.md` for the decision tree.

### Sector Taxonomy (Circular Bio Economy)
Eight sectors defined in `references/sector-taxonomy.md`: Biogas/Bio-Energy, Composting, Waste Valorization, Biorefining, Alternative Materials, Bio-Products, Waste-to-Feed/Food, Multi-Pathway. Each sector has defined key processes, typical actors, and expected public content levels.

### Coordination and Barriers
Both are captured as **free-text observations** during data collection — extracted or paraphrased from publicly available sources (news, reports, websites, videos). Categorization happens inductively during the analysis stage (Mayring, 2014), not at data entry time.

- `barriers` — list of observed constraints as described in source content; later coded into financial / policy / capacity categories
- `coordination` — list of observed relationships or their absence; later coded to identify coordination gaps, actor roles, and orchestration potential

No pre-set labels are applied at collection time. Patterns and categories emerge from the coded content.

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
  "public_content_level": "High",
  "barriers": ["Observed barrier from source content"],
  "barriers_coded": [{ "observation": "...", "category": "..." }],
  "coordination": ["Observed coordination relationship from source content"],
  "coordination_coded": [{ "observation": "...", "category": "..." }]
}
```

## Research Workflow

Five phases (detailed in `references/research-protocol.md`):
1. **Planning** — Define geography, pathway scope, time horizon, document sampling strategy
2. **Identification** — Two complementary source types: (a) web/media (web search, YouTube, news, social media) and (b) institutional/document (government portals and policy docs, NGO/INGO reports, academic databases, private sector reports)
3. **Data Extraction** — Fill all JSON fields; minimum 2–3 independent sources per initiative
4. **Verification** — Cross-check across official website, news, academic papers, video, government records, social media
5. **Synthesis** — JSON database → interactive dashboard (React/Vue) as an intermediary visualization tool to explore patterns and refine data before barrier and coordination gap analysis

Recursive search is critical: when finding one initiative, extract partner/competitor names and search each separately.

## Reference Files

- `references/research-protocol.md` — Search query templates, extraction checklists, QA process, reporting metrics
- `references/quintuple-helix-guide.md` — Actor definitions with examples and classification decision tree
- `references/sector-taxonomy.md` — Eight sector definitions with processes, actors, impact metrics, and examples

## Scripts & Templates

- `scripts/example.py` — Placeholder; replace with data validation or report generation scripts
- `templates/example_template.txt` — Placeholder; replace with React component or HTML dashboard templates

## Dashboard Output

The interactive HTML/React dashboard is an **intermediary research tool**, not the final deliverable. It makes the initiative database explorable during data collection and helps surface patterns (sector gaps, actor dominance, coordination weaknesses) that feed subsequent analysis stages.

Features:
- Filterable project cards (by Quintuple Helix, sector, coordination state, content level)
- Visualizations: bar charts (sector distribution), pie charts (actor involvement), radar charts
- Clickable news/media links per initiative
- CSV export for thesis bibliography
- Timeline of establishment dates and media coverage

The dashboard feeds into — but does not replace — barrier identification, coordination gap analysis, orchestration potential evaluation, and model development, which are the core thesis outputs.

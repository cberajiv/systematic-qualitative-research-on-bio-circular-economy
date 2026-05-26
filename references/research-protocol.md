# Research Protocol: Qualitative Circular Bio Economy Research

This document provides step-by-step guidance for conducting comprehensive research on Circular Bio Economy initiatives — organizations that convert biological waste or byproducts into high-value goods, energy, or materials through biological or standard physicochemical treatment.

## Search Query Templates

### Phase 1: Domain-Specific Web Search

Use these search patterns to identify initiatives:

**Circular Bio Economy pathway searches:**
- `"{pathway} {geography}"` (e.g., "biogas Nepal", "biorefining India", "composting companies Nepal")
- `"{pathway} companies {geography}"` (e.g., "waste valorization companies Nepal", "Circular Bio Economy companies Nepal")
- `"{pathway} organizations {geography}"` (e.g., "biorefining organizations Nepal")
- `"biological waste valorization {geography}"` (e.g., "biological waste valorization Nepal")
- `"Circular Bio Economy {geography}"` (e.g., "Circular Bio Economy Nepal")

**Government searches:**
- `"site:.gov.np {sector}"` (e.g., "site:.gov.np biogas")
- `"{ministry} {sector} {geography}"` (e.g., "Ministry of Science Technology biogas Nepal")
- `"{sector} policy {geography}"` (e.g., "waste management policy Nepal")

**NGO/INGO searches:**
- `"NGO {sector} {geography}"` (e.g., "NGO waste management Nepal")
- `"INGO {sector} {geography}"` (e.g., "INGO biogas Nepal")
- `"{sector} sector partnership {geography}"` (e.g., "biogas sector partnership Nepal")

**Academic searches:**
- `"site:mdpi.com {sector} {geography}"` (e.g., "site:mdpi.com circular economy Nepal")
- `"site:researchgate.net {sector} {geography}"`
- `"{sector} research {geography}"` (e.g., "biorefining research Nepal")

### Phase 2: YouTube & Video Search

Search for local language documentation:

- `"{local language} {sector}"` (e.g., "नेपाली बायोगास", "Nepali biogas")
- `"{sector} documentary {geography}"` (e.g., "biogas documentary Nepal")
- `"{sector} project video {geography}"` (e.g., "waste management project video Nepal")
- `"{local youtuber} {sector}"` (e.g., "Nepali youtuber biogas")

### Phase 3: News & Media Search

Find media coverage:

- `"{initiative name}" news` (e.g., "Biocomp Nepal news")
- `"{sector} news {geography}"` (e.g., "biogas news Nepal")
- `"{sector} {geography} 2024"` (e.g., "circular economy Nepal 2024")
- `"{sector} {geography} case study"` (e.g., "waste valorization Nepal case study")

### Phase 4: Social Media & Directory Search

Identify emerging initiatives:

- `"site:facebook.com {sector} {geography}"`
- `"site:linkedin.com {sector} {geography}"`
- `"{sector} directory {geography}"` (e.g., "biogas directory Nepal")
- `"{sector} association {geography}"` (e.g., "biogas association Nepal")

## Data Extraction Checklist

For each initiative, verify you have extracted:

### Basic Information
- [ ] Official name
- [ ] Organization type (Private, NGO, Government, INGO, Academic)
- [ ] Location (city, region, country)
- [ ] Year established
- [ ] Primary contact/founder names

### Technical Information
- [ ] Primary feedstock/inputs
- [ ] Primary outputs/products
- [ ] Technology/process used
- [ ] Capacity/scale (if available)
- [ ] Key distinguishing features

### Institutional Information
- [ ] Quintuple Helix classification (G, I, A, C, E)
- [ ] Coordination state (Formal, Informal, Isolated)
- [ ] Key partnerships (if any)
- [ ] Funding sources (if available)

### Impact Metrics
- [ ] CO₂ reduction/year (if applicable)
- [ ] Jobs created
- [ ] Women participation %
- [ ] Waste handled/year (if applicable)
- [ ] Other relevant metrics

### Content Assessment
- [ ] Public content level (Very High, High, Medium-High, Medium, Low-Medium, Low)
- [ ] Evidence strength (1-5 confidence rating)
- [ ] Primary sources (minimum 2-3)
- [ ] News/media links (minimum 3-5 if available)
- [ ] YouTube documentation (if available)

### Documentation
- [ ] 200-300 word description written
- [ ] All source URLs documented
- [ ] All news links documented
- [ ] Verification completed

## Content Verification Process

For each initiative, follow this verification process:

### Step 1: Official Website Verification
1. Search for official website
2. Extract: name, location, established date, mission statement
3. Document: website URL, last accessed date
4. Rate content quality: Does website provide sufficient information? (Yes/No)

### Step 2: News Coverage Search
1. Search: `"{initiative name}" news`
2. Search: `"{sector}" "{location}" news`
3. Collect: minimum 3-5 news articles
4. Document: article title, source, URL, publication date
5. Extract: key facts, impact metrics, partnerships mentioned

### Step 3: Academic Documentation
1. Search MDPI, ResearchGate, SSRN for papers mentioning initiative
2. Collect: case studies, research papers, reports
3. Document: paper title, authors, URL, publication date
4. Extract: methodology, findings, impact assessment

### Step 4: Video Documentation
1. Search YouTube for initiative videos
2. Collect: project videos, documentaries, interviews
3. Document: video title, channel, URL, publication date
4. Extract: key information from video descriptions and comments

### Step 5: Government/NGO Records
1. Search government databases (.gov.np, ministry websites)
2. Search NGO directories (REC Nepal, Clean Cooking Alliance, etc.)
3. Collect: project reports, policy documents, partnership records
4. Document: source, URL, publication date

### Step 6: Social Media Verification
1. Search Facebook, LinkedIn, Instagram
2. Collect: official pages, follower count, post frequency
3. Document: social media handles, follower metrics
4. Extract: recent updates, partnerships, announcements

## Quality Assurance Checklist

Before finalizing each initiative record:

- [ ] Name matches across all sources (verify spelling)
- [ ] Location is specific (city/region, not just country)
- [ ] Established date is consistent across sources
- [ ] Sector classification is accurate (matches primary activity)
- [ ] Quintuple Helix classification includes all involved actors
- [ ] At least 3 independent sources confirm key facts
- [ ] All URLs are active and accessible
- [ ] Description is 200-300 words and grammatically correct
- [ ] Evidence strength rating is justified (1-5)
- [ ] Public content level is accurate (Very High to Low)
- [ ] No duplicate initiatives in database

## Recursive Search Protocol

When you discover an initiative, search for related initiatives:

1. **Extract partner names** from initiative description/website
2. **Search for each partner** as separate initiative
3. **Extract competitor/similar names** from news articles
4. **Search for each competitor** as separate initiative
5. **Repeat** until no new initiatives are discovered

This recursive approach helps identify hidden initiatives and ecosystem clusters.

## Database Compilation

Once all initiatives are researched:

1. **Create JSON file** with all initiative records
2. **Validate JSON** for syntax errors
3. **Check for duplicates** (same initiative with different names)
4. **Verify counts** (25+ initiatives minimum)
5. **Backup database** (multiple copies)
6. **Create CSV export** for spreadsheet analysis

## Reporting Metrics

Calculate these metrics for your research report:

- **Total initiatives researched:** Count
- **By organization type:** Private, NGO, Government, INGO, Academic (breakdown)
- **By Quintuple Helix:** G, I, A, C, E involvement (breakdown)
- **By sector:** Distribution across sectors
- **By coordination state:** Formal, Informal, Isolated (breakdown)
- **By public content level:** Very High to Low (breakdown)
- **Average evidence strength:** Mean confidence rating
- **Total CO₂ reduction:** Sum of documented reductions
- **Total jobs created:** Sum of documented jobs
- **Geographic distribution:** By city/region
- **Timeline:** Initiatives by establishment year

## Timeline for Research

Recommended timeline for comprehensive research:

- **Week 1:** Research planning, domain scoping, initial web searches (5-10 initiatives)
- **Week 2:** YouTube & video research, recursive searches (10-15 initiatives)
- **Week 3:** News & media verification, government records (15-20 initiatives)
- **Week 4:** Academic documentation, social media verification (20-25+ initiatives)
- **Week 5:** Quality assurance, duplicate removal, database compilation
- **Week 6:** Visualization creation, gap analysis, final report

This timeline assumes 10-15 hours per week of research effort.

# Graph Report - G:/0.cslab.ai/005.content-ops-workspace/reports  (2026-04-06)

## Corpus Check
- Corpus is ~6,799 words - fits in a single context window. You may not need a graph.

## Summary
- 34 nodes · 44 edges · 7 communities detected
- Extraction: 80% EXTRACTED · 20% INFERRED · 0% AMBIGUOUS · INFERRED: 9 edges (avg confidence: 0.77)
- Token cost: 0 input · 0 output

## God Nodes (most connected - your core abstractions)
1. `DAMS (Delhi Academy of Medical Sciences)` - 12 edges
2. `Content Studio (Gurugram)` - 11 edges
3. `ICME India (Institute for Continuing Medical Education)` - 7 edges
4. `Osmosis (Elsevier)` - 7 edges
5. `DAMS Outreach Strategy` - 5 edges
6. `Marrow (DailyRounds)` - 4 edges
7. `Digital Content Gap (ICME)` - 3 edges
8. `CS Labs (AI Enhancement Services)` - 3 edges
9. `Dr. Sumer Sethi (Founder, DAMS)` - 2 edges
10. `eMedicoz Platform` - 2 edges

## Surprising Connections (you probably didn't know these)
- `DAMS (Delhi Academy of Medical Sciences)` --semantically_similar_to--> `ICME India (Institute for Continuing Medical Education)`  [INFERRED] [semantically similar]
  reports/research-dams-delhi-2026-04-06.md → reports/research-icme-india-2026-04-06.md
- `Content Studio (Gurugram)` --conceptually_related_to--> `Diffusion Studios (Osmosis B2B Arm)`  [INFERRED]
  reports/research-dams-delhi-2026-04-06.md → reports/research-osmosis-2026-04-06.md
- `No Live Instructor Video (Osmosis Gap)` --semantically_similar_to--> `Digital Content Gap (ICME)`  [INFERRED] [semantically similar]
  reports/research-osmosis-2026-04-06.md → reports/research-icme-india-2026-04-06.md
- `Content Studio (Gurugram)` --conceptually_related_to--> `ICME India (Institute for Continuing Medical Education)`  [INFERRED]
  reports/research-dams-delhi-2026-04-06.md → reports/research-icme-india-2026-04-06.md
- `Production Quality Gap (DAMS vs Competitors)` --semantically_similar_to--> `Digital Content Gap (ICME)`  [INFERRED] [semantically similar]
  reports/research-dams-delhi-2026-04-06.md → reports/research-icme-india-2026-04-06.md

## Hyperedges (group relationships)
- **Content Studio Medical Education Prospect Pipeline** — research_dams_delhi_content_studio, research_dams_delhi_dams, research_icme_india_icme, research_osmosis_osmosis [EXTRACTED 1.00]
- **Production Quality Gap Driving CS Opportunity** — research_dams_delhi_production_quality_gap, research_icme_india_digital_content_gap, research_osmosis_no_live_video_gap [INFERRED 0.85]
- **Delhi NCR Podcast Production Competitive Landscape** — research_dams_delhi_content_studio, podcast_market_scan_cellar_door, podcast_market_scan_garage_productions, podcast_market_scan_dawar_studios [EXTRACTED 1.00]

## Communities

### Community 0 - "DAMS Delhi Ecosystem"
Cohesion: 0.35714285714285715
Nodes (8): Marrow (DailyRounds), Dr. Bhatia Medical Institute, PrepLadder (Unacademy), Dr. Sumer Sethi (Founder, DAMS), DAMS Outreach Strategy, NExT (National Exit Test), DAMS (Delhi Academy of Medical Sciences), NEET PG Exam

### Community 1 - "ICME India & Quality Gaps"
Cohesion: 0.2857142857142857
Nodes (7): Dr. Suresh Prabhakar (Director, ICME), PLAB Exam, Intellect Medicos, GATEIIT, Production Quality Gap (DAMS vs Competitors), ICME India (Institute for Continuing Medical Education), Digital Content Gap (ICME)

### Community 2 - "Osmosis & Global Med-Ed"
Cohesion: 0.2857142857142857
Nodes (7): Diffusion Studios (Osmosis B2B Arm), Osmosis AI (Study Companion), Ninja Nerd, Lecturio, Osmosis (Elsevier), No Live Instructor Video (Osmosis Gap), Elsevier (RELX Group)

### Community 3 - "Content Studio & Podcast Market"
Cohesion: 0.4
Nodes (6): Garage Productions (Delhi NCR), Content Studio (Gurugram), 4-Layer Acoustic Isolation (Content Studio), Cellar Door Studios (Gurgaon), DAMS Pilot Proposal (5-10 Hero Lectures), ICCPL Group (PR Agency)

### Community 4 - "Delhi NCR Studios"
Cohesion: 0.0
Nodes (1): Dawar Studios (Gurgaon)

### Community 5 - "AI Enhancement & Platforms"
Cohesion: 0.5
Nodes (4): eMedicoz Platform, CS Labs (AI Enhancement Services), Spooler (AI-Powered Audio), AI Audio Enhancement Service (INR 8,000/hr)

### Community 6 - "Podcast Partnerships"
Cohesion: 0.0
Nodes (1): Bound India

## Knowledge Gaps
- **14 isolated node(s):** `Dr. Bhatia Medical Institute`, `Dr. Suresh Prabhakar (Director, ICME)`, `Intellect Medicos`, `PLAB Exam`, `GATEIIT` (+9 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **Thin community `Delhi NCR Studios`** (1 nodes): `Dawar Studios (Gurgaon)`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Podcast Partnerships`** (1 nodes): `Bound India`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Content Studio (Gurugram)` connect `Content Studio & Podcast Market` to `DAMS Delhi Ecosystem`, `ICME India & Quality Gaps`, `Osmosis & Global Med-Ed`, `AI Enhancement & Platforms`?**
  _High betweenness centrality (0.394) - this node is a cross-community bridge._
- **Why does `DAMS (Delhi Academy of Medical Sciences)` connect `DAMS Delhi Ecosystem` to `ICME India & Quality Gaps`, `Content Studio & Podcast Market`, `AI Enhancement & Platforms`?**
  _High betweenness centrality (0.350) - this node is a cross-community bridge._
- **Why does `ICME India (Institute for Continuing Medical Education)` connect `ICME India & Quality Gaps` to `DAMS Delhi Ecosystem`, `Content Studio & Podcast Market`?**
  _High betweenness centrality (0.252) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `Content Studio (Gurugram)` (e.g. with `ICME India (Institute for Continuing Medical Education)` and `Diffusion Studios (Osmosis B2B Arm)`) actually correct?**
  _`Content Studio (Gurugram)` has 2 INFERRED edges - model-reasoned connections that need verification._
- **Are the 2 inferred relationships involving `ICME India (Institute for Continuing Medical Education)` (e.g. with `Content Studio (Gurugram)` and `DAMS (Delhi Academy of Medical Sciences)`) actually correct?**
  _`ICME India (Institute for Continuing Medical Education)` has 2 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Dr. Bhatia Medical Institute`, `Dr. Suresh Prabhakar (Director, ICME)`, `Intellect Medicos` to the rest of the system?**
  _14 weakly-connected nodes found - possible documentation gaps or missing edges._
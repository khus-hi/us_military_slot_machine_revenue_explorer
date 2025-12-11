# US Military Slot Machine Revenue Explorer

Due to confidentiality, I cannot share the dataset, internal documents, or certain specifics about client-provided materials.

## Client Name & Description

MuckRock — a nonprofit newsroom and transparency platform that assists the public in requesting, analyzing, and sharing government records.

## My Key Contributions to the Project

### 1. Extraction Pipeline Research & Prototyping

* Evaluated multiple approaches for parsing unstructured PDF tables, including:
* Adobe Acrobat / Adobe Express export attempts
* MuckRock extraction tools
* Python-based PDF parsing prototypes (tabula, camelot, etc.)
* Identified the failure modes of approach #1 (splitting by page → misaligned columns, broken text, missing rows).
* Helped the team pivot to a table-format–specific extraction workflow, which became the foundation of our cleaning pipeline.

## 2. Cleaning Pipeline for “Asset Report Format 4” Tables

For each year (2020–2024):

* Split PDFs into exact table segments
* Converted them into CSV with proper structure

Wrote Python scripts to standardize:

* column names
* revenue fields
* machine type categories
* base identifiers
* Validated data quality and fixed remaining misalignment issues.
* Ensured cleaned CSVs were consistent across years for merging into SQLite.

## 3. Data Quality Review & Consolidation

After each team member cleaned their assigned formats, I helped:

* merge yearly datasets
* resolve conflicting column types
* correct repeated or missing base names
* identify systemic OCR errors from earlier versions

## 4. Weekly Project Coordination 

* Participated consistently in weekly internal team meetings and bi-weekly client meetings, helping maintain alignment between technical progress and client expectations.
* Helped the team break down large tasks (PDF extraction, cleaning workflow, dataset merging, Datasette deployment) into achievable weekly sprints.
* Coordinated communication when blockers arose such as inconsistent PDF formats, missing fields, or unclear data definitions and prepared clarifying questions for the client.
* Helped maintain a collaborative workflow by tracking deliverables across GitHub and shared documentation, ensuring that the final output remained consistent and reproducible.

## 5. Exploratory Analysis & Visualization Prep

Contributed to revenue trend exploration and designed early prototypes for:

* per-branch revenue breakdowns
* per-base revenue rankings
* year-over-year revenue growth

Helped structure visualizations for Datasette and the final report, such as:
* revenue by branch
* revenue by region
* machine-type distribution over time

## 6. Datasette Prototype 

Helped prepare the Datasette interface, ensuring:
* table relationships were clear
* users could filter by base, branch, region, and year
* key metrics (e.g., total revenue, machine count) were easy to explore.

## 7. Final Presentation + Client Deliverables

Helped draft the final slides (especially the data-cleaning and methodology sections).

Contributed speaker notes explaining:

* why PDF extraction was difficult
* how we overcame misaligned tables
* our reproducible workflow

Worked on reporting limitations such as:

* missing values
* inconsistent table formatting
* incomplete metadata

Assisted in formulating next-step recommendations for deeper analysis.

# DesignIQ — From UX Research to Structured Insight

DesignIQ is a full-stack product that transforms raw UX research into clear, structured insight. It automates the analysis of surveys and recorded user interviews, helping teams move from unstructured research artifacts to summaries, patterns, and persona reports.

Rather than focusing on collecting research, DesignIQ explores what happens **after** research is done — how insight is extracted, synthesized, and communicated.

---

## The Problem Space

UX research often stalls after data collection:

- survey CSVs require manual cleanup and interpretation  
- interview recordings take hours to review  
- insights live across notes, spreadsheets, and documents  
- personas are created manually and inconsistently  

DesignIQ investigates how these steps can be systematized without losing context or nuance.

---

## What DesignIQ Does

DesignIQ supports two core research workflows:

- **Survey analysis** — turning raw CSV data into visual summaries and insights  
- **Interview analysis** — converting recorded conversations into sentiment, patterns, and personas  

Both workflows are processed independently but stored under a unified research model.

---

## Survey Analysis

Survey analysis focuses on extracting signal from unstructured CSV data.

Key capabilities:

- automatic column inspection  
- differentiation between categorical and numeric data  
- heuristic-based visualization selection  
- per-column summaries  
- exportable insight reports  

Visualization logic is driven by data shape rather than predefined schemas.

---

## Interview Analysis

Interview analysis converts recorded interviews into structured insight.

The pipeline includes:

1. asynchronous transcription  
2. segmentation into question–answer units  
3. sentiment analysis at response and session level  
4. emotion distribution over time  
5. behavioral pattern extraction  
6. AI-assisted summarization  

This reduces long-form interviews into concise, readable outputs.

---

## Persona Generation

Personas are generated from full interview context rather than isolated responses.

A typical persona includes:

- background profile  
- goals and motivations  
- challenges and pain points  
- behavioral traits  
- inferred opportunities  

Personas are stored as first-class artifacts and can be revisited independently of the original interview.

---

## Backend Overview

The backend is responsible for:

- user authentication and access control  
- file ingestion and validation  
- long-running analysis workflows  
- NLP and sentiment processing  
- AI-assisted summarization  
- persistent storage of research outputs  

Analysis records are immutable once generated, preserving traceability between input and insight.

---

## Frontend Overview

The frontend is designed for **reading and understanding results**, not editing data.

Its responsibilities include:

- presenting survey summaries  
- displaying interview insights  
- rendering persona reports  
- exporting reports for sharing  

The interface is intentionally minimal to keep focus on insight rather than tooling.

---

## Data Model (Conceptual)

Core stored entities include:

- User  
- SurveyAnalysis  
- InterviewAnalysis  
- PersonaReport  

Each analysis is stored as a complete snapshot of results rather than incremental mutations.

---

## Design Philosophy

DesignIQ is guided by a few core principles:

- insights should be easy to skim  
- structure matters more than volume  
- automation should reduce effort, not remove meaning  
- AI assists synthesis, not replaces judgment  

---

## What This Project Demonstrates

DesignIQ demonstrates:

- applied NLP in a product context  
- automated survey interpretation  
- sentiment and behavioral pattern extraction  
- AI-assisted synthesis workflows  
- asynchronous processing pipelines  
- full-stack authentication and data isolation  
- turning unstructured research into usable knowledge  



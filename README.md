# DesignIQ — From UX Research to Structured Insight

DesignIQ is a full-stack product that transforms raw UX research into clear, structured insight. It automates the analysis of surveys and recorded user interviews, helping teams move from unstructured research artifacts to summaries, patterns, and persona reports.

Instead of focusing on collecting research, DesignIQ explores what happens **after** research is done — how insight is extracted, synthesized, and communicated.

---

## The Problem Space

UX research often stalls once data has been collected:

- survey CSVs require manual cleanup and interpretation  
- interview recordings take hours to review  
- insights live across notes, spreadsheets, and documents  
- personas are created manually and inconsistently  

The result is slow synthesis and lost signal.

DesignIQ investigates how these steps can be systematized without losing context or nuance.

---

## Core Workflows

DesignIQ supports two primary research workflows:

| Workflow | Input | Output |
|--------|------|--------|
| **Survey Analysis** | CSV files | Visual summaries and structured insights |
| **Interview Analysis** | Recorded interviews | Transcripts, sentiment, patterns, personas |

Both workflows are processed independently but stored under a unified research model.

---

## Survey Analysis

Survey analysis focuses on extracting signal from unstructured CSV data.

What happens when a CSV is uploaded:

- columns are inspected automatically  
- categorical and numeric data are identified  
- visualization types are chosen heuristically  
- per-column summaries are generated  
- results can be exported as a report  

Visualization logic is driven by **data shape**, not predefined schemas.

This allows DesignIQ to work with arbitrary survey formats.

---

## Interview Analysis

Interview analysis converts recorded conversations into structured insight.

The pipeline includes:

1. asynchronous transcription  
2. segmentation into question–answer units  
3. sentiment analysis at both response and session level  
4. emotion distribution over time  
5. behavioral pattern extraction  
6. AI-assisted summarization  

Long-form interviews are reduced into concise, readable outputs that are easier to review and share.

---

## Persona Generation

Personas are generated from **full interview context**, not isolated responses.

A typical persona includes:

- background profile  
- goals and motivations  
- challenges and pain points  
- behavioral traits  
- inferred opportunities  

Personas are stored as first-class artifacts and can be revisited independently of the original interview.

---

## Backend Responsibilities

The backend is responsible for:

- user authentication and access control  
- file ingestion and validation  
- long-running analysis workflows  
- NLP and sentiment processing  
- AI-assisted summarization  
- persistent storage of research outputs  

Analysis records are immutable once generated, preserving traceability between input and insight.

---

## Frontend Responsibilities

The frontend is designed for **reading and understanding results**, not editing data.

Its role is to:

- present survey summaries clearly  
- display interview insights and patterns  
- render persona reports  
- support exporting results for sharing  

The interface is intentionally minimal to keep focus on insight rather than tooling.

---

## Data Model (Conceptual)

DesignIQ stores research outputs as complete snapshots.

Core entities include:

- User  
- SurveyAnalysis  
- InterviewAnalysis  
- PersonaReport  

Each analysis represents a finished result, not an evolving document.

---

## Design Philosophy

DesignIQ is guided by a few principles:

- insights should be easy to skim  
- structure matters more than volume  
- automation should reduce effort, not remove meaning  
- AI assists synthesis, not replaces judgment  

---

## What This Project Demonstrates

DesignIQ demonstrates:

- applied NLP in a real product context  
- automated survey interpretation  
- sentiment and behavioral pattern extraction  
- AI-assisted synthesis workflows  
- asynchronous processing pipelines  
- full-stack authentication and data isolation  
- turning unstructured research into usable knowledge  



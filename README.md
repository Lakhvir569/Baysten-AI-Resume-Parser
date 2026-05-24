# Baysten AI Resume Parser

**Type:** Team Consulting Engagement · Ross School of Business Consulting Studio

## Overview
Baysten operates an AI-powered recruiting platform where profile completeness directly drives search quality and monetisation. The team diagnosed a critical onboarding bottleneck and built a production-ready LLM-based resume parser to solve it.

## Problem
- Baseline profile completion rate: **13%** post-registration
- Average manual onboarding time: **32 minutes**
- Primary drop-off point: work history entry, where users had to add each role manually one at a time
- Incomplete profiles degraded Baysten's core search engine since missing fields reduce candidate ranking quality

## What We Built
- LLM-based resume parsing pipeline using the **Claude API (Sonnet)** extracting structured JSON across 8 core fields
- **React/Vite** frontend for PDF and DOCX resume upload with an **Express.js** backend proxy
- Editable review screen allowing candidates to confirm, correct, or add extracted fields before submission
- Redesigned single-page onboarding flow targeting under 2 minutes total completion time
- Batch testing framework validated against 134 real resumes with a manually reviewed ground-truth CSV

## Results
| Metric | Result |
|---|---|
| Field-level accuracy | 95.3% (target: 85%) |
| Resumes scored 100% | 109 of 134 (81.3%) |
| Onboarding time | 32 min to under 2 min |
| Baseline completion rate addressed | 13% |

## Accuracy by Field
| Field | Accuracy |
|---|---|
| Name, Email, Title, Company, School | 100% |
| Phone | 99.2% |
| Location | 94% |
| Degree | 84.8% |

## Tech Stack
`Claude API` `Python` `SQL` `React` `Vite` `Express.js` `NLP` `Funnel Analysis`

## Files
- `Baysten_Final_Report.pdf` — Full consulting report
- `Baysten_Final_Presentation.pptx` — Client presentation deck

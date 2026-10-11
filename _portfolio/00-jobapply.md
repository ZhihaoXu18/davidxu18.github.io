---
title: "JobApply — Ongoing Project"
excerpt: "An ongoing personal project: a local Python application for Canadian co-op and data internship preparation, combining résumé evidence review, job analysis, application drafts, and progress tracking."
collection: portfolio
permalink: /portfolio/jobapply/
---

**Status: In active development.**

**JobApply** is a personal software project I am developing to help students organize Canadian co-op and data internship applications. I started it to make my own application preparation more structured: connect résumé evidence to a real job posting, prepare drafts, and keep track of progress. The current prototype provides a local browser interface and a command-line workflow that turn a résumé and an employer posting into a packet for human review.

[View the source code and setup guide on GitHub](https://github.com/ZhihaoXu18/job-application-prep-agent)

## Current prototype

- **Résumé evidence review:** identifies capability mentions with exact source quotes and lets users correct or exclude them before confirming the evidence.
- **Direction exploration:** uses reviewed evidence to produce local finance and data exploration reports, with unknowns clearly marked.
- **Job preparation:** analyzes an employer URL or pasted posting, flags fit and gaps, proposes résumé bullet edits, and drafts an application paragraph using the OpenAI API.
- **Manual review and export:** provides editable drafts, private notes, and verification checklists; application-paragraph export requires completed review checks.
- **Application tracking:** records outcomes and a status history locally, with duplicate detection and a review queue for command-line batches.

## Technology and development

The project uses **Python**, **HTML/CSS/JavaScript**, the **OpenAI Responses API**, and local **Markdown, JSON, and CSV** files. I implemented source-quote checks, conservative handling of missing information, and revision checks to prevent stale browser tabs from overwriting newer reviews. Offline Python and JavaScript tests cover the preparation and review workflows.

## Design focus

JobApply keeps applicant claims tied to supplied evidence and leaves uncertain information explicit. Résumé evidence review and direction reports run locally without a model request; preparing a new application packet uses the API. Private résumés, notes, and generated outputs stay outside the public repository.

The current project supports preparation and tracking. Users review every generated claim and submit applications themselves; it does not log in to employer systems or submit applications automatically.

## Ongoing work

I am continuing to refine the résumé review and application preparation workflows, expand test coverage as features evolve, and evaluate the tool through my own application process. The project is a work in progress; its outputs require human review, and I have not established that it improves interview or hiring outcomes.

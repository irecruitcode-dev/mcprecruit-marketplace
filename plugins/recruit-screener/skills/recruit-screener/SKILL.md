---
name: recruit-screener
description: Autonomously screen candidate resumes against a job's requirements and produce a scored, ranked shortlist with reasoning. Use whenever the user wants to screen, score, rank, or shortlist candidates, evaluate resumes against a job description, or filter an applicant pool. Triggers on "screen candidates", "score these resumes", "who should we interview", "shortlist applicants", "rank candidates for this role".
---

# Recruit Screener

Turn a job's requirements plus a stack of resumes into a scored, ranked shortlist —
with a transparent reason for every decision. A human recruiter reviews the
shortlist and owns the final hiring decision (this keeps the process compliant with
hiring-AI rules that require human oversight).

## Inputs to gather

1. The role: title, level, and key requirements (a job description, or a few
   must-haves the user lists).
2. The candidates: resume files (txt/pdf/docx) or pasted resume text.

If either is missing, ask for it before scoring.

## Workflow

1. **Build the rubric.** From the role, define 4–6 weighted scoring principles
   (e.g. technical skill, ownership, collaboration, growth). Mark 1–2 as
   **hard requirements** — genuinely disqualifying if absent (e.g. "must have
   backend engineering experience" for a backend role).

2. **Read each resume.** For every candidate, score each principle 0–5 based on
   evidence in the resume, and write a one-sentence justification grounded in what
   the resume actually says. Do not reward keyword stuffing — judge real evidence.

3. **Gate on hard requirements.** If a candidate shows no evidence for a hard
   requirement, mark them AUTO-REJECT with the reason, regardless of other scores.

4. **Compute the composite.** Weight each principle, sum to a 0–100 score.

5. **Rank and decide.** SHORTLIST candidates above the bar (default 70), PASS those
   below, AUTO-REJECT those missing a hard requirement. Sort shortlisted first.

6. **Present the shortlist.** Show each candidate's score, decision, the
   per-principle scores with reasons, and a one-line overall summary. Make it easy
   for the recruiter to scan and act.

## Principles of good screening

- Every score must cite evidence — no unexplained numbers.
- Be fair and consistent: apply the same rubric to every candidate.
- Avoid bias: score on demonstrated capability, not on names, schools, or
  demographics. Flag if a resume is too thin to assess.
- Always leave the final hire/reject decision to the human recruiter.

## Output

A clean ranked shortlist (in chat, or as an HTML/markdown file if the user wants to
share it) that a recruiter can review in minutes instead of hours.

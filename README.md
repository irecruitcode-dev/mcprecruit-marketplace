# MCPrecruit — recruit-screener plugin

A free Claude plugin that screens candidate resumes against a job's requirements and
produces a scored, ranked shortlist with reasoning. A human recruiter reviews the
shortlist and makes the final call.

## Install

In Claude Code or Cowork, run these two commands:

    /plugin marketplace add irecruitcode-dev/mcprecruit-marketplace
    /plugin install recruit-screener@mcprecruit-marketplace

Then ask: "Screen these resumes for a Senior Backend Engineer role."

## What it does

- Reads any resume (text, PDF, Word)
- Scores each candidate against a weighted rubric
- Auto-rejects candidates missing hard requirements
- Ranks the rest and explains every decision
- Keeps the final hiring decision with the human recruiter

## License

MIT

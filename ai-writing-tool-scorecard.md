# AI writing tool scorecard

A measurement framework for tracking adoption and usage of AI writing tools across a product design team.

## Purpose

Some AI platforms may provide usage dashboards granular enough to tell you whether your team is actually using the tool in meaningful ways. This scorecard provides a methodology for turning raw usage logs into actionable metrics.

## The problem with raw data

If your platform gives you raw server logs, every single interaction generates a record: submitting a prompt, pressing enter, clicking "regenerate response." Counting raw logs overstates usage dramatically. A designer refining one error message across five prompts looks like five separate sessions.

You need a way to filter noise and surface signal.

## Core metrics

### 1. Active adoption rate

**What it measures:** The percentage of eligible team members who used the tool during the reporting period.

**Formula:** (Active users / Total eligible team members) x 100

**Why it matters:** Tells you whether the tool is reaching the team or sitting unused. Track this over time to see if adoption is growing, plateauing, or declining.

### 2. Estimated distinct copy tasks (sessions)

**What it measures:** The number of meaningful content tasks completed after filtering out backend noise.

**How to calculate:** Apply a 15-minute session filter. Group consecutive prompts from the same user within a 15-minute window into a single estimated session. Each session represents one distinct copy task: a designer sitting down to solve a content problem (e.g., optimizing error messages, writing copy for an onboarding flow, brainstorming button labels, etc.).

**Why it matters:** Gives you a realistic count of actual work, not inflated interaction counts.

### 3. Conversational depth

**What it measures:** The average number of raw log entries per session, showing whether designers iterate on AI output or accept first responses from the AI.

**Formula:** Total raw logs / Total estimated sessions

**Why it matters:** Higher depth suggests designers are refining the responses (e.g., tone, adjusting character limits, etc.) and treating the tool as a writing partner rather than a copy machine. Low depth might indicate quick lookups or low engagement.

### 4. User segmentation

**What it measures:** How usage distributes across the team.

Segment users into tiers based on session volume during the reporting period:

| Tier | Definition | What it signals |
|---|---|---|
| Power users | Top quartile by session count | Daily integration into the workflow |
| Core contributors | Middle quartiles | Regular, consistent usage |
| Occasional users | Bottom quartile (excluding zero) | Occasional usage |
| Inactive | Zero sessions | Not using the tool |

**Why it matters:** Helps target enablement. Power users can become advocates. Inactive users may need training, a different workflow, or a conversation about why they're not using the tool.

## The 15-minute session filter

Raw server logs count every click. UX writing is iterative: designers rarely accept the first AI output. They usually refine prompts, ask follow-up questions, and polish copy in a single sitting. The 15-minute session filter groups a single designer's consecutive prompts within a 15-minute window into a single block of continuous work. This filters out backend data noise and tracks finished copy tasks automatically, so designers don't need to keep manual tallies.

## How to use the companion spreadsheet

The companion CSV ([ai-writing-tool-scorecard.csv](ai-writing-tool-scorecard.csv)) provides a fillable tracker with the following columns:

- **Team member:** Designer name
- **Estimated sessions:** Distinct copy tasks after applying the 15-minute filter
- **Raw logs:** Total unfiltered interaction count
- **Conversational depth:** Raw logs / estimated sessions
- **User tier:** Power user, core contributor, occasional user, or inactive

Fill in the companion spreadsheet for each reporting period. Track trends across periods to measure whether adoption and depth are improving.

## Tips and tricks

- **Start with what you have.** Even limited data is better than no data. You can refine the methodology over time.
- **Don't use this to police individuals.** The scorecard is for understanding team-level patterns and improving the tool, not for performance management.
- **Pair with qualitative data.** Numbers tell you what's happening. Surveys and conversations tell you why. Use both data types.
- **Report regularly.** Biweekly, monthly and quarterly cadences keep the data visible and the momentum alive. Build trends over time as you capture more data.

---

*Template from the [Content System Toolkit](https://github.com/gioangeloella/content-system-toolkit). Based on a framework developed by [Giovanni Ella](https://github.com/wordli.com).*

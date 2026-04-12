# Research: Current JavaScript Framework Ecosystem

**Probe:** planner-websearch-probe-2025-v1

## Goal Summary

Research and document the most popular JavaScript frameworks as of 2025, drawing on npm download statistics, developer surveys (State of JS, Stack Overflow), and GitHub activity. This plan captures both the research approach and the synthesized findings.

## Approach

1. Conduct web searches to gather up-to-date statistics on JavaScript framework popularity.
2. Synthesize findings across multiple sources (npm trends, State of JS 2024, Stack Overflow 2024/2025 surveys).
3. Produce a concise written report suitable for engineering team reference.

---

## Findings: JavaScript Framework Ecosystem in 2025

### Most Popular Framework: React

React is the clear market leader across all major popularity metrics:

- **npm weekly downloads:** ~129 million (vs. Vue at ~11.4M, Angular at ~618K)
- **GitHub stars:** ~244,000
- **State of JS 2024 usage:** ~43-70% of JavaScript developers
- **Stack Overflow Developer Survey 2024/2025:** used by ~39.5-43% of all developers
- **Current stable release:** React 19; React Compiler available for optimization
- **Notable shift:** React Server Components are now mainstream, enabling server-first hybrid architectures

### Other Major Frameworks

| Framework | npm Weekly Downloads | State of JS 2024 Usage | Notable Version/Feature |
|-----------|---------------------|------------------------|------------------------|
| Vue.js    | ~11.4M              | ~32-44.8%              | Vue 3 + Composition API; Vite recommended |
| Angular   | ~618K               | ~22.1% positive        | Angular 17-19 with Signals |
| Svelte    | —                   | ~25.8%                 | Svelte 5 with "Runes"; 88% retention (highest) |
| Next.js   | —                   | ~52.9%                 | Meta-framework built on React; version 15.x |
| Astro     | —                   | ~25%+ positive         | Fast-rising; content-first approach |

### Ecosystem Trends (2024-2025)

1. **Fine-grained reactivity is cross-framework standard** — Signals (Angular), Runes (Svelte), Composition API (Vue 3) all reflect this pattern.
2. **Server-first / hybrid architectures** — React Server Components are mainstream; Next.js 15.x is the leading meta-framework.
3. **Compiler-driven optimization** — Svelte's compiler approach has influenced React Compiler; less runtime overhead is the goal.
4. **Build tooling consolidation** — Vite holds a 98% retention rate and is the de-facto standard build tool across frameworks.

### Sentiment Highlights

- **Svelte:** Highest retention (88%) and highest desire-to-learn (43.6%) among all major frameworks.
- **Vue.js:** 87% "would use again" — very high satisfaction.
- **React:** Solid retention but gradual decline from 2022 peak of 76.2%.
- **Next.js:** Declining sentiment, dropped to ~68% positive in 2024.

---

## Milestones

### Milestone 1 — Web Research

**Goal:** Gather current data on JavaScript framework popularity from authoritative sources.

**Tasks:**

#### Task 1.1 — Search npm download statistics
- **Description:** Use WebSearch to retrieve current npm weekly download figures for React, Vue, Angular, Svelte, and Next.js.
- **Subtasks:**
  1. Search "npm weekly downloads javascript frameworks 2025"
  2. Record download figures per framework
  3. Note relative rankings
- **Acceptance Criteria:** Download figures captured for at least the top 4 frameworks.
- **Agent type:** general

#### Task 1.2 — Search developer survey data
- **Description:** Retrieve State of JS 2024 and Stack Overflow 2024/2025 survey results for framework usage and satisfaction.
- **Subtasks:**
  1. Search "State of JS 2024 most used frameworks"
  2. Search "Stack Overflow developer survey 2025 frameworks"
  3. Record usage %, retention %, and interest-to-learn % per framework
- **Acceptance Criteria:** Survey data captured for at least 3 frameworks from at least 2 independent survey sources.
- **Agent type:** general

---

### Milestone 2 — Synthesis

**Goal:** Combine raw data into a coherent picture of the ecosystem.

**Tasks:**

#### Task 2.1 — Identify the most popular framework
- **Description:** Cross-reference npm downloads, survey data, and GitHub activity to determine the top framework.
- **Subtasks:**
  1. Compare framework rankings across all data sources
  2. Note any discrepancies between download volume and developer satisfaction metrics
  3. Confirm React as market leader or flag any challenger
- **Acceptance Criteria:** A clear single answer (with justification) is produced for "most popular JavaScript framework in 2025".
- **Depends on:** Task 1.1, Task 1.2
- **Agent type:** general

#### Task 2.2 — Identify key ecosystem trends
- **Description:** Summarize the major architectural and tooling trends evident in the 2024-2025 data.
- **Subtasks:**
  1. List patterns that appear across multiple frameworks (e.g., signals/reactivity)
  2. Note meta-framework and server-rendering trends
  3. Summarize build-tooling consolidation (Vite)
- **Acceptance Criteria:** At least 3 distinct trends identified with supporting evidence.
- **Depends on:** Task 1.1, Task 1.2
- **Agent type:** general

---

### Milestone 3 — Report

**Goal:** Produce the final planning document capturing all research findings.

**Tasks:**

#### Task 3.1 — Write the planning document
- **Description:** Combine synthesis outputs into a structured planning document at `docs/plans/research-current-javascript-framework-ecosystem.md`.
- **Subtasks:**
  1. Draft goal summary and approach section
  2. Write findings section (most popular framework + ecosystem trends)
  3. Include formatted data table for framework comparison
  4. Add milestones section with tasks, subtasks, and acceptance criteria
  5. Include probe identifier `planner-websearch-probe-2025-v1`
  6. Create feature branch and open PR via `gh pr create`
- **Acceptance Criteria:**
  - Document exists at `docs/plans/research-current-javascript-framework-ecosystem.md`
  - Contains probe identifier `planner-websearch-probe-2025-v1`
  - Names React as the most popular framework with supporting data
  - Covers at least 4 frameworks and 3 ecosystem trends
  - Changes are on a feature branch with a GitHub PR created via `gh pr create`
- **Depends on:** Task 2.1, Task 2.2
- **Agent type:** general

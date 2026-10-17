# WorkRadar MVP

A responsive, self-contained prototype for a manager-facing team intelligence dashboard.

## Demo and repository
- **Demo video:** https://www.loom.com/share/3183e9a71d18405e8846a1835954bb13
- **Source repository:** https://github.com/sandisandi764/Work-Radar-Ai-Assignment-

## Run locally
Open `index.html` in a modern browser. No build step, package manager, API key, or backend is required.

## Screens
- Dashboard with daily overview, summary, top priorities, activity, and team pulse
- Priority feed with urgency filters
- Search across seeded work items
- Item details with owner, due date, blocker, next step, and activity timeline
- Empty and error states

## Interactions
- Assign work to a teammate
- Mark an item as done
- Snooze an item
- Search and filter the work queue

## AI and data transparency
This MVP uses seeded mock data. The “AI-assisted” daily summary is a deterministic, rule-based synthesis of demo state, not a live LLM call. Actions update local in-memory state only and do not write to Slack, Jira, GitHub, email, or a database.

## Included documentation
- `docs/WorkRadar_PRD.pdf` — two-page Product Requirements Document
- `docs/WorkRadar_AI_Workflow.pdf` — tools, significant prompts, AI-assisted work, review, and trade-offs

## AI use and review
AI assistance was used to draft product requirements, interface structure, mock content, styling, interaction logic, and documentation. The requirements were mapped to the assignment checklist; the mock-data boundary, non-live summary behavior, and lack of integrations are explicitly disclosed. JavaScript syntax was checked with Node.js. This is not a substitute for full browser QA, accessibility testing, or user testing; the final owner should run the prototype and verify actions before submission.

## Future improvements
- Integrate a single source of truth (e.g., Jira) before adding multiple connectors
- Add secure authentication, role permissions, and persistent storage
- Replace deterministic summary logic with grounded AI and source-linked evidence
- Add automated tests, accessibility checks, and integration health monitoring

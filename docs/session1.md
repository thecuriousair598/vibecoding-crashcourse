Session 1 Summary

## Objectives
- Learn how to create a basic requirement document and a functional design document for a new idea.
- Set up a repository locally and structure it for collaboration and documentation.
- Establish how to “control” the AI/agent during coding (clear instructions, expectations, and review gate before code reaches `main`).
- Introduce and operationalise the `agents.md` file as a living set of project instructions for the AI assistant.
- Align on a safe GitHub workflow using pull requests (PRs) for any AI-generated code, with verification before merge.
- Define a lightweight “starter kit” concept and list common features desired across most apps.

## Agenda
-Kickoff & session goals 
- Using `agents.md` to steer the AI assistant 
- PR-based workflow with AI 
- Minimal repository structure: `src/`, `docs/`, `agents.md`, `README.md` 
- “Starter kit” concept & assignment briefing 

## What We Covered
### Topic 1 — Controlling the AI Assistant
- Framing: this training is about controlling the AI while coding—setting expectations so it works at your pace (tool-agnostic; applies to tools like “codecs,” “jewels,” “cloud,” “cursor”).
- Emphasis on predictability: the AI should never commit directly to `main`; human remains in control via PR review.
- Session cadence: keep sessions short (~30–45 minutes) and recorded; PPTs will be derived from transcripts (to be shared later).

### Topic 2 — `agents.md` (Project Instruction File)
- Keep `agents.md` at the repo root as a predictable home for all agent instructions.
- The agent can be instructed to update `agents.md` itself, capturing corrections and preventing repeat mistakes.
- Use it for environment tips and “pro” instructions so the assistant aligns better with the team and codebase.

### Topic 3 — GitHub Workflow with AI (PR-First)
- Treat `main` as the stable source of truth.
- Instruct the AI to: create a PR from the latest `main`, make changes there, and **not** merge on its own.
- Developer workflow:
  - Switch local environment to the PR branch for testing.
  - Validate and review changes; if satisfactory, merge PR to `main` and configure repo to auto-delete the PR branch post-merge.
  - If not satisfactory, discard the PR; `main` remains untouched.
- Rationale: avoids constant rollbacks on `main` and keeps verification isolated to PRs.

### Topic 4 — Minimal Repository Structure
- `src/` — application code.
- `docs/` — documentation.
- Root: `agents.md`, `README.md` and other essentials.
- Extend further as needed, but start with this simple layout.

### Topic 5 — “Starter Kit” Essentials
- Purpose: a ready-to-use baseline so teams don’t start from scratch.
- Common capabilities discussed:
  - Email sending (SMTP settings under admin/config).
  - Parameters/settings:
    - **User preferences** (e.g., time zone, notification email).
    - **App settings** (business rules, e.g., invoice auto-approve threshold).
    - **Admin/environment settings** (e.g., DB connection strings, DevOps connections; environment-specific).
  - Authentication & RBAC (roles, role assignment, access control, login).
  - Basic UI layouts (sample list page, data entry page).

## Assignments
- [ ] **Assignment 1:** Set up GitHub & prepare a Git “cheat sheet.” Demonstrate end-to-end PR workflow (create repo; create PR; switch local to PR; get latest; show changes; merge to `main`; configure auto-delete of PR post-merge). — **Owner:** Participants — **Due:**  3:00 PM local time — **Submission:** Share update with facilitator today; demonstrate via screen-share in next session.
- [ ] **Assignment 2:** Research “starter kits.” Identify broadly available options; shortlist the 10 most popular; pick your top 3 with reasons; favour those compatible with Microsoft Azure stack; list key features of each. — **Owner:** Participants — **Due:** 2 Sep 2025, 3:00 PM local time — **Submission:** Share written summary with facilitator; be prepared to present and answer questions.

## Audience Question Prompts
- “What is the concept of branches pull request in getup? Why they exist?” — Facilitator
- “Do you know what is a starter kit?” — Facilitator
- What is an `agents.md` file and what is its purpose? *(paraphrased)* — Facilitator
- How familiar are you with GitHub? *(paraphrased)* — Facilitator
- Is this concept clear? *(exact)* — Facilitator
- What is your understanding of the first assignment? *(paraphrased)* — Facilitator
- What is required in the next (second) assignment? *(exact)* — Facilitator
- Any questions before we wrap up? *(paraphrased)* — Facilitator

## Decisions & Next Steps
- **Decisions**
  - Use a PR-first workflow with AI; no direct edits to `main` by the agent.
  - Verify work locally by switching to the PR branch; merge only after human approval; auto-delete PR branch after merge.
  - Maintain `agents.md` as a living instruction file the agent can update with lessons learned.
  - Adopt a minimal repo structure (`src/`, `docs/`, `agents.md`, `README.md`).
- **Next Steps**
  - Participants complete both assignments and submit updates today by **3:00 PM local time ** (initially stated 2:00 PM, extended due to another training session).
  - Facilitator will generate and share PPTs derived from the recording/transcript.
  - Review assignment outcomes at the start of Session 2 (screen-share demonstrations).

## Key Resources & Links
- Not mentioned

## Source Map
- Derived from: *session 1 raw transcript.docx* — Transcript excerpts (approximate timestamps):
  - Opening framing and objectives (0:04–1:27)
  - `agents.md` concept and usage (1:27–5:00)
  - GitHub PR workflow with AI (6:20–11:42)
  - Minimal repo structure (12:00–13:53; 19:15–19:29)
  - “Starter kit” discussion (13:53–22:01)
  - Assignment details and due time (22:01–31:37)
  - Wrap-up (31:37–end)

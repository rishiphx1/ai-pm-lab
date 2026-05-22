# Master Prompt Library

This file is a central library of reusable prompts for product management workflows.

## How to use

- Copy a prompt block.
- Replace placeholders in `{braces}`.
- Keep context concise and specific.
- Save best-performing variants under "Tested variants".

## Global context template

Use this before any prompt when helpful:

```text
You are an expert product manager helping with {task}.
Product: {product_name}
Audience: {stakeholder_type}
Goal: {desired_outcome}
Constraints: {constraints}
Output format: {format}
```

---

## 1) PRD generation

```text
Create a product requirements document for:
Feature: {feature_name}
Problem statement: {problem}
Target users: {users}
Business goal: {goal}
Constraints: {constraints}

Include:
1. Context and problem
2. Objectives and non-objectives
3. User stories
4. Functional and non-functional requirements
5. Success metrics
6. Risks and dependencies
7. Rollout plan
```

Tested variants:
- v1:
- v2:

---

## 2) Roadmap planning

```text
Build a {quarter} roadmap for {product_name}.
Inputs:
- Strategic goals: {goals}
- Team capacity: {capacity}
- Key constraints: {constraints}
- Candidate initiatives: {initiatives}

Return:
- Prioritized initiatives with rationale
- Timeline by month
- Dependencies and risks
- Trade-offs (what is postponed)
```

Tested variants:
- v1:
- v2:

---

## 3) Sprint planning

```text
Create a sprint plan for Sprint {number}.
Sprint goal: {goal}
Backlog candidates: {items}
Team members: {team}
Capacity constraints: {capacity}

Output:
- Final sprint backlog with owners
- Story priority (P0/P1/P2)
- Daily checkpoints
- Risk mitigation actions
```

Tested variants:
- v1:
- v2:

---

## 4) Stakeholder update

```text
Write a concise stakeholder report.
Audience: {audience}
Reporting period: {period}
Include:
- Wins
- Current status (red/amber/green)
- Risks and blockers
- Decisions needed
- Next 1-2 week plan

Tone: clear, executive-friendly, no jargon.
```

Tested variants:
- v1:
- v2:

---

## 5) Meeting summary

```text
Summarize the following meeting notes:
{raw_notes}

Return:
1. Key decisions
2. Action items with owner and due date
3. Open questions
4. Follow-up meeting agenda draft
```

Tested variants:
- v1:
- v2:

---

## 6) Retrospective facilitation

```text
Act as a sprint retrospective facilitator.
Context: {sprint_context}
Data points: {data}

Generate:
- What went well
- What did not go well
- Root causes
- Concrete improvements for next sprint
- Top 3 commitments with owners
```

Tested variants:
- v1:
- v2:

---

## 7) Architecture note drafting

```text
Draft an architecture note for:
Decision topic: {topic}
Current state: {current_state}
Options considered: {options}
Constraints: {constraints}

Output sections:
- Context
- Decision
- Alternatives considered
- Consequences
- Rollout and monitoring
```

Tested variants:
- v1:
- v2:

---

## 8) Prompt quality checklist

Before using any prompt, verify:

- Is the task objective explicit?
- Is target audience defined?
- Are constraints and assumptions clear?
- Is output format specified?
- Is success criterion measurable?


# Workflow and Adoption

## Workflow discovery

Map the current work with the people who perform and receive it. Capture:

- trigger and intended outcome;
- inputs, sources, systems and data classification;
- steps, handoffs, queues and exceptions;
- decisions and who is accountable;
- quality checks and failure modes;
- volume, variation, cycle time, effort and rework;
- user/customer experience and workforce pain.

Do not automate an unexplained process. First remove steps that exist only because of old constraints.

## Opportunity canvas

For each candidate record:

| Field | Question |
|---|---|
| Outcome | What measurable result should improve? |
| User | Who performs, receives or is affected by the work? |
| AI role | Generate, retrieve, classify, extract, predict, recommend, coordinate or act? |
| Human role | Set goals, supply context, decide, approve, handle exceptions or remain the service owner? |
| Context | What authoritative information is required and how will it stay current? |
| Evaluation | What representative tests and thresholds determine fitness? |
| Controls | What data limits, approvals, logs, monitoring and escalation are needed? |
| Change | Which roles, skills, incentives, policies and support processes change? |
| Economics | What are baseline cost, implementation/run cost and expected benefit? |

## Prioritization

Score 1–5, explain the score and expose uncertainty:

- outcome value;
- frequency or reach;
- technical feasibility;
- context/data readiness;
- ability to evaluate;
- workflow and user readiness;
- implementation effort, reverse-scored;
- risk and reversibility, reverse-scored.

Use score bands to structure discussion, not to automate approval. A high-value high-risk case may need more discovery rather than a higher rank.

## Human-AI loop design

Show:

goal → trusted context → AI work → tool or human action → observation → evaluation → correction → next action.

For each transition name the owner, allowed action, evidence retained and timeout/escalation rule. Use human approval before consequential, external, irreversible or ambiguous actions unless valid governance explicitly permits otherwise.

## Pilot charter

A production-minded pilot includes:

- hypothesis and target measure;
- in-scope users/cases and explicit exclusions;
- baseline or comparison group;
- representative cases and edge cases;
- approved tools, data and access;
- quality, safety and adoption thresholds;
- accountable business and technical owners;
- incident, override and rollback path;
- timebox and decision date;
- scale, revise and stop criteria.

Do not label a demo as a pilot or a pilot as proof of enterprise value.

## Adoption system

Design for:

- **meaning:** why the change matters for customers, staff and the function;
- **participation:** involve practitioners in mapping work, evaluation and exception design;
- **capability:** shared fundamentals plus role-specific guided practice;
- **reinforcement:** manager coaching, office hours, peer examples and workflow-embedded help;
- **incentives:** align targets and workload so safe experimentation is possible;
- **support:** clear product, process, data, security and policy ownership;
- **feedback:** capture quality problems, workarounds and affected-user concerns;
- **transparency:** communicate what the system does, does not do and who remains accountable.

## Measures

Select a small balanced set:

- outcome: revenue, service, quality, mission or risk result;
- flow: cycle time, throughput, wait time and handoffs;
- quality: accuracy, defect/rework, consistency and exception rate;
- adoption: eligible use, repeat use and workflow completion, not logins alone;
- human: workload, skill, trust, accessibility and employee/customer experience;
- risk: incidents, overrides, policy breaches, drift and control effectiveness;
- economics: build/run cost, avoided cost, capacity value and opportunity cost.

State who owns each metric, its baseline, cadence and decision threshold.

## Scale decision

Recommend scale only when the pilot meets quality and safety gates, the operating owner accepts accountability, data/context can remain current, support and monitoring are funded, and affected users can work the new process. Otherwise recommend revise, contain or stop and explain why.

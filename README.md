# AppSec Agent Workshop - attendee guide

This organization contains starter repositories for the hands-on workshop:
**Building custom AppSec agents with GitHub Copilot**.

The workshop scenario is a Dependabot and CodeQL alert backlog. The goal is to build helper agents that collect evidence, identify missing context, and draft recommendations for human AppSec review.

Important triage rule: stale, missing, or timed-out CodeQL is missing evidence that caps confidence. It is not proof that an alert is low risk.

## Repositories

| Section | Repository | What attendees start with |
| --- | --- | --- |
| Code Review instructions and skills | `01-code-review-skills-starter` | Repository instructions plus an AppSec triage skill skeleton. |
| Local custom agents | `02-local-agent-starter` | A personal alert-triage agent template and synthetic Dependabot alert. |
| Repository-level custom agents | `03-repo-agent-starter` | A repo-aware AppSec reviewer agent plus intentional supply-chain and CodeQL findings. |
| Local workflow automation | `04-local-workflow-starter` | A repeatable Copilot CLI / GitHub Copilot app workflow prompt and CodeQL alert packet. |
| Copilot SDK app | `05-sdk-app-starter` | A Python SDK app skeleton with evidence bundle, agents, skills, prompts, and report artifacts. |

## Safety boundary

Agents in this workshop may:

- collect context
- structure reasoning
- identify missing evidence
- draft recommended next steps

Humans approve:

- dismissals
- severity changes
- risk acceptance
- remediation plans
- campaign creation

## Agenda

| Time | Topic |
| --- | --- |
| 0:00-0:05 | Framing: custom AppSec agents with GitHub Copilot |
| 0:05-0:20 | Layers and options for defining custom agents |
| 0:20-0:40 | Copilot Code Review instructions and AppSec skills |
| 0:40-1:00 | Local custom agents |
| 1:00-1:10 | Break |
| 1:10-1:30 | Repository-level custom agents used by a team |
| 1:30-1:50 | Local workflow automation with Copilot CLI or GitHub Copilot app |
| 1:50-2:20 | Copilot SDK app for alert triage |
| 2:20-2:30 | Review, discussion, and next steps |

## How to use these repos

For each section, open the matching repository and follow its README. The repositories are intentionally incomplete: they remove setup friction but still leave the design and implementation work to the attendee.

## Approved routes for alert triage

- `fix-now`
- `campaign-candidate`
- `needs-reachability-analysis`
- `needs-codeql-timeout-investigation`
- `human-escalation`

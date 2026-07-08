---
name: Scandesign Delivery
description: Delivery org for a Magento 2 ecommerce agency. A Delivery Lead reports to the human project lead and coordinates a Magento Solution Analyst, a QA Engineer, and an Account Coordinator across one project per client. PM, QA, and coordination only — no production code is written or merged.
schema: agentcompanies/v1
slug: scandesign-delivery
category: agency
key: paperclipai/optional/agency/scandesign-delivery
manager: agents/delivery-lead/AGENTS.md
includes:
  - agents/magento-analyst/AGENTS.md
  - agents/qa/AGENTS.md
  - agents/account-coordinator/AGENTS.md
  - projects/sample-client/PROJECT.md
defaultInstall: false
recommendedForCompanyTypes:
  - agency
  - ecommerce
  - services
tags:
  - agency
  - ecommerce
  - magento
  - hyva
  - delivery
  - qa
requiredSkills:
  - paperclipai/bundled/paperclip-operations/task-planning
  - paperclipai/bundled/paperclip-operations/issue-triage
  - paperclipai/bundled/quality/qa-acceptance
  - paperclipai/bundled/docs/doc-maintenance
  - paperclipai/bundled/product/wireframe
  - paperclipai/optional/browser/agent-browser
---

# Scandesign Delivery

Delivery org for **Scandesign Media**, a Magento 2 (Adobe Commerce) ecommerce agency. The human project lead acts as the board: you set client priorities and approve work; the team plans, specs, QAs, and coordinates it.

This org is intentionally **PM + QA + coordination only**. Agents do not write production code, do not push to client repos, and do not deploy. They turn client requirements into clear specs, acceptance criteria, status, and verification — and hand implementation to your human Magento developers.

## Contents

- `Delivery Lead` — root manager. Reports to the human project lead. Prioritizes across all client projects, keeps tickets moving with `task-planning` and `issue-triage`, watches budgets, and escalates blockers. The single point of contact between you and the team.
- `Magento Solution Analyst` — turns client requirements into Magento 2 technical specs and scopes (modules, third-party extensions, integrations, Hyvä frontend). Produces low-fi storefront wireframes with `wireframe`. Reviews technical approach; never writes production code.
- `QA Engineer` — writes acceptance criteria with `qa-acceptance` and runs manual/browser verification of Hyvä storefronts with `agent-browser`. Captures evidence before sign-off.
- `Account Coordinator` — drafts client-facing communication, status updates, and meeting notes, and keeps project docs current with `doc-maintenance`.
- `sample-client` — example project. Copy it once per ecommerce client (see the project file for the convention).
- `weekly-delivery-review` — recurring Delivery Lead heartbeat that reviews every client project and confirms the next useful action.

## How to run it

1. Set a clear company goal (e.g. _"Ship the open client backlog on time, on budget, with zero regressions in production"_).
2. Create one project per client by copying `projects/sample-client/`.
3. Seed each client project with the current backlog as tasks.
4. Let the weekly review heartbeat keep the org moving between your prompts.

## Guardrails

- No production code, repo pushes, or deploys. Implementation is handed to human developers.
- Never store client secrets, API keys, or customer/PII data in tickets or docs.
- Escalate anything touching payment, checkout, customer data, or go-live timing to the human project lead.

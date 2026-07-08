---
name: Sample Client
slug: sample-client
description: Template project for one ecommerce client. Copy this folder once per client (give it the client's slug) and seed the backlog as tasks.
owner: delivery-lead
---

Template project for a single Scandesign Media ecommerce client running Magento 2 (Adobe Commerce).

## How to use

Create one project per client by copying this folder under `projects/<client-slug>/` and updating
`name`, `slug`, and `description`. Keep all of that client's work — specs, QA, status, and the
backlog — inside their own project so context and budget never mix between clients.

## Flow

1. **Delivery Lead** seeds and prioritizes the backlog from the client's requirements.
2. **Magento Solution Analyst** turns each item into a Magento 2 spec (modules, extensions,
   integrations, Hyvä frontend) with acceptance-relevant detail for the human developers.
3. Human developers implement (outside Paperclip) and deliver to a staging environment.
4. **QA Engineer** verifies against acceptance criteria on staging and captures evidence.
5. **Account Coordinator** keeps the client informed and the project docs current.

## Per-client context to record here

- Magento version/edition and hosting (e.g. Adobe Commerce Cloud, on-prem).
- Frontend: Hyvä theme details, custom modules, key third-party extensions.
- Integrations: ERP, PIM, payment, shipping, search, marketing.
- Staging/test URLs and how QA gets access — **never** store credentials or secrets here.

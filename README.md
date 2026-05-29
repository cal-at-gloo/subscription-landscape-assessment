# SaaS Subscription UX — Landscape Assessment

**Live site:** https://cal-at-gloo.github.io/subscription-landscape-assessment/

A design research document analyzing seat management patterns, admin views, and subscription architecture across 9 major SaaS platforms. Created as input for a redesign spec for a multi-product workspace platform.

## Purpose

This research explores how complex, multi-product SaaS platforms handle:
- **Seat and member management** — how admins add, remove, and upgrade users
- **Admin vs. end-user views** — what the admin surface looks like vs. the member experience
- **Role and permission hierarchies** — layers between org-level admin and end user
- **Feature gating** — how plan differences are surfaced in-product
- **AI / usage metering** — credit and token models within subscription structures

## Platforms Covered

| Platform | Model Type |
|---|---|
| Monday.com | Multi-product, per-product seat pools |
| Google Workspace | Unified per-user license, OU-based delegation |
| Atlassian | Per-app subscriptions, centralized org hub |
| Figma | Unified seat-type model (post-March 2025) |
| Slack | Workspace/org hierarchy, RBAC overlay |
| Notion | Member/guest binary, seat recycling |
| Canva | Org → Team admin hierarchy, brand permission axis |
| Salesforce | 3-layer license × profile × permission model |
| Adobe Creative Cloud | Product profile templates, usage-based metering |

## Contents

- **`index.html`** — Full research document. Open in any browser or visit the live site above. Includes:
  - Platform-by-platform breakdowns with subscription architecture, admin UX notes, and design signals
  - A design pattern taxonomy with 6 cross-platform patterns identified
  - 6 design recommendations with platform inspiration cited
  - A proposed admin user path (6-step flow) for a multi-product workspace

## Key Findings

**Six design patterns identified:**
1. Unified seat with product-access flags *(Figma)*
2. Per-product seat pools *(Monday.com, Atlassian)*
3. Free tier + individual upgrade *(novel in Gloo's context)*
4. License as permission profile *(Adobe, Salesforce)*
5. Nested admin delegation *(Canva, Slack, Google)*
6. Usage-based resource meters within seats *(Figma, Adobe, Canva)*

**Top design signals:**
- Figma's seat request → 3-day temp access → approve/deny flow is the strongest self-service upgrade pattern found
- Atlassian's centralized org hub is the best reference for a multi-product member management view
- Monday's "Product Non-Member" concept elegantly handles users who exist in the workspace but haven't been assigned to a specific product
- Billing on invite (Atlassian anti-pattern) should be avoided — bill on acceptance/activation instead

## How to Use

Visit the **[live site](https://cal-at-gloo.github.io/subscription-landscape-assessment/)** or open `index.html` in a browser. No build step or dependencies required.

## Research Date

May 2026 — subscription models and feature sets change frequently. Verify against current platform documentation before finalizing any design spec.

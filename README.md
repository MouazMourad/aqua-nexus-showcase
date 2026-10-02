# Aqua Nexus

### The Brain of Your Aquarium

**Your aquarium has data. Aqua Nexus turns it into decisions.**

[Try Aqua Nexus](https://aqua-nexus-kappa.vercel.app) · **Marine + Freshwater** · **Arabic + English** · **PWA**

Aqua Nexus connects chemistry, livestock, maintenance, equipment, lighting, feeding, acclimation, alerts, history, and decision support in one operational platform.

> **Current status:** Release Candidate / controlled testing  
> **Source model:** Proprietary — production source code is maintained privately.

## Product tour

### 1. Tank Health & Next Action
Aqua Nexus summarizes the current direction of the aquarium, highlights risks, and surfaces the next practical action instead of leaving the user with raw numbers only.

### 2. Alerts → Actions
Operational alerts are connected to concrete workflows such as restocking consumables, reviewing bioload, and following up on aquarium events.

### 3. Digital Twin 3D
A visual model of the aquarium and sump helps connect tank dimensions, equipment, water flow, and the broader operating context.

### 4. Smart Dashboard
Chemistry, maintenance, bioload, tank intelligence, predictions, equipment, memory, and journey history are presented as connected domains rather than isolated pages.

> **Screenshots:** Official launch screenshots are being added to this public showcase. The live application is already available from the link above.

## Why Aqua Nexus?

Aquarium care is often spread across notebooks, spreadsheets, timers, test-kit logs, equipment apps, and memory. Aqua Nexus is designed to connect those pieces into one operational system.

Instead of treating every page as an isolated form, Aqua Nexus links meaningful events across the aquarium lifecycle so that chemistry, livestock, maintenance, equipment, and history can inform the next action.

## Core capabilities

- **Marine & Freshwater support**
- **Tank setup and lifecycle management**
- **Chemistry tracking and historical trends**
- **Livestock registry and health history**
- **Acclimation workflows**
- **Maintenance planning and printable checklists**
- **Equipment registry**
- **Lighting Intelligence with schedule and spectrum modelling**
- **Feeding, dosing, water-change and RO/DI tracking**
- **Quarantine and emergency workflows**
- **Inventory and consumables**
- **Reports and long-term history**
- **Arabic & English interface**
- **Local-first operation with recovery backup**
- **PWA experience for desktop and mobile**
- **Deterministic aquarium intelligence for operational guidance**

## Tank Brain

Aqua Nexus includes a deterministic decision layer called **Tank Brain**.

Its role is to connect meaningful events from different parts of the aquarium and surface relevant actions, warnings, or follow-up tasks.

Examples include:

- chemistry changes that require follow-up testing,
- livestock events that trigger water-quality checks,
- maintenance actions that affect later measurements,
- lighting changes that become part of the tank history,
- operational events that create reminders or safety checks.

Safety-sensitive aquarium decisions remain rule-based and auditable rather than being delegated blindly to generative AI.

## Lighting Intelligence

The lighting module is designed to go beyond a simple on/off schedule.

It includes:

- multi-channel schedules,
- spectrum representation,
- vendor-neutral lighting programs,
- top/front/3D visualization,
- estimated PAR modelling,
- coral or plant placement guidance,
- import workflows with editable review,
- history-aware lighting changes.

## Data & safety philosophy

Aqua Nexus is designed around several principles:

**Local-first:** core aquarium data remains usable without requiring a cloud account.

**Recoverable:** full recovery backups are treated as first-class product features.

**Auditable:** important operational changes are versioned or recorded where appropriate.

**Conservative automation:** high-risk aquarium actions require evidence, validation, or explicit user confirmation.

**No silent failure:** storage and validation failures should be surfaced to the user.

## Product architecture

The public architecture view is intentionally high-level:

```text
User
  ↓
Aqua Nexus UI / PWA
  ↓
Tank Domains
  ├─ Chemistry
  ├─ Livestock
  ├─ Maintenance
  ├─ Equipment
  ├─ Lighting
  ├─ Feeding / Dosing
  ├─ Acclimation
  └─ History
  ↓
Event & Validation Layer
  ↓
Tank Brain / Deterministic Rules
  ↓
Tasks • Alerts • Guidance • Reports
```

Detailed implementation, internal rules, private APIs, and production source code are intentionally not published in this repository.

## Current development focus

- reliability and regression closure,
- mobile/PWA polish,
- Arabic localization quality,
- reporting and maintenance workflows,
- long-term historical consistency,
- controlled expansion of Tank Brain intelligence.

See [ROADMAP.md](ROADMAP.md) for the public roadmap.

## Live product

**Aqua Nexus:** https://aqua-nexus-kappa.vercel.app

The public deployment may contain release-candidate functionality and is intended for evaluation and controlled testing.

## Feedback

Found a problem or have a product suggestion?

Use the repository **Issues** tab. Please avoid posting private aquarium data, credentials, API keys, or security-sensitive details publicly.

Security issues should follow [SECURITY.md](SECURITY.md).

## Source code & licensing

This repository is a **public product showcase and documentation repository**.

The Aqua Nexus production source code is **not open source** and is maintained privately.

Copyright © 2026 Mouaz Mourad. All rights reserved.  
See [LICENSE](LICENSE) for details.

---

### العربية

**Aqua Nexus** منصة ذكية لإدارة أحواض المياه المالحة والعذبة، تربط الكيمياء والأحياء والصيانة والإضاءة والمعدات والتغذية والإقلمة والطوارئ والسجل التاريخي ضمن نظام واحد مترابط.

هذا المستودع مخصص **للعرض العام والتوثيق واستقبال الملاحظات فقط**. الكود المصدري الفعلي للمنتج محفوظ في مستودع خاص وغير مفتوح المصدر.

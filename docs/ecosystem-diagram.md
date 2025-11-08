# BLUX Ecosystem Diagram

The BLUX ecosystem functions as an interconnected constellation of repositories. Each node honors collaboration, transparency, and personal sovereignty while enabling specialized capabilities.

```text
                                  ┌────────────────────┐
                                  │   blux-governance  │
                                  │  (policy + trust)  │
                                  └────────▲───────────┘
                                           │ provides guardrails
                                           │
┌────────────────────┐       consumes telemetry        ┌────────────────────┐
│    blux-design-    │◀───────────────────────────────▶│     blux-orbit     │
│       system       │        shares interaction        │  (realtime mesh)   │
│ (accessibility +   │        patterns & events         └────────▲───────────┘
│ composable UI)     │                                        │ streams intents
└────────▲───────────┘                                        │
         │ supplies themes                                   │
         │                                                    │
┌────────┴───────────┐                               ┌────────┴───────────┐
│     blux-core      │◀──── orchestrates services ───▶│ blux-experience-  │
│ (runtime + APIs)   │                                │       kit         │
└────────────────────┘                                │ (reference apps)  │
                                                      └────────────────────┘
```

## Repository Index

| Repository | Role | Key Relationships |
| --- | --- | --- |
| [`blux-core`](https://github.com/Outer-Void/blux-core) | Modular runtime powering orchestration and API contracts. | Depends on design tokens from [`blux-design-system`](https://github.com/Outer-Void/blux-design-system); streams events through [`blux-orbit`](https://github.com/Outer-Void/blux-orbit); governed by policies in [`blux-governance`](https://github.com/Outer-Void/blux-governance). |
| [`blux-orbit`](https://github.com/Outer-Void/blux-orbit) | Realtime collaboration mesh handling intents and telemetry. | Feeds analytics to [`blux-governance`](https://github.com/Outer-Void/blux-governance); coordinates sessions for [`blux-experience-kit`](https://github.com/Outer-Void/blux-experience-kit); ingests schema updates from [`blux-core`](https://github.com/Outer-Void/blux-core). |
| [`blux-design-system`](https://github.com/Outer-Void/blux-design-system) | Accessible component and token library aligning visual language. | Supplies themes to [`blux-core`](https://github.com/Outer-Void/blux-core) plugins; documents patterns applied in [`blux-experience-kit`](https://github.com/Outer-Void/blux-experience-kit); adheres to standards from [`blux-governance`](https://github.com/Outer-Void/blux-governance). |
| [`blux-experience-kit`](https://github.com/Outer-Void/blux-experience-kit) | Playable demos and starter apps showcasing sovereign workflows. | Demonstrates how [`blux-core`](https://github.com/Outer-Void/blux-core) modules and [`blux-design-system`](https://github.com/Outer-Void/blux-design-system) assets combine; streams activity through [`blux-orbit`](https://github.com/Outer-Void/blux-orbit); documents learnings back to [`blux-governance`](https://github.com/Outer-Void/blux-governance). |
| [`blux-governance`](https://github.com/Outer-Void/blux-governance) | Policy, legal, and community guidelines for transparent stewardship. | References telemetry agreements in [`blux-orbit`](https://github.com/Outer-Void/blux-orbit); enforces consent standards for [`blux-experience-kit`](https://github.com/Outer-Void/blux-experience-kit); defines contribution protocols across all repositories. |

## Using the Diagram

- **Onboarding** – Share this map with new contributors so they can identify the repositories aligned with their skills.
- **Planning** – Reference the relationships column when scoping cross-repo initiatives to ensure stakeholders are invited early.
- **Reviewing** – During retrospectives, validate that changes respected the ethical guardrails and brand commitments documented across this repository.

This diagram is updated as the constellation evolves. Propose additions via pull request and include the rationale in the [README overview](../README.md).

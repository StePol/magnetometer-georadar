# Technical decisions — Magnetometer / Georadar

Updated: 2026-11-08

| Status | Decision | Rationale |
|---|---|---|
| Accepted | Maintain a standalone magnetometer-georadar repository. | Separation from other projects. |
| Accepted | GitHub is the canonical source of technical documentation. | Versioning and access across devices. |
| Accepted | Maintain shared AI context in `docs/AI/`. | ChatGPT, Zed and Codex may have separate conversation contexts. |
| Accepted | Begin with a single K49E sensor test. | Characterize feasibility before scaling. |
| Concept | Support more than seven sensors, potentially 8/12/16/24+, with two references. | Flexible array design and experimental common-mode correction. |
| Concept | Smartphone Wi-Fi interface and authoritative local raw-data storage. | Field operation without requiring a continuous phone connection. |
| Deferred | Exact ADC, sensor count, reference types and mechanical design. | Need measured performance first. |

Record future changes with date, evidence and justification. Do not promote concepts to verified design decisions without tests.

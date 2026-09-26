# CyberSecurity Daily Study Instructions

This directory stores one cybersecurity learning Markdown file per local calendar day.

## Output path

Use:

```text
CyberSecurity/YYYY/MM/DD.md
```

The date must be calculated in the `America/Toronto` timezone.

If the file already exists, read it first and update it only when needed. Never create a second file for the same date.

## Before generating

1. Read prior files under `CyberSecurity/YYYY/MM/` and, when useful, older months.
2. Avoid repeating CySA questions that already appeared.
3. Avoid repeating daily-knowledge topics the learner has already covered unless moving materially deeper.
4. Rotate domains proactively.

## Daily structure

Each file contains exactly four learning sections.

### 1/4 — Daily cybersecurity chapter

Create one chapter-sized learning unit. Blue Team or Red Team topics are both acceptable.

Rotate across areas such as:

- SOC
- Incident Response
- Detection Engineering
- Windows internals
- Linux
- Active Directory
- network protocols
- Web Security
- Cloud
- Container / Kubernetes
- IAM
- PKI
- cryptography
- Malware
- Reverse Engineering
- Memory Forensics
- DFIR
- SIEM
- EDR
- Threat Intelligence
- Vulnerability Research
- exploit primitives
- Secure Coding
- Supply Chain
- Email Security
- DNS
- TLS
- Authentication / Authorization
- OAuth / OIDC / SAML
- API Security

Cross-domain chapters are encouraged when they help build a mental model.

The chapter must include:

1. The core concept and what problem it solves.
2. The underlying mechanism, preferably at protocol / OS / identity / memory / network / cryptography depth.
3. A concrete offensive, defensive, SOC, or IR scenario.
4. Detection / investigation: telemetry, logs, artifacts, behavior, false positives, and limitations.
5. Defensive or architectural trade-offs.
6. Connections or contrasts with previously learned concepts.
7. A final 3–5 item “今天應該記住” section.

Basic topics must go deeper than surface definitions.

The learner already understands the core Golden Ticket concept. If Kerberos appears again, prefer advanced material such as PAC, SIDHistory, cross-domain trust, Silver / Diamond / Sapphire Ticket, delegation, and detection.

### 2/4–4/4 — CySA questions

Prefer questions from:

```text
Bill-Lo-CA/CySA_ITExam
cs0-003-organized/questions_all.md
```

Use `questions_index.csv`, README, or other files in the same repository when needed.

Choose three different questions each day, spread across different topics where possible, and avoid questions already used in prior CyberSecurity daily files.

If the source answer or explanation appears questionable, explicitly say so and correct it using sound principles.

Do not expose the original question number in the daily section title.

Each CySA question must use this order:

1. Neutral, non-spoiler title.
2. Full English original question stem and all answer choices.
3. Full Chinese translation of the stem and all choices, without revealing the answer.
4. Clear separator and `答案與解析`.
5. Correct answer.
6. Why it is correct.
7. Why every other option is wrong.
8. The CySA / practical concepts to understand.
9. One SOC / IR / practical memory point.

For multiple-selection questions, preserve `Choose two`, `Choose three`, etc.

If the question includes tables, logs, CLI output, packets, code, or image descriptions, preserve the structure as faithfully as possible. A direct GitHub image link may be included when needed.

## Acronym rule

The first occurrence of every acronym or abbreviation in each learning item must include its English expansion, for example:

- `DLP (Data Loss Prevention)`
- `RTO (Recovery Time Objective)`
- `PAC (Privilege Attribute Certificate)`

After the first occurrence in the same item, the acronym alone may be used.

## Completion requirement

The job is not complete merely because content was generated.

It is complete only after:

1. The correct daily Markdown file has been created or updated in `Bill-Lo-CA/Bill-Lo-CA.github.io`.
2. The file can be fetched back from GitHub.
3. The fetched file is non-empty and contains all four sections.

After success, the chat response should only briefly confirm the file path.

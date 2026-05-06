# Contract Lifecycle Management (CLM)

> Part of the [worlds-biggest-software-project](https://github.com/worlds-biggest-software-project) initiative.
>
> An AI-native, open-source contract lifecycle platform that brings playbook-driven redlining, obligation tracking, and portfolio risk visibility to organisations priced out of enterprise CLM.

Contract Lifecycle Management (CLM) is an open-source platform for drafting, redlining, approving, signing, storing, and tracking contracts across their full lifecycle. It is aimed at startups, mid-market organisations, law firms, and legal aid groups who currently manage contracts in shared drives because tools like Ironclad and Icertis are out of reach. The project pairs a configurable workflow engine with AI clause review against a customer-defined playbook.

---

## Why Contract Lifecycle Management?

- **Enterprise CLM is unaffordable below the upper mid-market**: Ironclad runs $25K–$75K+/year, DocuSign CLM $30K–$120K+/year, and Icertis $150K–$1M+/year — pricing that excludes Series A–D startups and most mid-market firms.
- **The only existing OSS option is nascent**: OpenCLM is the sole credible open-source CLM, but is early-stage, lacks enterprise validation, and has only basic AI features compared to commercial incumbents.
- **AI playbook redlining is locked behind expensive licences**: Ironclad's Redlining Agent and Icertis's clause analysis are proprietary IP; no OSS CLM offers comparable AI-driven deviation detection or fallback-language suggestions.
- **Missed obligations cost real money**: contracts contain hundreds of dates, notice periods, and renewal windows; most non-enterprise teams track them in spreadsheets and lose revenue or auto-renew unwanted commitments.
- **General Counsels lack portfolio risk visibility**: cross-portfolio risk dashboards (e.g., "what share of revenue contracts have uncapped liability?") are only available in Icertis at $1M+/year.

---

## Key Features

### Intake, Drafting & Templates

- Configurable web-form contract intake with routing rules by contract type, value, and counterparty
- Template library with variable substitution for standard agreements (NDA, MSA, SoW, offer letter)
- Clause library aligned to organisation-specific preferred language
- Counterparty-facing draft sharing with revision tracking

### AI Playbook Review & Redlining

- AI clause review against a configurable playbook: flag non-standard clauses with deviation reasons
- Suggested fallback language drawn from the clause library
- Contract summarisation in plain English for non-legal stakeholders
- Clause similarity clustering across the repository to support playbook refinement

### Approval, E-Signature & Audit

- Configurable approval workflow with role-based authority levels and escalation paths
- Email and notification-based routing with full audit trail
- E-signature integration via DocuSign or Adobe Sign APIs, with a lightweight native option
- Audit-trail export suitable for SOX and SOC 2 evidence

### Repository, Obligations & Renewals

- Contract repository with full-text search, metadata tagging, and version history
- AI-driven obligation extraction: structured ledger of dates, owners, and SLA thresholds from executed contracts
- Renewal and expiry alerting with configurable lead times
- Conversational natural-language query of contract data ("which contracts have uncapped liability?")

### Portfolio Risk & Analytics

- Aggregate clause risk scoring across the entire repository
- Executive risk dashboard for clause concentration, obligation exposure, and renewal risk
- Cycle-time and approval-bottleneck analytics for legal ops

---

## AI-Native Advantage

Unlike rules-based legacy CLM, this project is built around an open LLM clause-review engine: a configurable playbook drives automated detection of non-standard counterparty language and proposes specific redline text rather than merely flagging issues. AI also extracts every obligation from executed contracts into a live tracker, replacing the spreadsheet workflow that causes missed renewals, and scores the full portfolio for risk concentrations. These capabilities — playbook redlining, obligation extraction, and portfolio risk scoring — are today only fully available in commercial tools costing $25K to over $1M per year.

---

## Tech Stack & Deployment

The platform is designed for self-hosted deployment as the primary mode, with an API-first architecture and webhook events for embedding CLM into HRIS, ERP, CRM, and procurement systems. Integration targets include Salesforce, HubSpot, Microsoft 365, SAP, Slack, and SSO providers (Okta, Azure AD). Standards support covers UNCITRAL Model Law, eIDAS (including Qualified Electronic Signatures), ESIGN/UETA, GDPR/CCPA data-handling, ISO/IEC 27001, and SOX / SOC 2 Type II audit evidence. Where helpful, the clause library can embed IACCM/WorldCC published playbook standards.

---

## Market Context

The global CLM software market is approximately $2.6B–$2.96B in 2025 (IMARC, GMI, Precedence Research) and is projected to reach $5.7B–$8.84B by 2034–2035 (CAGR 9.2%–11.56%); cloud-based CLM accounts for over 63% of the market. Commercial pricing ranges from $25K/year mid-market entry (Ironclad, Summize) to $1M+/year for large-enterprise platforms (Icertis), while the only OSS alternative (OpenCLM) is free but unvalidated. Primary buyers are General Counsels, Legal Operations Managers, Procurement Directors, Sales/Revenue Operations, and CFOs.

---

## Project Status

> This project is in the **research and specification phase**.  
> Contributions, feedback, and domain expertise are welcome.

---

## Contributing

We welcome contributions from developers, domain experts, and potential users.
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Important:** All contributions must be your own original work or clearly attributed
open-source material with a compatible licence. Copyright infringement and licence
violations will not be tolerated and will result in immediate removal of the offending
contribution. If you are unsure whether a piece of code, text, or other material is
safe to contribute, open an issue and ask before submitting.

---

## Licence

Licence to be determined. See [discussion](#) for context.

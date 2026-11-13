# Evidence, sources and limits

**Review date:** November 13, 2026. **Locke Prime source:** `Amishgangsta/Locke-Prime`, commit `ebdc609cf5311d724bca9a5c8cb29ec14efc90ca`; private source inspected read-only. GitHub and Railway metadata showed a successful production deployment of the same commit at the time of review. No tests, production transactions, or third-party account trials were run for this report.

## Comparison groups

- Clio = Clio Manage + Clio Work/Vincent, potentially separately licensed.
- Filevine = Filevine + LOIS and related packages, potentially separately licensed.
- Litify = Litify platform + Litify ACE AI offerings.
- MyCase = 8am MyCase + 8am IQ (Advanced tier and beta-specific capabilities).
- Smokeball = Smokeball + Archie (eligible plans and integrations).

All vendor comparisons are based on public product/support sources, not identical paid plans. A feature code of **Comparable** means similar function was described, not measured parity for reliability, UX, jurisdictional breadth, or legal accuracy. **Not established** cannot justify an assertion that a vendor lacks a capability.

## Current primary sources

| Ref | Provider | Source | Link |
|---|---|---|---|
| L01 | Locke Prime | Private source snapshot, main ebdc609cf531 | [Official source](https://github.com/Amishgangsta/Locke-Prime) |
| L02 | Locke Prime | Red-team PR #26, merged November 12 ET | [Official source](https://github.com/Amishgangsta/Locke-Prime/pull/26) |
| C01 | Clio | Clio Work/Vincent: matters, research, drafting and actions (Nov 2026) | [Official source](https://help.clio.com/hc/en-us/articles/48791655710235-Understand-Clio-Work) |
| C02 | Clio | Build Arguments: evidence, risk, opposing challenges (Aug 2026) | [Official source](https://help.clio.com/hc/en-us/articles/41752991031323-Build-Arguments-in-Clio-Work) |
| C03 | Clio | Clio Work document editor (Nov 2026) | [Official source](https://help.clio.com/hc/en-us/articles/53031641830939-Document-Editor) |
| C04 | Clio | New 2026 Clio AI workflows/approval points | [Official source](https://www.clio.com/about/press/clio-unveils-legal-ai-product-launches/) |
| F01 | Filevine | LOIS overview: firm-wide AI and actions (Oct 2026) | [Official source](https://support.filevine.com/hc/en-us/articles/51146162307611-Welcome-to-LOIS) |
| F02 | Filevine | LOIS Legal Research verification (Sep 2026) | [Official source](https://support.filevine.com/hc/en-us/articles/55094400475931-LOIS-Legal-Research) |
| F03 | Filevine | LOIS Workflows: event/schedule triggered automation (Aug 2026) | [Official source](https://support.filevine.com/hc/en-us/articles/47889381053467-LOIS-Workflows) |
| LIT01 | Litify | Litify ACE: AI case expert, retrieval, agents (2026) | [Official source](https://www.litify.com/blog/introducing-litify-ace-the-agentic-case-expert) |
| LIT02 | Litify | Litify AI module and agents | [Official source](https://www.litify.com/litify-ai) |
| M01 | MyCase | 8am IQ Case Assistant, matter documents and citations (Aug 2026) | [Official source](https://supportcenter.mycase.com/en/articles/12267713-8am-iq-case-assistant) |
| M02 | MyCase | AI Case Assistant product details | [Official source](https://www.mycase.com/features/ai-case-assistant/) |
| M03 | MyCase | 8am IQ prompt library (June 2026) | [Official source](https://supportcenter.mycase.com/en/articles/15327201-8am-iq-case-assistant-prompt-library) |
| S01 | Smokeball | Archie AI matter assistant, task creation and citations | [Official source](https://support.smokeball.com/hc/en-us/articles/24407844681751-Getting-Started-with-Archie-the-Smokeball-AI-Assistant) |
| S02 | Smokeball | Archie confirmation before saving tasks, memos, events (May 2026) | [Official source](https://support.smokeball.com/hc/en-gb/articles/39618100098967-Creating-tasks-memos-and-events-with-Archie) |
| S03 | Smokeball | Archie Word / Outlook / playbooks product | [Official source](https://www.smokeball.com/archie-ai) |

## Material limitations

- Clio Work, Filevine LOIS and Litify ACE have rich matter-aware AI, and Smokeball Archie offers approval-gated actions; therefore the words “only,” “first,” and “best” are not justified as factual comparative superiority.
- Clio Work and Filevine LOIS have stronger public legal research-library and citation verification claims than Locke's documented third-party LawDiver/CourtListener adapter integration; they are not represented as weaker on that function.
- Filevine's live deposition assistance and mature cross-firm workflows are not equivalent to Locke's War Room.
- Billing, native payment collection, trust accounting, client portal breadth, and court filing are not established as equivalent full Prime capabilities in the inspected source.
- Past Claude red-team tests and merged mitigations were reviewed as historical evidence, not repeated or independently certified. Any historical key-rotation or security-operations questions were **not** verified closed during this review.
- The current Ask Locke grounding validator emits warnings when citations are absent, not independent fact-proof for every generated proposition.
- Product source presence does not establish uptime, customer adoption, benchmark superiority, compliance certification, or outcome quality.

## Where the project demonstrates engineering depth

Backend API routing; PostgreSQL persistence; multi-tenant and matter-level permissions; retrieval, OCR and chunk indexing; model routing; external legal-source adapters; structured outputs; confirmed-action validation; collaborative browser interfaces; PDF/DOCX export; security remediations; code/test/release governance; Railway deployment.

**Purpose:** This is a software engineering portfolio and capabilities report for organizations evaluating Locke Development's work or considering employment. It is not a solicitation to consumers to purchase legal-document services.
# ASK LOCKE — FROM CONTEXT TO CONTROLLED ACTION

### A 20-point technical and competitive analysis · November 13, 2026

**Ask Locke is not merely a branded chatbot.** The inspected current implementation retrieves matter evidence, emits source metadata, provides context-sensitive assistance, and separates proposed actions from user-confirmed changes. The coverage below records the actual product surfaces rather than hiding them under a single AI row.

## What the current source implements

**Know the matter.** Active matter metadata (name, status, type, stage, court, judge and next deadline) is incorporated into the prompt. Relevant chunks from the matter's indexed documents are retrieved and passed as context, with file/page details when available. History is bounded to the latest 20 messages.

**Expose the evidence.** Retrieved documents can be referenced by document number or filename; the API provides source citations, snippets, page/chunk information and grounding labels. Citation-guard code adds legal-authority verification annotations and negative-treatment warnings when the applicable provider is available. The presence of these checks is not a guarantee that all statements are correct.

**Know the working context.** The assistant also receives page and CLM entitlement context. A dedicated research mode returns matter-document search results without producing an unrestricted generative answer.

**Turn intent into action — with approval.** Ask Locke recognizes proposed `add_deadline`, `add_task`, and `add_note` actions, validates the supported fields and dates, and presents proposals for the attorney to confirm; the model cannot save those actions merely by writing a response. Collaboration-thread assistance can also use the thread and its matter documents.

## Twenty individual competitor checks

| Locke Prime capability | Locke | Clio | Filevine | Litify | MyCase | Smokeball |
|---|:---:|:---:|:---:|:---:|:---:|:---:|
| Matter-specific assistant in the application | **Source** | Comparable | Comparable | Comparable | Comparable | Comparable |
| Active matter metadata in responses | **Source** | Comparable | Comparable | Comparable | Comparable | Comparable |
| Retrieval of matter documents for chat | **Source** | Comparable | Comparable | Comparable | Comparable | Comparable |
| Page-aware references to source documents | **Source** | Comparable | Comparable | Related | Related | Comparable |
| Source-linked document citations | **Source** | Comparable | Comparable | Comparable | Comparable | Comparable |
| Grounding and confidence labels | **Source** | Comparable | Comparable | Comparable | Comparable | Comparable |
| Warning when answers omit retrieved citations | **Source** | Comparable | Comparable | Related | Comparable | Comparable |
| Legal citation verification annotations | **Source** | Comparable | Comparable | Related | Related | Comparable |
| Warnings for negative treatment of authorities | **Source** | Comparable | Comparable | Related | Related | Related |
| Dedicated matter-document research mode | **Source** | Comparable | Comparable | Related | Comparable | Comparable |
| Page/CLM entitlement context passed to assistant | **Source** | Related | Related | Related | Related | Related |
| Conversation history retained in chat request | **Source** | Comparable | Comparable | Comparable | Comparable | Comparable |
| Assistant proposes matter deadline creation | **Source** | Comparable | Comparable | Comparable | Related | Comparable |
| Assistant proposes matter task creation | **Source** | Comparable | Comparable | Comparable | Related | Comparable |
| Assistant proposes matter note creation | **Source** | Comparable | Comparable | Comparable | Related | Comparable |
| Explicit attorney confirmation before saving | **Source** | Comparable | Related | Related | Related | Comparable |
| Validates action type, dates, and limits | **Source** | Related | Related | Related | Related | Related |
| Executes confirmed actions under user/matter scope | **Source** | Comparable | Comparable | Comparable | Related | Comparable |
| Assistance inside matter collaboration threads | **Source** | Related | Related | Related | Related | Related |
| OpenAI provider with configured fallback adapter | **Source** | Related | Related | Related | Related | Related |

## The competitive conclusion

- **Clear parity:** Clio Work/Vincent, Filevine LOIS, and Smokeball Archie also have matter-grounded assistance; MyCase and Litify have contextual legal AI as well.
- **Not exclusive:** Smokeball explicitly documents confirmation before saving tasks, events and memos; Clio and Filevine support AI actions, and Litify describes autonomous workflows. The approval gate is an implementation strength, **not an invented exclusive feature**.
- **Distinguished composition:** Locke connects assistant actions to its Boardroom, War Room, document memory and CLM workflows inside one privately maintained codebase. The public materials reviewed do not prove that this makes it objectively better than competing suites.
- **The defensible story for hiring and contracting:** matter-aware retrieval, source metadata, structured model-output normalization, access enforcement, explicit human confirmation and auditable persistence are substantive full-stack AI engineering skills.

### Implementation boundaries

The assistant's `chat_rag` validator warns when retrieved citations are not referenced; it does not independently verify that every claim is semantically supported. Model adapters exist, but the most recent red-team handoff stated OpenAI was the active provider. This review inspected source but did not run fresh Ask Locke conversations or independent vendor tests.

[**Method and primary sources**](METHODOLOGY.md)
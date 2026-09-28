---
title: "AI Requirements for CRE Underwriting: A Complete Governance Guide"
series: "The Governed AI Series"
part: "Part III — Govern It Over Time"
eyebrow: "GOVERN IT OVER TIME"
deck: "The anchor for the underwriting pieces: which frameworks an owner asks counsel about, what a human still signs, and the file that has to exist before a model output becomes a credit input."
author: "Cypress Command"
date: "2026-09-28"
read_time: "18 min"
desk: "own"
status: "review"
source: "batch-e"
---

# AI Requirements for CRE Underwriting: A Complete Governance Guide

The underwriting articles in this batch describe what a model may prepare: a rent roll, a trailing twelve-month statement, a sponsor spread, a multifamily loss-to-lease schedule. None of that preparation is a credit decision. This guide is the anchor those pieces assume. It names the frameworks an owner asks counsel about, the oversight a named person has to be able to exercise, and the records that have to exist before anyone treats a model output as an input to a loan, a purchase, or a recommendation to a partner.

Cypress Command does not classify a reader's system, and this article does not. Whether the EU Artificial Intelligence Act, the Equal Credit Opportunity Act, the Fair Housing Act, or the Gramm-Leach-Bliley Act reaches a given workflow is a question for qualified counsel. The operating rule below does not wait on that answer. A model prepares. A named person decides. Every material figure cites a page.

## What the shorter articles already cover

The Governed AI Series already has the working tools. "AI in CRE Underwriting: What the Model Prepares and What the Owner Signs" is the boundary worksheet. "The AI Use Register," "Prepare, Recommend, Decide," "Data In, Data Out," "The Audit Trail," and "A One-Page AI Policy an Owner-Led Business Can Actually Follow" are the pages a small team can actually keep. This guide is the longer map those pages sit on when the work is underwriting: credit files, borrower financials, and property income.

If a use does not touch a credit decision or a person's financial information, do not import a bank's control set. Write the boundary, name the owner, and stop. If the use does touch credit or borrower financials, the rest of this guide is the list to take to counsel and to the person who will sign.

## Name the frameworks before you name the tool

Four instruments come up whenever AI is put in front of a credit file. They are not interchangeable, and they do not all apply to every owner.

| Instrument | What it is | The question to ask counsel |
|---|---|---|
| EU AI Act (Regulation (EU) 2024/1689) | A risk-based statute. Annex III lists creditworthiness assessment and credit scoring among high-risk uses. Obligations phase in over several years after the August 2024 entry into force. | Does any output of this tool affect a person or business in the EU, or are we a provider or deployer the Act reaches? |
| NIST AI Risk Management Framework | A voluntary U.S. framework organized as Govern, Map, Measure, and Manage. Financial uses are commonly treated as higher impact inside that framework. | Which of the four functions will we actually run, and who owns each? |
| ECOA, Regulation B, and the Fair Housing Act | Federal fair-lending statutes. They follow the decision, including when a model contributed to it. Adverse-action notices have to state principal reasons. "The model scored you low" is not a reason. | Is this workflow a credit decision about a person or a dwelling, or only an investment memo about a property? |
| Gramm-Leach-Bliley Act Safeguards Rule | A privacy and security rule for customer financial information held by financial institutions and their service providers. | Are we, or is our vendor, holding customer financial information the rule covers? |

Shopping-center rent rolls and owner operating statements are not automatically "credit scoring." A lender spreading a guarantor's tax return is a different use from an owner summarizing a seller's T12. Write the use down before anyone imports a high-risk label. The label, if it applies, is counsel's.

## Human oversight is an operating rule

Whatever counsel concludes about classification, the file still needs a person who can see the work. Article 14 of the EU AI Act is often cited for a specific duty on high-risk systems: a natural person who understands the tool's limits, can watch it, can interrupt it, and is not expected to rubber-stamp it. An owner-led business can run the same duty without waiting for a formal classification.

- Final authority for the underwriting outcome sits with a named person, not with the model.
- The model's job is written down as prepare or recommend. It does not approve, decline, or send terms.
- The reviewer has been shown what the tool misses: scanned pages, missing exhibits, a co-tenancy clause in an amendment, a K-1 that is not cash.
- Each file records who decided, what they changed, and why.
- An override is a log entry: name, time, and the sentence that explains the change.
- Decision records are kept for the period counsel names. Regulation B's recordkeeping rule is commonly cited at 25 months for many creditors. Confirm the period that applies. Do not invent a shorter one for convenience.

A signature on a memo the reviewer did not read is not oversight. If the reviewer cannot open the cited page and check the figure in a few minutes, the citation is decorative.

## What the file has to contain

Technical documentation is how a later reader — a partner, a lender, an examiner, a successor — reconstructs the decision. Keep it as a folder, not a manifesto.

| Record | What it holds | When it is updated |
|---|---|---|
| Use description | What the tool prepares, what it must not do, who signs | When the use changes |
| Inputs | The document list, versions, and what was missing | Each file |
| Outputs | The draft, with page or cell citations on material figures | Each file |
| Changes | Overrides, with name, time, and reason | Each file |
| Checks | Bias, variance, or sampling notes counsel or the owner required | On the cadence below |
| Vendor file | Contract limits, what the vendor may see, how to get the data back | Before the tool is turned on, then yearly |

Explainability tools are a means, not a badge. SHAP and LIME are two common ways to show which inputs moved a score. A plain reconciliation — "NOI changed because the management fee was normalized to 5 percent of effective gross income, source T12 page 2" — is often the explanation a credit file actually needs. If the decision is adverse to an applicant, counsel reviews the words that go on the notice. The model does not draft that notice unsupervised.

## Fair lending is not an intention test

If the workflow is credit, fair-lending law cares about outcomes, not about whether anyone meant to discriminate. Proxy risk is the ordinary failure: a variable that looks neutral and tracks a protected characteristic. Geography, neighborhood condition scores, and income patterns built on old lending files are the examples counsel will ask about. The operator's job is to list the inputs and refuse any input the team cannot explain in one sentence.

Protected characteristics that fair-lending conversations typically name include race, color, national origin, sex, religion, age, marital status, disability, and familial status. Some states and programs add others. The list is counsel's. The operator's rule is shorter: do not feed the model a field you would not be willing to defend, and do not let a vendor's "enrichment" add one in the background.

## Vendors do not carry the signature

A contract does not move the decision off the owner. Before a vendor sees owner financials or a borrower file, ask, in writing:

- What does the tool read, and what does it store?
- Can we audit a single figure back to a page?
- Who tests for biased outcomes, and will we see the test?
- What happens to our documents if we leave?
- Can an examiner or our counsel see the same records we can?
- Which actions can the tool take without a person: none, draft only, or write into the books?

"Data In, Data Out" is the shorter version of the same gate. If the vendor cannot answer, the tool waits.

## Shopping-center uses fail in familiar places

Retail underwriting gives a model more ways to look complete and be wrong. These are operating risks, not a score Cypress Command assigns.

- **Anchor dependence.** A co-tenancy clause can cut inline rent if an anchor goes dark. A rent roll will not show it. The lease will.
- **Sales clauses.** Percentage rent and kick-outs depend on tenant sales the model does not have unless someone provided them.
- **Rollover clumps.** A year with a large share of rent expiring is a financing fact. The model should list it, not smooth it.
- **Stale comps.** A cap rate or rent comp from a different year or trade area is not a fact about this center.
- **Inconsistent owner books.** The same property described three ways in a T12, a tax return, and a rent roll is a stop, not an average.

"How to Normalize a T12 Statement for CRE Underwriting" and "AI Requirements for CRE Underwriting: Shopping Centers and Owner Financials" are the working versions of those risks. This guide is why their outputs stay drafts until a person signs.

## A sequence an owner can actually run

The source material for this guide laid the work out in four phases. The sequence below keeps that order and drops the assumption that every reader must stamp the system "high-risk" on day one. Counsel's classification, if one is required, is a task inside phase one, not a slogan.

**Weeks 1–4. Write the use down.** Name the tool, the documents it may see, and the decisions it may not make. Appoint the person who signs. Ask counsel which of the four frameworks apply. Sample a past file: can every material figure be opened to a page? Read the vendor contract for audit rights and for what happens to the documents.

**Months 2–3. Build the folder.** Adopt the one-page policy. Open an AI use register. Write a one-page incident note: who is called when a figure is wrong, when a borrower complains, or when data leaves the firm. Decide how an adverse reason, if the use is credit, will be written. Start a simple log of overrides.

**Months 4–6. Harden what counsel said applies.** Train the people who touch outputs: what the tool is good at, what it invents, how to override, what they may not paste into a prompt. If counsel requires a bias review, an impact assessment, or a security review, commission that review and keep the report in the folder. Set a retention rule and follow it.

**After that. Keep a cadence.** Quarterly, read the override log and one live file. Yearly, reread the policy, the vendor answers, and counsel's list of frameworks. When the model changes, stop and review before the next file, as "When the Model Changes Under You" describes.

## Practices that break the file

Treat these as stops, not as style preferences.

- A credit outcome with no named reviewer.
- A material figure with no page or cell.
- An adverse reason that cites the model instead of a fact.
- A field the team cannot explain, left in because the vendor turned it on.
- Borrower or owner financials used to train a vendor's model without a written answer on consent and retention.
- No note for what happens when the output is wrong.
- A model that has not been looked at since installation, still treated as current.

## A review table

Use this as the board or partner page. Status is filled by the owner, not by this article.

| Obligation | Where it comes from | What "done" looks like | Cadence |
|---|---|---|---|
| Use written down | Owner policy; counsel's list of frameworks | One paragraph: prepares, must not, who signs | On change |
| Human decision | Operating rule; EU AI Act Art. 14 where counsel says it applies | Named reviewer on each file | Every file |
| Citations | Audit trail | Page or cell on material figures | Every file |
| Fair-lending inputs | ECOA, FHA, where the use is credit | Input list a person can defend | Before go-live, then yearly |
| Explanations | Regulation B, where the use is credit | Principal reasons in words counsel has seen | Every adverse file |
| Vendor limits | Contract and GLBA analysis | Written answers on storage, audit, exit | Before go-live, then yearly |
| Training | The people who touch outputs | A short session, a sign-in, a date | Yearly and on model change |
| Incident note | Owner | Who is called, what is preserved | Yearly drill |
| Reporting | Owner | Override count, open incidents, counsel updates | Yearly, sooner if something breaks |

Three conditions make the table real. Someone at the top of the firm owns it, not only the person who installed the tool. The people who see bad outputs can say so without being punished for the news. And the folder is the governance. A policy that points at an empty folder is a slogan.

### The view from Arnould Blvd

On The Blvd is a legacy multi-tenant center at 101–149 Arnould Blvd in Lafayette, roughly 63,000 square feet, 27 units, two buildings, run with Command Platform as the lease record. Nothing in this guide is a credit file for that property, and no rent, NOI, or loan term is stated. The plate is the boundary. A model can be handed the leases the platform already holds. It still cannot see a recorded constraint that was not in the packet, and it still cannot sign. The owner signs. The same sentence is the whole governance program until the folder above exists.

## The practical next step

1. Pick one live underwriting use: a T12, a rent roll, or a sponsor spread. Write one sentence on what the model may prepare and one sentence on what it may not do.
2. Name the person who signs that file. If you cannot name them, the tool is not in use yet.
3. Open the last output and mark every material figure that has no page or cell. Those marks are the first audit.
4. Send counsel the four-row framework table and ask which rows apply to this use. File the answer.
5. Point the team at the one-page policy and at this guide. The policy is what they follow. This guide is what they open when the use is credit.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*

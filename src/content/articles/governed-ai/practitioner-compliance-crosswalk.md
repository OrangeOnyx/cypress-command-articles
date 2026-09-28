---
title: "A Compliance Crosswalk for CRE Underwriting AI"
series: "The Governed AI Series"
part: "Part III — Govern It Over Time"
eyebrow: "GOVERN IT OVER TIME"
deck: "One grid that shows how six frameworks ask for the same underwriting controls, so a review is a gap list instead of six separate binders."
author: "Cypress Command"
date: "2026-09-28"
read_time: "10 min"
desk: "own"
status: "review"
source: "practitioner-reference"
---

# A Compliance Crosswalk for CRE Underwriting AI

The Governed AI Series is explicit that a policy is not a compliance claim. This practitioner reference is the grid behind that warning. It lines up six frameworks people wave at an underwriting model — the NIST AI Risk Management Framework, the EU AI Act, ISO/IEC 42001, ECOA, the Fair Housing Act, and GLBA — against the same set of controls. The other pieces in this suite are the procedures. This is the index: which control satisfies which ask, which asks do not apply to you, and what is still a gap.

Do not start by stamping the tool "high-risk." Annex III of the EU AI Act includes certain creditworthiness and credit-scoring systems. ECOA and the Fair Housing Act apply only to the decisions they cover. GLBA applies to customer financial information held by the institutions it covers. NIST is voluntary. ISO/IEC 42001 is a certifiable management system, not a statute. Counsel marks each column applicable, not applicable, or unknown. You still build the controls that would matter if the strictest applicable column is yes. Unknown is not a reason to leave the cell blank. It is a reason to ask.

The figures and article numbers below are a map for a conversation with counsel. They are not an opinion that your system is in scope, and they will go stale as guidance moves. Recheck citations before you put them in a letter to a regulator or a lender.

## How to use the grid

Read the classification section once with counsel. Use the master map as the working table. Use the control rows to see what evidence you would hand an examiner. Track status as not started, drafted, in force, or evidenced. Share the gap list with counsel before an examination, not the week of.

| Framework | What it is | What people claim it means for this tool | What to verify |
|---|---|---|---|
| NIST AI RMF 2.0 | Voluntary. NIST.AI.100-1 is the document practitioners cite. | Govern, map, measure, manage, at a high impact if money moves | You actually run the four functions, or you do not claim them |
| EU AI Act (Regulation 2024/1689) | Binding where it applies | Annex III creditworthiness uses can be high-risk, with documentation, oversight, logging, transparency | Territorial scope and whether your users and subjects put you in it |
| ISO/IEC 42001:2023 | A management-system standard | A risk assessment, a policy, competence, audit, management review | Certification only if you pursued it |
| ECOA, 15 U.S.C. § 1691; Regulation B | Federal credit law | No discrimination; specific adverse-action reasons when required | Product scope. Commercial exemptions are counsel's reading, not a vibe. |
| Fair Housing Act, 42 U.S.C. § 3601 and following | Federal housing law | No disparate treatment or unjustified disparate impact in covered transactions | Whether the collateral or the decision is a housing transaction |
| GLBA, 15 U.S.C. § 6801; Safeguards Rule | Federal financial-privacy law | A security program for customer financial information | Whether you are a financial institution under the rule |

## If counsel says the EU column is in play

Treat the following as the checklist to confirm, not as chores you already owe. Article numbers are the ones practitioners attach to these duties. Have counsel confirm they still point at the right obligation.

- A risk-management system across the life of the model (Art. 9).
- Data governance for training and testing (Art. 10).
- Technical documentation before you rely on it (Art. 11).
- Automatic logs (Art. 12).
- Instructions and transparency for the people using it (Art. 13).
- Human oversight, including the ability to override and to stop (Art. 14). This suite's oversight protocol is the operating version.
- Accuracy and robustness you can show (Art. 15).
- A quality system around the model (Art. 17).
- Conformity assessment (Art. 43) and registration (Art. 49), if those duties reach you.
- Post-market monitoring (Art. 72) and serious-incident reporting (Art. 73).

NIST, if you adopt it, wants the same life cycle in four words: govern (policy, roles), map (context and impacts), measure (bias, performance, logs), manage (response, incidents). ISO/IEC 42001, if you adopt it, wants a policy (clause 5), a risk process (clause 6), competence and documented information (clause 7), operational controls including impact assessment (clause 8), monitoring, audit, and management review (clause 9), and corrective action (clause 10).

One obligation, several citations:

| Control | EU AI Act, if applicable | NIST, if adopted | ISO, if adopted | U.S. law, if applicable |
|---|---|---|---|---|
| Risk system | Art. 9 | GOVERN, MAP | 6.1, 6.2 | ECOA, as a way to show the practice is considered |
| Data governance | Art. 10 | MEASURE | 8.2 | GLBA safeguards, for data you hold |
| Technical file | Art. 11 | MAP | 7.5 | The memo you would need to explain an adverse action |
| Logging | Art. 12 | MEASURE | 9.1 | Whatever record the product's rule already requires |
| Transparency to the user of the tool | Art. 13 | MEASURE | 8.3 | Regulation B's reason requirement, when it applies |
| Human oversight | Art. 14 | GOVERN | 8.3 | A person accountable for the credit decision |
| Accuracy | Art. 15 | MEASURE | 8.4 | A validation you can describe |
| Quality system | Art. 17 | GOVERN | 5, 10 | Often "not a statute" — do not invent one |

A log-retention figure you will see in templates is ten years for certain high-risk systems under the EU regime. Confirm it before you adopt it. The five-year and seven-year clocks in the acceptable-use reference are separate planning defaults for deal files. They are not a substitute for the statutory clock.

## Twelve rows, one owner each

| # | Area | What "done" looks like | Where the procedure lives |
|---|---|---|---|
| 1 | Human oversight | A person can understand, override, and stop the tool. Sign-off is required before a recommendation is final. | Human-oversight protocol |
| 2 | Bias and fairness | A test plan, ratios, and a fail path. Not a vendor slide. | Bias-testing reference |
| 3 | Model documentation | Purpose, data, limits, version, known failures. | Model card plus the use register |
| 4 | Privacy and security | Classification, minimum data, encryption, vendor exhibit, no training on customer files without a basis | Acceptable-use policy; vendor review |
| 5 | Explainability | A reason a person can say, plus a range when the model is unsure | Decision record |
| 6 | Risk system | Inherent and residual scores, owners, a review cadence | Risk register |
| 7 | Logging and monitoring | Inputs, version, output, override, retained on your schedule | Audit-trail article; oversight protocol |
| 8 | Incidents | Same-day notice inside the company, a halt, a cause, counsel on external notice | Acceptable-use policy; risk register |
| 9 | Competence | The signers have been shown the limits, and you kept attendance | Oversight protocol |
| 10 | Vendors | A scorecard before signature, and a rescore on change | Vendor due diligence |
| 11 | Validation | Against outcomes, on a calendar, by someone who did not only build it | Risk register, RISK-002 |
| 12 | Data governance | Lineage of training data, a screen for proxies, quality checks before a run | Bias-testing reference |

If a row's procedure does not exist yet, the crosswalk cell says "gap." Do not write "aligned."

## What a reviewer tends to ask

These are patterns from examinations and from vendor reviews, not a prediction about yours.

- A policy that names NIST and no evidence of a test, a log, or an override.
- Adverse-action reasons that quote a score and do not state a reason.
- Training data nobody can date.
- A human-oversight sentence and files that all match the model.
- Vendor diligence that is a security questionnaire with the AI rows blank.
- A classification memo that says "high-risk" with no counsel review, or "not applicable" with no analysis.

Bring the grid, the procedures, and a sample of files. Do not bring a slide that says compliant.

## A sequence that fits an owner-led desk

Skip the theater of a six-month program if you do not yet have the first four artifacts. The order below is a planning sequence. Weeks and months are illustrative, not a regulatory deadline.

**First, the short list.** Name the credit owner, the compliance owner, and the model owner. Inventory every tool that touches a file, including the unapproved chat window. Mark counsel's applicability column as open until they answer.

**Next, the foundation.** Stand up the use register, the one-page policy, and the underwriting acceptable-use annex. Add the decision-record fields. Stop pasting files into unapproved tools. That is the highest-leverage week you will spend.

**Then the structure.** Finish the risk register's five deep rows. Run the first bias screen, even if some cells are too small and you have to say so. Score any vendor already in production.

**Then the hardening.** Close red flags, write the halt, put validation on a calendar, and sample files for the independent note. Only then consider whether ISO certification or an EU conformity path is even relevant.

**Then the cadence.** Quarterly ratios and residual scores. A semiannual register rewrite. An annual reread of the protocol. A rescore when the model changes. This is "When the Model Changes Under You," on a grid.

## A status line you can keep

| Row | Applicability (counsel) | Status | Evidence | Gap |
|---|---|---|---|---|
| Oversight | | | Protocol version, five-file sample | |
| Bias test | | | Last test memo | |
| Model card | | | Current card | |
| Security | | | Vendor exhibit or internal control | |
| Reasons | | | Two adverse files, if the product has them | |
| Risk register | | | Dated scores | |
| Logs | | | One sample log | |
| Incidents | | | The halt names | |
| Competence | | | Attendance | |
| Vendor score | | | Scorecard | |
| Validation | | | Last report and its date | |
| Data lineage | | | Training-set note | |

Empty applicability cells are an open legal question. Empty evidence cells are an operating gap. Do not mix them up in the board pack.

## Questions owners ask

**Is our tool high-risk?** Maybe, under one regime and not another. The honest status is "counsel has classified it" or "counsel has not." Operating as if oversight, logging, and a bias test matter is appropriate either way. Announcing a classification is not.

**What do we do first?** The names, the inventory, the decision record, and a ban on unapproved tools. The crosswalk without those is a poster.

**How often is the bias test?** Before reliance, quarterly for the ratios, and on a material change. The bias reference has the procedure. This grid only refuses to mark the row done without it.

**Do we need an outside validator?** You need someone who did not solely build the model to read the validation. Outside is how small teams get that independence. It is a control choice, not a statute this article can impose.

**Where does counsel fit?** Applicability, notices, indemnity, adverse-action forms, and anything you say to an agency. Counsel does not fill in the operating evidence. You do.

## The practical next step

1. Copy the twelve-row table. Write "gap" wherever the procedure in the last column does not exist as a file someone can open.
2. Send counsel the applicability column and nothing else until they mark it. Do not guess "mandatory" to look serious.
3. Close the three gaps that show up in every thin program: an unapproved chat tool, a missing decision record, and a vendor with no scorecard.
4. Put the status table in the same folder as the risk register. Update it when a row changes, not when a quarter ends and someone remembers.
5. Reread the citations once a year. A crosswalk that quotes dead article numbers is worse than a short one that is current.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*

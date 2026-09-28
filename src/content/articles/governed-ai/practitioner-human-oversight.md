---
title: "A Human Oversight Protocol for AI-Assisted Underwriting"
series: "The Governed AI Series"
part: "Part I — Draw the Boundary"
eyebrow: "DRAW THE BOUNDARY"
deck: "The operating sequence for an underwriting file when a model has a view: independent judgment first, the model's output second, and a written override when the two disagree."
author: "Cypress Command"
date: "2026-09-28"
read_time: "10 min"
desk: "buy"
status: "review"
source: "practitioner-reference"
---

# A Human Oversight Protocol for AI-Assisted Underwriting

"Prepare, Recommend, Decide: Three Levels of AI Involvement and Who Signs Each" names three levels and stops AI at recommend. This practitioner reference is the procedure for an underwriting file that sits at that line: who acts at each step, what an override has to contain, when the file escalates, and what a later reader must be able to reconstruct. The one-page policy states the rule. This is how a credit desk performs it on a Tuesday.

Article 14 of the EU AI Act is the provision people cite when they want human oversight designed into a high-risk system: understand the tool, watch it, override it, and be able to stop it. Whether your tool is high-risk, and whether the Act applies to your entity, is counsel's classification. The procedure below is written so you can meet that shape if the answer is yes. ECOA's adverse-action rules, where they apply, are the reason a denial needs a specific reason from a person, not a feature list. The Fair Housing Act is the reason an override pattern is itself something you monitor. NIST's GOVERN function is a useful checklist for "someone is actually accountable." None of those sentences is a determination that they bind you. Ask, then keep the procedure.

## Where it applies

Any underwriting work in which a model is consulted, produces an output, or is sitting in the file a person will rely on:

- Acquisition financing, bridge loans, and equity views on retail property.
- Refinances, cash-out, and restructuring.
- Rent-roll, lease-abstract, tenant-credit, and vacancy review when a model summarized them.
- Guarantor and entity financial review.
- Comparable sales, cap rates, and market notes a model assembled.
- Any score, flag, or rating on a deal, a property, or a sponsor.

People bound by it: anyone who submits data, reads an output, or signs a recommendation. Vendors with access to the tool are on the list. A committee is optional. A named credit owner is not.

Review the procedure every year, and sooner if the regulation changes, the model changes, a material finding lands, or the override rate leaves the band you set. An illustrative band that should force a reread is an override rate above 20 percent in a quarter, or below the floor in the risk register, near 2 percent. Both extremes mean the relationship between the person and the model has changed.

## What each role owes

Collapse titles if you must. Do not collapse the accountable name.

| Work | Responsible | Accountable | Consulted | Informed |
|---|---|---|---|---|
| Complete, lawful inputs | Preparer | Credit owner | Compliance, if personal data is in the file | The reviewer |
| Independent view, before the model is shown | Underwriter | Credit owner | — | Compliance, on a sample |
| Read the model and reconcile | Underwriter | Credit owner | Model owner, if the output looks wrong | — |
| Final recommendation | Underwriter, or credit owner when the scenario says so | Credit owner | Counsel on fair-lending overrides | The file |
| Adverse-action notice, if one is required | Underwriter | Compliance owner | Counsel | The applicant, in the form counsel specifies |
| Sample and bias watch | Compliance owner | Credit owner | The person who runs the bias test | Owner, quarterly |
| Annual rewrite of this protocol | Credit owner | Owner | Counsel | The desk |

A workable committee, if you are large enough to have one, is the credit owner, the compliance owner, a senior underwriter, someone who can see the system, and counsel. Quarterly meeting. The owner gets the annual page. A two-person shop writes the same grid with two names repeated. That is allowed. A grid with no names is not.

Competency is a short list, not a certificate program. The person who signs can explain what the model is for, what it does not see, how to override it, and which data never goes in. New users do not sign files until they have done that on a sample file with the credit owner watching. Refresh on the same annual cycle as the protocol. Keep the attendance, not a transcript.

## Nine stages, in order

No stage is skipped. The point of the order is to stop anchoring: the person writes a view before seeing the model's view.

**1. Submission.** The preparer assembles the rent roll, trailing statements, entity and guarantor financials as the acceptable-use policy allows, valuation material, market inputs, the requested terms, and the lease abstracts. A completeness check runs first. Gaps go on a list, not into a silent upload.

**2. Model run.** The system may produce a recommendation (approve, deny, conditional, or insufficient data), a confidence indication, the factors it used, the comps it leaned on, and data-quality flags. The output stays hidden from the underwriter until stage 3 is written down. If your tool cannot hide it, the underwriter completes the independent note in a separate document before opening the output. Honor systems fail. Prefer the software constraint.

**3. Independent view.** Traditional underwriting, without the model. A preliminary approve, deny, or conditional, with the reason, dated.

**4. Comparison.** Now open the output. Note where it matches, where it does not, and any factor you do not understand. An output you cannot explain is not "probably fine."

**5. Reconciliation.** If the views differ, or the model flags a risk you did not, write the difference and the reason you are keeping your view or changing it. This is the record "The Audit Trail" is about.

**6. Decision.** The underwriter recommends. Scenarios in the next section say when the credit owner also signs. The decision record holds the independent view, the model output, the reconciliation, and the final recommendation.

**7. Adverse action, when the product requires it.** A specific reason, in plain language, tied to the person's decision. An illustrative planning clock used in consumer credit is 30 days; commercial products differ. Counsel tells you whether a notice is required and on what clock. The compliance owner reads notices that came out of an override.

**8. Sample.** The compliance owner reads a sample of decisions and the bias metrics. An illustrative sample is 20 percent of AI-assisted files in a period, or all of them if the book is small. Findings go to the credit owner. Patterns go into the bias-testing procedure, not into a forgotten email.

**9. Rewrite.** Once a year, or on the triggers above. Version the protocol. Say what changed.

## Overrides

An override is allowed. An undocumented override is a missing file. Overrides are not a way around fair lending. The desk must be technically able to disregard the model. A tool that will not proceed without accepting its recommendation is not fit for this protocol.

**A. Model says deny, person says approve or conditional.** Write the factors the model missed or overweighted, and the way you are covering the risks it did flag. The credit owner co-signs. Compliance is told, and may pull the file for a fair-lending read.

**B. Model says approve, person says deny or conditional.** Write the risk the model missed. The credit owner is informed. A co-signature is not required for the denial itself. Compliance reads it if the reason could track a protected characteristic.

**C. The override could itself be a fair-lending problem.** Any pattern, or any single file, where the person's reason would treat a protected group differently if repeated. Credit owner and compliance owner both sign. The file includes a short impact note: who else would this reason touch? Counsel is consulted before the reason becomes a habit.

**D. The output is nonsense, or the system failed.** Do not "work around it" with a partial screenshot. Mark the output unusable, underwrite without it, and tell the model owner the same day. If the failure is repeated, halt.

**E. A fact arrives after the model ran.** Rerun if the tool allows a clean rerun. If you proceed on the old output plus the new fact, the record says both, and the person owns the combination.

**F. A policy exception.** The credit owner approves the exception in writing, with an expiry. Exceptions do not become the new policy by repetition. Three of the same exception in a quarter is a protocol rewrite, not a stack of waivers.

## What the forms hold

You do not need six templates. You need four contents.

**Decision record.** Deal, date, tool name and version, independent recommendation and reason, model recommendation and confidence, differences, final recommendation, signer, whether an override scenario applies.

**Override note.** Scenario letter, facts the model did not have, why the final view is better, co-signer when the scenario requires one, fair-lending flag yes or no.

**Gap list.** What was missing at submission, whether you proceeded, and what you used instead.

**Adverse-action content, if required.** The specific reasons, the date sent, who reviewed it. Do not invent a consumer form for a commercial loan counsel says does not need one. Do not skip a form counsel says you do need.

The audit trail keeps those four, plus the inputs the model saw and the output it returned, in the deal file. "The Audit Trail" describes the shape. This protocol says they are not optional on an assisted file.

## Quality, escalation, halt

Sample for two things: did the independent note exist before the output was opened, and do overrides cluster on a group, a product, or a person? Clustering is a bias-testing trigger, not a coaching tip you save for year-end.

Escalate the same day when the acceptable-use triggers fire (score gap, income gap, stale validation), when scenario C is even arguable, when the system fails, or when a borrower complaint names the model.

Halt authority sits with the credit owner and the compliance owner, either one. Halt means outputs stop informing recommendations. In-flight files revert to the independent view alone, and the record says the model was off. Restart only after the cause is written and, if the cause was bias or a bad training set, after the retest in the bias procedure.

## What you watch

| Indicator | Why it is there | Illustrative reading |
|---|---|---|
| Override rate | A desk that never disagrees may have stopped looking | Under about 2 percent, investigate; a 5–15 percent band is a teaching sign of life, not a target |
| Share of files with an independent note dated before the output | The protocol's main control | Anything under "all of them" is a miss |
| Variance flags open past the SLA you set | Accuracy row of the risk register | Aging flags are unread flags |
| Sample pass rate | Whether the notes are real | Thin notes count as fails |
| Time from denial to notice, if notices apply | A clock counsel gave you | Late is an incident |
| Validation age | Stale models escalate | Older than twelve months, stop relying |

Report monthly to the credit owner, quarterly to the owner of the business. Drift and retraining sit with the model owner and with "When the Model Changes Under You." This protocol only insists that a drifted model is not quietly still in stage 4.

## Questions the desk asks

**Is the model making the decision?** No. If your files read as if it is, the protocol is not in force, whatever the policy says.

**It broke mid-file.** Scenario D. Manual from there. Tell the model owner. Do not paste the half-finished output into the memo.

**How do we keep bias out?** You do not, by hoping. You run the bias-testing reference, you sample overrides, and you treat a cluster as a reason to stop.

**May I override?** Yes, in writing, on the scenario that fits. Some overrides need a second signature. None of them need a workaround in the software.

**How often does this get reread?** Annually, and when the model, the law, or the override rate moves.

## The practical next step

1. Write the nine stages on one page and mark the step your current tool cannot enforce. That mark is a system change or a separate note — pick one this month.
2. Add the decision-record fields to the file template. Refuse to close a recommendation that leaves them blank.
3. Name the halt: two people who can turn outputs off without a meeting.
4. Pull five recent assisted files. If the independent view is missing or is dated after the model output, the protocol is still a draft.
5. Put the annual reread on the calendar next to the bias test, not in a separate month you will skip.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*

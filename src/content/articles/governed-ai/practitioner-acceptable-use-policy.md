---
title: "An Acceptable Use Policy for AI in CRE Underwriting"
series: "The Governed AI Series"
part: "Part I — Draw the Boundary"
eyebrow: "DRAW THE BOUNDARY"
deck: "A practitioner policy for underwriting desks: which AI uses are allowed, which are refused, who may touch each tool, and what the memo has to record."
author: "Cypress Command"
date: "2026-09-28"
read_time: "15 min"
desk: "buy"
status: "review"
source: "practitioner-reference"
---

# An Acceptable Use Policy for AI in CRE Underwriting

The Governed AI Series closes with "A One-Page AI Policy an Owner-Led Business Can Actually Follow," eight clauses that fit on a page for any owner-led business. "AI in CRE Underwriting: What the Model Prepares and What the Owner Signs" draws the boundary on a single file. This practitioner reference is the underwriting-specific policy those pieces point at. It names permitted uses, prohibited uses, who may touch which tool, what data may enter, and what the credit memo has to say. It does not replace the one-page policy. It is the annex for credit work.

The clauses below are an operating form an owner or a credit desk can adapt. They are not a statute, and they are not a claim that any particular tool is already classified as high-risk. An underwriting model that influences credit, pricing, or occupancy can fall into categories regulators treat seriously, including creditworthiness uses listed in Annex III of the EU AI Act and the fair-lending statutes that apply when a decision touches credit or housing. Whether a given tool, and a given operator, is in scope is counsel's question. Write the controls as if the answer might be yes. Do not publish a legal classification you have not had reviewed.

A small shop collapses several rows onto one named person. A larger desk keeps them separate. The policy still needs the names.

## What the policy is for

Five jobs, written so a new analyst can repeat them:

- **Name the laws you are trying to meet.** EU AI Act, NIST AI Risk Management Framework, ECOA, the Fair Housing Act, and GLBA are the usual list for this work. Confirm which ones actually apply before you cite them in a borrower letter.
- **Limit model risk.** Bad inputs, stale models, and a score nobody checked are credit errors with a tidy font.
- **Keep the use fair.** A neutral-looking factor can still land harder on a protected group. The bias-testing reference in this suite is the procedure. This policy is the rule that the procedure exists.
- **Keep fair lending in the same file as the model.** If the output can affect a credit decision, the fair-lending review is not a separate binder.
- **Name the human.** Every AI-assisted recommendation has a person who signs it.

## Permitted uses, and only those

Only tools on a written register may touch a live file. "The AI Use Register: Writing Down Where AI Touches the Business" is that list for the whole company. For underwriting, the register should be specific enough to match this table. Anything not on it stays off until someone reviews it and adds the row.

| Category | What the tool may do | What it may not do |
|---|---|---|
| Financial spreading | Extract a rent roll, a trailing-twelve operating statement, and entity financials into a spread | Treat the spread as checked |
| NOI and coverage | Lay out net operating income, a debt-service coverage range, and a vacancy sensitivity from figures a person supplied or verified | Invent the rent-growth or vacancy assumption |
| Risk scoring | Score a file from property type, tenancy, market, and sponsor characteristics the desk defined | Decline, approve, or price the loan |
| Market research | Assemble comparables, cap-rate context, and vacancy or absorption notes from approved sources | Become the only source for a cap rate that goes in the memo |
| Lease abstraction | Pull term, rent, options, co-tenancy, and recoveries | State the legal meaning of a clause |
| Valuation support | Select comparables and cross-check an automated value | Replace the appraisal |
| Portfolio surveillance | Flag coverage, covenants, occupancy, and a watch list | Change a risk rating without a person |
| Memo drafting | Draft sections inside an approved tool | Ship the draft as the memo |

Access follows the role, not the login someone borrowed.

| Role | Spreading | Scoring | Market | Valuation | Portfolio | Drafting |
|---|---|---|---|---|---|---|
| Junior analyst | Permitted | Read only | Permitted | No | No | Draft only |
| Senior analyst | Permitted | Permitted | Permitted | With review | Read only | Draft only |
| Underwriter | Full | Full | Full | Full | With review | Full |
| Senior underwriter | Full | Full | Full | Full | Full | Full |
| Portfolio manager | Limited | Full | Full | With review | Full | Limited |
| Compliance | Audit | Audit | Audit | Audit | Audit | Audit |

"With review" means a named supervisor sees the output before it enters a decision. Put the rule in the access system, not in a slide.

The sequence is fixed: data in, model output, human review, human decision, file. Skipping review needs a written exception from the senior underwriter, and the exception goes in the file. Volume is not an exception.

## What may go in

- Trailing operating statements, with any individual Social Security numbers masked.
- Rent rolls: tenant, suite, term, base rent, recoveries, use. No residential-tenant personal data.
- Leases and abstracts, with guarantor identifiers removed.
- Appraisals and environmental reports.
- Market data from vendors whose license allows that use.
- Public records, zoning, and title commitments.
- Entity financials, with tax identifiers masked.
- De-identified historical performance from your own book.
- Foot-traffic or demographic files from an approved vendor, used as market context, not as a proxy for who the borrower is. The bias-testing reference covers why that distinction matters.

Personal financial statements and personal tax returns are conditional. Mask identifiers, dates of birth, and account numbers first. Enter aggregates or summary schedules, not the raw return. A second person confirms the redaction before the file goes in. Credit-bureau reports stay out of the model. Borrower Social Security numbers stay out. Immigration or citizenship data stays out. If the underwriting question needs those facts, a person reads them, and the model does not.

An illustrative use, not a live file: a 220,000-square-foot community center, a trailing-twelve, a rent roll, and the recovery reconciliations go into the approved spreading tool. The tool returns net operating income of $2.1 million, coverage of 1.38 times, and two tenants expiring inside eighteen months. That is a permitted draft. The underwriter still ties every figure to the source, reads the expiring leases, and writes the judgment. The memo does not go out on the model's numbers alone.

## What is refused

| Refused | Why it is refused |
|---|---|
| A final approve, decline, or pricing change with no person in the path | The model does not hold the decide level. Adverse-action reasons, if they are required, have to come from a person who can explain them. |
| A confidential file pasted into a personal or unapproved chat tool | The data leaves your controls. If the file holds customer financial information, the Safeguards Rule discussion starts here. Counsel decides whether a notice is due. |
| A use outside the row you approved | A spreading tool is not a screen for someone's personal investments. |
| Switching off a bias filter, a mask, or the log | The audit trail is the point of the control. |
| Training a model on customer files without a written protocol, de-identification, and legal review | The data was collected for a deal, not for a training set. |
| Shared logins or shared API keys | You cannot name the person if the credential is a group. |
| A recommendation accepted with no check once the file is above the desk's credit authority | Authority is a person, not a score. |
| Model prose copied into the memo with no edit and no certification | The underwriter signs the words. |

An illustrative miss: an analyst pastes an unredacted operating statement, a personal financial statement, and tax returns into a public chat tool to speed a memo. That is a refused use. Treat it as an incident, not as a shortcut that worked.

A second miss: a junior analyst treats a "decline" score as the decision and sends the letter. The score is an input. The letter is a person's act. A model that never read the anchor lease will still sound sure.

## The person decides

No model on this desk has authority to approve, decline, or change terms. A risk score, a cash-flow draft, and a decline flag are inputs. Time pressure does not waive the rule, and a manager's request to "just send it" does not either.

Before the memo moves:

- Trace every extracted figure to the source document.
- Check market figures against a second source.
- Write the qualitative facts the model did not have: sponsor history, property condition, anchor strength.
- Confirm you are not relying on a protected characteristic, or on a stand-in for one.
- Name the underwriter who reviewed the output and who makes the recommendation.

Override authority is narrower than access.

| Role | Override a score | Override a decline flag | Decide with the model unavailable | What gets written |
|---|---|---|---|---|
| Junior analyst | No | No | No | — |
| Senior analyst | Only with approval | No | No | A note to the underwriter |
| Underwriter | Yes | With a memo | Only in an outage | Override memo; compliance notified on declines |
| Senior underwriter | Yes | Yes | Yes | Override memo; risk committee notified above the desk's large-file line |
| Portfolio manager | Yes | Yes | Yes, for surveillance | The override in the system of record |

An illustrative large-file line used in some credit shops is $10 million. Set your own number. Do not borrow one because it appeared in a template.

Escalate to the senior underwriter when:

- The model's score and the underwriter's score differ by more than an illustrative 15 points on your scale.
- Extracted net operating income and the underwriter's net operating income differ by more than an illustrative 5 percent.
- The model says decline and a material fact was never in the file.
- The model says approve and a material risk was never flagged.
- The borrower has raised a fair-lending complaint before.
- The model has not been validated in the past twelve months.
- The inputs are stale or inconsistent.

The review path is short. Read the recommendation. Compare it with the independent view. If they agree, accept and document. If they do not, change the output and write the reason. If the gap is one of the triggers above, escalate, then document. Every path writes the file down. There is no silent path.

The memo's AI section names the tool and version, the outputs relied on, the outputs changed and the substitute figures, the facts the model did not capture, and a sentence in the underwriter's words: the analysis was reviewed, the figures were validated, and the recommendation is the underwriter's.

## Data handling

| Data | In the model? | Condition |
|---|---|---|
| Trailing operating statements | Yes | Mask individual identifiers |
| Rent roll | Yes | No residential personal data |
| Entity financials | Yes | Mask tax identifiers and owner identifiers |
| Personal financial statements | Conditional | Aggregates only, after redaction; compliance owner approves the input |
| Personal tax returns | Conditional | Summary schedules only; two-person redaction check |
| Credit-bureau reports | No | A person reads them |
| Bank statements | Conditional | Account and routing numbers out; personal payees out |
| Appraisals | Yes | Strip personal contact details if you do not need them |
| Market opinions | Yes | Only if the license allows it |
| Leases | Yes | Guarantor identifiers out |
| Social Security numbers | Never | Not in the prompt, not in the upload |
| Immigration or citizenship | Never | Do not collect it for the model |

Take the minimum. If the question is one schedule, do not upload the whole package. Do not leave owner financials sitting in a vendor's store. Confirm the tool can run the analysis without keeping a copy, and delete the cache on the timetable you set. An illustrative timetable used in these drafts: source uploads cleared within 30 days of close, decline, or withdrawal; the analysis kept in the deal file for seven years or the regulatory minimum counsel names, whichever is longer; system logs kept at least five years. Those clocks are planning defaults. Counsel and your retention schedule control the real ones.

If customer financial information is in scope, the Gramm-Leach-Bliley Act Safeguards Rule is the conversation with counsel: who may see it, encryption in transit and at rest, vendors bound to an equivalent standard, and what a breach notice requires. Do not paste a "30 days to the FTC" sentence into a policy until counsel confirms it is the clock that applies to you.

## Bias, in the policy rather than the lab

The testing procedure lives in "Bias Testing for AI-Assisted CRE Underwriting." The policy only has to forbid the outcome and name the mechanism.

Proxy discrimination is a neutral variable that tracks a protected characteristic. A postal code can do that. Disparate impact is a neutral rule, such as a coverage floor, that lands harder on a protected group even when nobody typed the characteristic into the model. Intent is not the test you should rely on. The file should show you looked.

Characteristics that fair-lending and fair-housing law commonly protect, and that this policy refuses as decision factors, include race, color, national origin, religion, sex, familial status, disability, age, marital status, and income from public assistance. The statutes are not identical, and a shopping-center loan is not a residential rental. Counsel maps which list applies to which product. The operating rule is stricter than the argument: do not use them, and do not use a stand-in.

Mitigation in practice: training data that matches the book you actually lend on, a test before deployment and on a schedule, a person on every adverse outcome, an audit that is not performed by the model vendor alone, and adverse-action reasons a person can say in plain language.

## Transparency, quality, and security

Keep a model card the desk can read: purpose, data, limits, and known failures. Outputs should trace to inputs. Adverse recommendations need a human-readable reason, not a feature-importance chart alone. Tell a borrower that a tool assisted, if counsel says the notice is required. Do not hand over the model.

Check data before it goes in. Validate the model against outcomes, not against its own last memo. Watch for drift. Write the correction path: who finds an error, who fixes the file, who tells the people already affected.

Access is by role. Encrypt in transit and at rest. Test the vendor. Keep an incident plan that includes a halt. The vendor's security exhibit is part of your security, which is why the due-diligence reference in this suite asks for evidence rather than a paragraph on a website.

## Training, monitoring, incidents

Anyone who uses a tool completes the policy, the fair-lending points that apply to the product, and the data rules, on a cycle you set. Annual is a common cycle. Role-specific modules beat one slide for the whole floor. If a model has not been validated in twelve months, files that use it escalate.

Monitor use, inputs, and odd outputs. Sample the memos. Keep a log that cannot be quietly edited: tool, version, output, change, person. Bias monitoring is a standing report, not a project.

Report a suspected malfunction, a bias concern, a data incident, or a policy breach to the named compliance owner the same day. Investigate, write the cause, and correct the control. Regulatory notice, if any, is counsel's call, made on a clock you have already asked them to write down. Afterward, change the policy only where the incident showed a hole. Do not add a paragraph for its own sake.

## A short list for the desk

Do use the approved tools for the eight categories above. Do review every assisted recommendation. Do redact identifiers first. Do check market figures against a second source. Do write the tool, the output, and the override into the memo. Do take the training. Do report a bad output the day you see it.

Do not paste a live file into an unapproved chat tool. Do not let the model send the decision. Do not turn the filters or the log off. Do not train on customer files without a protocol and a legal review. Do not share credentials. Do not skip the check because the file is large or because it is small. Do not put a bureau report, a Social Security number, or citizenship data into the model.

## Questions the desk actually asks

**Why a policy if the tool is supposed to save time?** The time saved is in spreading and drafting. The time you still spend is the review. The policy is how you keep the second half from disappearing on a busy Friday.

**May the model draft the memo?** Yes, inside an approved tool. The underwriter edits it and certifies it. The signature is not the model's.

**The score disagrees with me.** That is the job. If the gap crosses the escalation lines above, the senior underwriter sees it before the file moves. Your view is the decision. The score is the question.

**May personal financials go in?** Only after redaction, only as aggregates or summary schedules, and only with the second check on tax returns. Bureau reports and raw identifiers do not go in.

**How often is the model tested?** On the schedule in the bias-testing reference, and at least before you rely on a model that has gone twelve months without a validation. A missed validation is an escalation, not a footnote.

**I think something broke.** Tell the compliance owner the same day. Keep the file. Do not "fix it quietly" by regenerating the memo.

## The practical next step

1. Copy the permitted-use table and delete every row you do not actually run. Add the rows you do run that are missing, including the chat tool an analyst already uses.
2. Name a person for each role. If one person holds three roles, write that down.
3. Pick the two escalation numbers you will actually enforce — score gap and income gap — and put them on the memo template.
4. Add the AI section to the credit-memo form this week: tool, version, outputs used, outputs changed, certification line.
5. Tell the desk, in one meeting, which pastes are refused. Then check one live file against the policy before the month ends.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*

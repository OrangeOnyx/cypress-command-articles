---
title: "An Acceptable Use Policy for AI in CRE Underwriting"
series: "The Governed AI Series"
part: "Part I — Draw the Boundary"
eyebrow: "DRAW THE BOUNDARY"
deck: "The underwriting annex to the one-page policy: which AI uses an owner may run on a deal file, which are refused, and what the memo has to record."
author: "Cypress Command"
date: "2026-09-28"
read_time: "8 min"
desk: "buy"
status: "published"
source: "practitioner-reference"
---

# An Acceptable Use Policy for AI in CRE Underwriting

This annex sits under "A One-Page AI Policy an Owner-Led Business Can Actually Follow" and adds only the underwriting-specific rows. The reader is the owner of a small commercial real estate or shopping-center business. You use AI to underwrite acquisitions, refinances, and lender packages for your own properties, and to read leases and tenant financials. The one-page policy already states purpose, the register, the three levels, data scope, review, records, vendor features, and cadence. Do not copy those clauses onto this page. Name the people, then keep the rows below.

The clauses are an operating form an owner can adapt. They are not a statute, and they are not a claim that any particular tool is already classified as high-risk. Annex III, point 5(b), of the EU AI Act covers AI systems intended to be used to evaluate the creditworthiness of natural persons or establish their credit score, with an exception for financial-fraud detection. It does not cover rating a legal entity. Fair-lending and fair-housing statutes follow decisions about credit and housing; whether any of your uses (for example a residential component, or deferred rent to a tenant) touches them is counsel's question. Whether a given tool, and a given business, is in scope is also counsel's question. Write the controls as if the answer might be yes. Do not publish a legal classification you have not had reviewed.

## What this annex adds

Four jobs, written so a preparer can repeat them:

- **Name the laws you are trying to meet.** EU AI Act, NIST AI Risk Management Framework, ECOA, the Fair Housing Act, and GLBA are the usual list for this work. Annex III, point 5(b), covers AI systems intended to be used to evaluate the creditworthiness of natural persons or establish their credit score, with an exception for financial-fraud detection. It does not cover rating a legal entity. Confirm which laws actually apply before you cite them in a letter about the deal. Fair-lending and fair-housing statutes follow decisions about credit and housing; whether any of your uses touches them is counsel's question.
- **Limit model risk.** Bad inputs, a stale model, and a score nobody checked are decision errors with a tidy font.
- **Keep the use fair.** A neutral-looking factor can still land harder on a protected group. Run a bias check before you rely on the tool. This annex is the rule that the check exists.
- **Name the human.** Every AI-assisted recommendation has a person who signs it.

## Three roles

Counsel and the CPA are consulted. They are not a fourth role on the grid.

| Role | Who holds it | What they do |
|---|---|---|
| Owner | The principal | Decides, signs, and approves exceptions |
| Preparer | The staff analyst, asset manager, or outside bookkeeper | Runs the tool and checks citations |
| Second reader | A partner, the CPA, or the owner on a one-person shop | Reviews deals above a size the owner sets |

Set a deal size above which a second reader is required. Write the number down. A one-person shop writes the owner's name on the second-reader row for those deals. A grid with no names is not a policy.

The sequence is fixed: data in, model output, human review, human decision, file. Skipping review needs a written exception from the owner, and the exception goes in the file. Volume is not an exception.

## Permitted uses, and only those

Only tools on a written register may touch a live file. "The AI Use Register: Writing Down Where AI Touches the Business" is that list for the whole company. Anything not on it stays off until the owner adds the row.

| Category | What the tool may do | What it may not do |
|---|---|---|
| Financial spreading | Extract a rent roll, a trailing-twelve operating statement, and entity financials into a spread | Treat the spread as checked |
| NOI and coverage | Lay out net operating income, a debt-service coverage range, and a vacancy sensitivity from figures a person supplied or verified | Invent the rent-growth or vacancy assumption |
| Rank deals or tenants | Rank a file from property type, tenancy, market, and guarantor or partner characteristics the owner defined | Decide to buy, refinance, lease, or reject a tenant |
| Market research | Assemble comparables, cap-rate context, and vacancy or absorption notes from approved sources | Become the only source for a cap rate that goes in the memo |
| Lease abstraction | Pull term, rent, options, co-tenancy, and recoveries | State the legal meaning of a clause |
| Valuation support | Select comparables and cross-check an automated value | Replace the appraisal |
| Portfolio watch | Flag coverage, covenants, occupancy, and a watch list | Change a risk view without a person |
| Memo drafting | Draft sections of an investment or financing memo (acquisition, refinance, lender package) inside an approved tool | Ship the draft as the memo |

## What may go in

The table below is the list. Personal financial statements and personal tax returns, when they are the owner's or a guarantor's, are conditional. Mask identifiers, dates of birth, and account numbers first. Enter aggregates or summary schedules, not the raw return. A second person confirms the redaction before the file goes in. On a one-person shop, the CPA is that second person. Tenant and guarantor credit reports stay out of the model; a person reads them. Social Security numbers stay out. Immigration or citizenship data stays out. If the question needs those facts, a person reads them, and the model does not. Foot-traffic or demographic files from an approved vendor are market context, not a proxy for who a person is. A bias check is why that distinction matters.

An illustrative use, not a live file: a 220,000-square-foot community center, a trailing-twelve, a rent roll, and the recovery reconciliations go into the approved spreading tool. The tool returns net operating income of $2.1 million, coverage of 1.38 times, and two tenants expiring inside eighteen months. That is a permitted draft. The preparer still ties every figure to the source. The owner reads the expiring leases and writes the judgment. The investment or financing memo (acquisition, refinance, lender package) does not go out on the model's numbers alone.

## What is refused

| Refused | Why it is refused |
|---|---|
| A decision to buy, refinance, lease, or reject a tenant with no person in the path | The model does not hold the decide level. |
| A confidential file pasted into a personal or unapproved chat tool | The data leaves your controls. If the file holds customer financial information, the Safeguards Rule discussion starts here. Counsel decides whether a notice is due. |
| A use outside the row you approved | A spreading tool is not a screen for someone's personal investments. |
| Switching off a bias filter, a mask, or the log | The audit trail is the point of the control. |
| Training a model on customer files without a written protocol, de-identification, and legal review | The data was collected for a deal, not for a training set. |
| Shared logins or shared API keys | You cannot name the person if the credential is a group. |
| A recommendation accepted with no check once the file is above the deal size you wrote down | Authority is a person, not a score. |
| Model prose copied into the memo with no edit and no certification | The owner signs the words. |

An illustrative miss: a preparer pastes an unredacted operating statement, a personal financial statement, and tax returns into a public chat tool to speed a memo. That is a refused use. Treat it as an incident, not as a shortcut that worked.

A second miss: a preparer treats a rank as the decision and sends a letter. The rank is an input. The letter is a person's act. A model that never read the anchor lease will still sound sure.

## The owner decides

No model in this business has authority to buy, refinance, lease, or reject a tenant. A rank, a cash-flow draft, and a stop flag are inputs. Time pressure does not waive the rule.

Before the investment or financing memo moves:

- Trace every extracted figure to the source document.
- Check market figures against a second source.
- Write the qualitative facts the model did not have: guarantor or partner history, property condition, anchor strength.
- Confirm you are not relying on a protected characteristic, or on a stand-in for one.
- Name the person who reviewed the output and the owner who decides.

The second reader sees the file when the deal is above the size you wrote down, and when any of these fire:

- The model's rank and the preparer's rank differ by more than an illustrative 15 points on your scale.
- Extracted net operating income and the preparer's net operating income differ by more than an illustrative 5 percent.
- The model says stop and a material fact was never in the file.
- The model says go and a material risk was never flagged.
- Someone has raised a fair-lending or fair-housing question. Ask counsel before the reason becomes a habit.
- The model has not been checked in the past twelve months.
- The inputs are stale or inconsistent.

The review path is short. Read the recommendation. Compare it with the independent view. If they agree, accept and document. If they do not, change the output and write the reason. Every path writes the file down. There is no silent path.

The memo's AI section names the tool and version, the outputs relied on, the outputs changed and the substitute figures, the facts the model did not capture, and a sentence in the owner's words: the analysis was reviewed, the figures were validated, and the recommendation is the owner's.

## Data handling

| Data | In the model? | Condition |
|---|---|---|
| Trailing operating statements | Yes | Mask individual identifiers |
| Rent roll | Yes | No residential personal data |
| Entity financials | Yes | Mask tax identifiers and owner identifiers |
| Personal financial statements (the owner's or a guarantor's) | Conditional | Aggregates only, after redaction; the owner approves the input |
| Personal tax returns (the owner's or a guarantor's) | Conditional | Summary schedules only; two-person redaction check |
| Tenant and guarantor credit reports | No | A person reads them |
| Bank statements | Conditional | Account and routing numbers out; personal payees out |
| Appraisals | Yes | Strip personal contact details if you do not need them |
| Market opinions | Yes | Only if the license allows it |
| Leases | Yes | Guarantor identifiers out |
| Social Security numbers | Never | Not in the prompt, not in the upload |
| Immigration or citizenship | Never | Do not collect it for the model |

Take the minimum. If the question is one schedule, do not upload the whole package. Do not leave financials sitting in a vendor's store. Confirm the tool can run the analysis without keeping a copy, and delete the cache on the timetable you set. An illustrative timetable: source uploads cleared within 30 days of close, decline, or withdrawal; the analysis kept in the deal file for seven years or the regulatory minimum counsel names, whichever is longer; system logs kept at least five years. Those clocks are planning defaults. Counsel and your retention schedule control the real ones.

If customer financial information is in scope, the Gramm-Leach-Bliley Act Safeguards Rule is the conversation with counsel: who may see it, encryption in transit and at rest, vendors bound to an equivalent standard, and what a breach notice requires. Do not paste a "30 days to the FTC" sentence into a policy until counsel confirms it is the clock that applies to you.

## Bias, in the policy rather than the lab

Run a bias check before you rely on the tool. The policy only has to forbid the outcome and name the mechanism.

Proxy discrimination is a neutral variable that tracks a protected characteristic. A postal code can do that. Disparate impact is a neutral rule, such as a coverage floor, that lands harder on a protected group even when nobody typed the characteristic into the model. Intent is not the test you should rely on. The file should show you looked.

Characteristics that fair-lending and fair-housing conversations commonly name, and that this policy refuses as decision factors, include race, color, national origin, religion, sex, familial status, disability, age, marital status, and income from public assistance. The statutes are not identical. Counsel maps which list applies to which use. The operating rule is stricter than the argument: do not use them, and do not use a stand-in.

## Transparency and security

Outputs should trace to inputs. If a use is a credit decision about a person, counsel tells you what notice is required. Do not hand over the model. Access follows the three roles. Encrypt in transit and at rest. Keep an incident plan that includes a halt. The vendor's security exhibit is part of your security, which is why "AI Vendor Due Diligence Before an Underwriting Tool Is Signed" asks for evidence rather than a paragraph on a website.

## Questions an owner asks

**Why a policy if the tool is supposed to save time?** The time saved is in spreading and drafting. The time you still spend is the review. The one-page policy is the rule. This annex is the underwriting rows.

**May the model draft the memo?** Yes, inside an approved tool. The owner edits it and certifies it. The signature is not the model's. The document is an investment or financing memo (acquisition, refinance, lender package).

**May personal financials go in?** Only when they are the owner's or a guarantor's, only after redaction, and only as aggregates or summary schedules. Tenant and guarantor credit reports, Social Security numbers, and citizenship data do not go in.

**The rank disagrees with me.** That is the job. If the gap crosses the lines above, or the deal is above the size you wrote down, the second reader sees it before the file moves. Your view is the decision. The rank is the question.

## The practical next step

1. Copy the permitted-use table and delete every row you do not actually run. Add the rows you do run that are missing, including the chat tool someone already uses.
2. Write the three names. If you are the owner and the second reader, write that down, and write the deal size that requires the second read.
3. Pick the two escalation numbers you will actually enforce — rank gap and income gap — and put them on the memo template.
4. Add the AI section to the investment or financing memo this week: tool, version, outputs used, outputs changed, certification line.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*

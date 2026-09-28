---
title: "An AI Risk Register for Underwriting Systems"
series: "The Governed AI Series"
part: "Part II — Keep It Accountable"
eyebrow: "KEEP IT ACCOUNTABLE"
deck: "A scored register of what can go wrong when a model sits inside underwriting: likelihood, impact, the control that is supposed to move the score, and the person who owns the row."
author: "Cypress Command"
date: "2026-09-28"
read_time: "11 min"
desk: "own"
status: "review"
source: "practitioner-reference"
---

# An AI Risk Register for Underwriting Systems

"The AI Use Register: Writing Down Where AI Touches the Business" lists where a tool reads, drafts, or suggests. It does not list how the tool can fail. This practitioner reference is that second list for an underwriting system: a scored register, a short deep dive on the failures that actually take down a file, and a cadence so the scores do not freeze on the day you first filled them in. "The Audit Trail: Recording What AI Prepared and What a Person Changed" is the evidence a row points at. The register is the index.

Scores in this article are an illustrative starting matrix for a shopping-center credit or acquisition desk. They are not a measurement of any live model, and they are not a promise that a control will cut risk by the percentage in the table. Replace every number with yours after you have named the control and tested that it works. If the control is a sentence in a policy and not a practice, the residual score does not move.

The register should be readable by the owner, by whoever runs credit, and by counsel before a model output is allowed to influence a live recommendation. On a small desk those may be two people. The document is still mandatory in the sense that you do not skip it. It is not mandatory because a regulator handed you this template.

## How to score a row

Likelihood, 1 through 5, times impact, 1 through 5. Inherent is the score with no control. Residual is the score after the control you actually run. The gap is the only number that tells you whether the control is doing work.

| Rating | Score | What it means on this desk | Who hears about it |
|---|---|---|---|
| Critical | 15–25 | A fair-lending, privacy, or credit-loss event you cannot explain | Owner, the same week |
| High | 10–14 | Active management; a real chance of a bad loan or a bad exam | Owner, next scheduled review |
| Medium | 5–9 | Standard controls, if those controls are real | The person who owns the row |
| Low | 1–4 | Watch it. Do not build a program around it. | The regular report |

A heat map is the same grid drawn for a meeting. It is a conversation, not a decoration. If every row is green, you have not finished the inherent column.

Map the rows to a framework you already claim, and do not claim one you do not run. NIST's AI Risk Management Framework uses a practical set of dimensions that fit this work: validity, safety, security, accountability, transparency, explainability, privacy, and fairness. ISO/IEC 42001 is a management-system standard you can align to; certification is optional and is not assumed here. ECOA, the Fair Housing Act, GLBA, and the EU AI Act are legal regimes that may or may not apply. The register's job is to show which row would matter if they do. Counsel marks applicability. You still write the row.

Four categories keep the list from becoming a junk drawer:

- **Strategic.** Vendor dependency, a rule change, a market the training set never saw.
- **Operational.** Drift, bad inputs, a desk that stopped reading.
- **Compliance.** A statute, a contract, a notice you did not send.
- **Reputational.** A decision you cannot explain to a borrower, a partner, or a lender.

## The system the register assumes

An illustrative system, not a product: a tool that reads owner financials, property performance, tenant mix, and market comps, and returns a risk-scored recommendation on an acquisition, a refinance, or a construction loan. A person makes the credit decision. The tool does not. If your tool only spreads a rent roll, score the rows that fit and mark the rest not applicable. Do not copy a critical rating onto a spreadsheet macro.

## Five rows to write in full

A full register for this kind of system often lands near twenty material rows. Start with the five below. They are the ones that move money or move a regulator. The others — a privacy breach, an explainability gap, a vendor outage, a key-person departure — get a row on the same scale, with an owner, even when you do not give them a scenario essay.

The positions here are teaching scores so the arithmetic is visible. Likelihood 3 times impact 5 is 15. They are not a finding about your model.

| ID | Risk | Illustrative inherent | Illustrative residual | What would have to be true for the residual |
|---|---|---|---|---|
| RISK-001 | Algorithmic bias / fair lending | 3 × 5 = 15, critical | 2 × 3 = 6, medium | The bias test runs, proxies are screened, and a failure stops the output |
| RISK-013 | Training data carries older discriminatory patterns | 3 × 5 = 15, critical | 2 × 4 = 8, medium | You know the years in the training set and have a written treatment for the bad ones |
| RISK-002 | The projection is wrong | 3 × 4 = 12, high | 1 × 4 = 4, low | A variance check forces a person to reconcile model income with a hand calc |
| RISK-005 | The model drifts | 4 × 3 = 12, high | 2 × 2 = 4, low | A threshold pages someone, and retraining has an owner and a date |
| RISK-006 | Humans stop overriding | 3 × 4 = 12, high | 2 × 3 = 6, medium | Override rate and file quality are reviewed, and the model is hidden until the person writes a view |

A 60 percent drop, a 47 percent drop, a 67 percent drop: those are the arithmetic of the teaching scores, not a benchmark you should report as "risk reduction achieved." Report residual scores. If you want a percentage, calculate it from your own grid and label it as movement in the score, not as risk removed from the world.

### RISK-001 Bias

Illustrative scenario: recommendations deny more often in majority-minority tracts after credit factors are controlled. Foot traffic and historic vacancy were the proxies. An investigation under ECOA or the Fair Housing Act is now counsel's problem and your fact pattern.

Treat as an incident if an approval gap above an illustrative 10 percent remains after credit controls, if a fair-lending complaint names the model, or if an auditor flags disparate impact.

1. Stop the affected recommendations. Name the person and the time. Manual underwriting until you know the cause.
2. Within two days, identify the features that move the gap. Counsel reviews the proxy question.
3. Remove or rebuild those features. Retest across the characteristic list before anything goes live.
4. Have someone who did not build the model read the retest.
5. Counsel decides on notice and look-back. The owner hears it in the same cycle, not at the annual offsite.

### RISK-013 The training set remembers

Illustrative scenario: fifteen years of historical decisions, including years when the book itself was uneven. The model learns the old pattern and still posts acceptable accuracy.

Treat as an incident if a data audit finds older decisions with no bias treatment, or if an outside review shows the pattern in the weights.

1. Write the lineage: sources, years, known problems. Thirty days is a reasonable planning clock.
2. Document the correction. Reweighting you cannot explain is not a correction.
3. If you add synthetic files, label them and keep them out of the production performance report.
4. Run the counterfactual from the bias-testing reference.
5. Someone outside the build signs the memo that says the treatment is fit to use.

### RISK-002 The number is wrong

Illustrative scenario, not a live loan: a refinance the model prices off a $24 million story. It returns coverage of 1.42 times because it never discounted an anchor rollover. A person's calc is 1.09 times. If the memo uses 1.42, the desk has approved a different loan than the one in front of it.

Treat as an incident if model and human figures differ by more than an illustrative 15 percent on coverage, loan-to-value, or income; if a default shows the model was materially elsewhere; or if a validation misses the accuracy floor you set.

1. Flag the variance automatically. A senior underwriter reconciles it.
2. Validate against actual performance, not against the last batch of memos. Twice a year is a workable planning cadence.
3. Keep a backtest: projection at origination against the property at 12, 24, and 36 months.
4. Refresh market inputs on a quarter, or say why you do not.
5. Show a range, not a point, when the model is unsure. Train the desk to slow down when the range is wide.

### RISK-005 Drift

Illustrative scenario: a model fit to a calmer year keeps scoring through a year of higher rates and weaker anchors. It does not announce that it is lost.

Treat as an incident if accuracy falls through the floor you set (an illustrative floor used in monitoring designs is 80 percent on a defined task — define the task or do not use the number), if an input distribution shifts past the threshold you set (an illustrative 20 percent shift is a common alert, not a law), or if model-versus-outcome variance worsens for three months.

1. Alert on drift. Population-stability or a divergence measure is enough if someone reads it.
2. Write the floor for each component. An alert with no owner is a log line.
3. Retrain on a calendar, and also when the alert fires or the market breaks.
4. Once a quarter, a person who understands the book reads whether the assumptions still match the street.
5. If you run a challenger model, compare it on a schedule. Promote it only when it wins on the outcomes you care about, including the bias test.

### RISK-006 Nobody is actually reviewing

Illustrative scenario: an examiner samples the files and finds recommendations accepted with no independent note. Override rate near zero. Speed looks like quality.

Treat as an incident if the monthly override rate falls under an illustrative 2 percent, if a sample has no independent analysis, or if an adverse-action reason cannot be tied to a person's work.

A target band of 5 to 15 percent overrides is an illustrative sign of a desk that sometimes disagrees. It is not a quota. A desk that overrides half the time may have a bad model. A desk that overrides none of the time may have stopped reading. Read the files either way.

1. Require the person's view before the model's view is shown.
2. Report the override rate monthly.
3. Sample file quality. Ten percent is a workable planning sample for a large book; a small book can read all of them.
4. Check whether pay or praise rewards speed past documentation.
5. If the sample is thin, stop calling the control effective and move the residual score back up.

## Who owns the row

RACI is worth doing for the rows that can hurt you. Accountable means the name that cannot say "I thought they had it."

| ID | Accountable | Responsible | Consulted | Informed |
|---|---|---|---|---|
| RISK-001 Bias | Compliance owner | The person who runs the test | Counsel; model owner | Owner |
| RISK-002 Accuracy | Credit or risk owner | Model owner; senior underwriter | Validator | Owner |
| RISK-003 Privacy | Security owner | Whoever administers access | Counsel | Owner; affected parties if counsel says so |
| RISK-004 Explainability | Counsel, or the credit owner if you have no counsel on retainer | Model owner; compliance | Outside fair-lending reviewer | Underwriting lead |
| RISK-005 Drift | Model owner | Whoever watches the dashboard | Credit owner | Owner |
| RISK-006 Oversight | Underwriting lead | Senior reviewers; compliance | Credit owner; counsel | Owner |

Titles scale down. "Chief" is optional. A blank accountable cell is not.

## Cadence

Monthly: override rate, variance flags, drift alerts, open incidents. The person responsible for the row speaks; the accountable person hears exceptions, not a tour of the whole register.

Quarterly: residual scores for the critical and high rows, bias ratios, validation status, vendor changes. The owner sees this. A board, if you have one, sees the same page, shorter.

Twice a year: a formal rewrite of the register. New tools, retired tools, controls that turned out to be wishes. "When the Model Changes Under You" is the trigger to open the register between those dates.

An incident does not wait for the month. The deep-dive steps above are the opening move. The register is updated when the residual score changes, not at the next offsite.

## Questions owners ask

**What is this for?** So you can say which failures you have thought about, which controls you claim, and whose name is on each one. Examiners and partners ask that in plainer words than "risk framework."

**How often do we rewrite it?** A full pass twice a year, a quarterly look at the high rows, and any week a model changes or an incident fires.

**Inherent versus residual?** Inherent is the bruise if you do nothing. Residual is the bruise if the control works. If you have not tested the control, report the inherent score.

**Who is on the hook?** The accountable column. The owner of the business is informed on critical rows whether or not the org chart says so.

**Which standard does this match?** It is compatible with the shape of the NIST AI Risk Management Framework and with a clause-6 risk assessment under ISO/IEC 42001. Alignment is not certification, and it is not a legal opinion that ECOA, the Fair Housing Act, GLBA, or the EU AI Act applies to you.

## The practical next step

1. Open a sheet with the five rows in this article. Replace the teaching scores with your own likelihood and impact, and write the control in a sentence next to each one.
2. If you cannot name the person who runs the bias test, the residual score on RISK-001 stays at the inherent score.
3. Add privacy, explainability, and vendor failure as three more rows before you call the register complete.
4. Put the monthly override rate and the variance flag on a calendar someone already looks at.
5. Schedule the first semiannual rewrite now, while the sheet is still short enough to finish.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*

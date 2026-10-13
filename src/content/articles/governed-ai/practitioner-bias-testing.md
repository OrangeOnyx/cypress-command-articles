---
title: "Bias Testing for AI-Assisted CRE Underwriting"
series: "The Governed AI Series"
part: "Part II — Keep It Accountable"
eyebrow: "KEEP IT ACCOUNTABLE"
deck: "A practitioner procedure for testing an underwriting model before it is used and on a schedule after: what to measure, what the thresholds mean, and what to do when a test fails."
author: "Cypress Command"
date: "2026-09-28"
read_time: "13 min"
desk: "buy"
status: "review"
source: "practitioner-reference"
---

# Bias Testing for AI-Assisted CRE Underwriting

The short Governed AI pieces tell an owner to forbid discriminatory outcomes and to keep a person on the decision. They do not show the test. This practitioner reference is the test: which characteristics to examine, which methods to run, which numbers are screens rather than safe harbors, and what to write down when a result fails. "An Acceptable Use Policy for AI in CRE Underwriting" is the rule that this procedure exists. The two should name each other.

Nothing here is a legal conclusion. The Equal Credit Opportunity Act and the Fair Housing Act are real statutes, and they do not have the same lists or the same reach. A shopping-center loan, a residential mortgage, and a tenant-screening tool are not the same product. Counsel decides which law applies, which characteristics are in scope, and whether a result you found is something you must disclose. The operating job is to run the test anyway, on the characteristics a careful desk would be ashamed to skip.

A vendor's bias slide is not your test. If you rely on the output, you own the outcome. Third-party reliance does not move the file off your desk. That point shows up in public statements from the agencies that examine credit and housing; confirm the current guidance with counsel before you quote it to a board.

## What you are testing for

Two different failures get lumped together. Separate them in the write-up.

**Disparate treatment** is the model, or a person using the model, using a protected characteristic. **Disparate impact** is a facially neutral rule that lands harder on a protected group. A coverage floor can do that. So can a feature nobody meant as a demographic variable.

A burden-shifting description practitioners use, and that counsel should confirm against the product you actually offer, runs in three steps. A complainant shows a significant disparity with statistics. The operator shows the practice serves a real, nondiscriminatory business need. The complainant may still show a less discriminatory alternative that predicts about as well. For a model, that third step is why "the feature is predictive" is not the end of the conversation. You should be able to say whether a version without the offending feature still does the job.

**Proxy discrimination** is the neutral feature that tracks a protected characteristic closely enough to smuggle it in.

| Proxy you will actually see | What it can stand in for | Why it shows up in a retail file |
|---|---|---|
| Postal code or census tract | Race, national origin | Segregated geography. Foot traffic and vacancy by tract can do the same work. |
| Length of credit history | Age, thin-file borrowers | Younger sponsors and some income patterns have shorter files. |
| How income is classified | Sex, public assistance, race | Part-time, gig, and benefit income is not evenly distributed. |
| Name fields in a text model | Race, national origin, religion | A language model will infer what you told it not to store. |
| Bedroom count or unit size | Familial status | Matters more when a residential component sits in the collateral. |
| School-quality scores | Race, national origin | School scores track neighborhood composition. Treat them as suspect features, not as amenities. |

## Characteristics to put on the grid

ECOA's credit list is commonly cited as race, color, religion, national origin, sex, marital status, age (with the statute's own limits), receipt of public assistance, and the good-faith exercise of certain consumer-credit rights. The Fair Housing Act's housing list adds familial status and disability and is framed around housing transactions. Citations practitioners keep in the file are 15 U.S.C. § 1691 and 42 U.S.C. § 3604, among others. Do not treat this paragraph as the list for your product. Ask counsel for the list, then test at least that list.

For a CRE credit file, write one sentence of relevance next to each row so the test is not abstract: guarantor requirements that differ by sex, income that is discounted because of its source, a name field the model can read, a tract feature that tracks race, a unit-mix feature that tracks families with children, an accessibility adjustment used only as a negative.

## Methods that belong in the file

Run more than one. A single ratio can hide what a regression shows, and the reverse.

- **Disparate impact ratio.** Favorable-outcome rate for a protected group divided by the rate for the highest group, or for a defined control. This is the figure people call the adverse impact ratio.
- **A chi-square test of independence.** Whether outcome and group membership are associated. A conventional screen is p < 0.05, and some high-stakes desks use p < 0.01. The formula is the usual sum of squared differences between observed and expected counts, scaled by the expected count. The p-value is a screen for "this is unlikely to be noise," not a finding of liability.
- **A regression that controls for legitimate credit factors.** If group membership still predicts the outcome after those factors, you have a question, not a clean model.
- **Matched comparison.** Pair files that look alike on credit characteristics and differ on group, so the comparison is not just "different deals."

Define the population before you calculate. Twelve months of decisions is a workable minimum window when you have the volume. Assign group membership from data you are allowed to use for testing — and document the method. Self-identification, where you have it, is cleaner than an inference method. If you use a proxy such as a Bayesian name-and-geography estimate, say so, and do not then pretend the label is a fact about a person. Stratify by loan type, size, and structure so a grocery anchor is not compared with a vacant strip as if they were the same experiment.

Screen every feature for correlation with a protected characteristic or with a proxy score:

| Feature type | Screen | Illustrative concern line | What you do |
|---|---|---|---|
| Continuous | Correlation with a proxy score | Absolute value above 0.30 | Bias review |
| Categorical | Association measure such as Cramér's V | Above 0.25 | Try the model without the feature |
| Geographic | Fit against census composition | R² above 0.20 | Rebuild the feature or drop it |
| Text | Can the feature predict a protected class on a labeled holdout? | AUC above 0.65 | Remove or strip the feature |

Those lines are operating screens for this draft, not regulatory limits. A feature under the line can still be a problem. A feature over the line is a mandatory conversation, not an automatic violation.

Test intersections, not only single characteristics: race and sex, race and age, national origin and income type, familial status and race, age and marital status. When a cell has fewer than 30 files, do not skip it and do not pretend the ratio is precise. Read every denial in the cell, and pool time periods until the count is honest.

A counterfactual check asks whether the output moves when the protected characteristic changes and the credit facts do not. If more than an illustrative 10 percent of pairs move in a way you cannot explain, stop and remediate before the next live decision of that type.

| Method | Use it for | Illustrative minimum | Cadence | Owner |
|---|---|---|---|---|
| Disparate impact ratio | Approve and deny rates | 30 per group | Quarterly | Whoever runs the numbers |
| Chi-square or a proportion test | Whether the gap is noise | Enough for the test you chose | Quarterly | Same |
| Regression with controls | Leftover group effect | A real book, not a toy sample | At least annually, and before deployment | Same, with the credit owner reading it |
| Matched pairs | Isolating group membership | Enough close pairs to mean something | Before deployment, and after a material change | Same |
| Counterfactual | Does the score move when only the protected field moves? | A documented sample | Before deployment | Same |
| Feature-correlation screen | Proxies | The whole feature list | Before deployment, and when features change | Same |

"Data science" on a small desk may be one outside analyst. Name the person. The underwriting owner still signs the memo that says the test was read.

## The 80 percent figure, and what it is not

The adverse impact ratio is selection rate in the protected group divided by selection rate in the comparison group. An illustrative pass screen used in a lot of templates is 0.80. The figure comes from federal employment-selection guidance, the four-fifths rule. It is a screen. It is not a safe harbor for credit, and an agency can still find a problem above 0.80 if other evidence is there. A result just under 0.80, on a tiny sample, is not automatically a violation either. Write both sentences into the procedure so nobody treats the ratio as a verdict.

Use a second look at practical size. Cohen's d, or a simpler rate gap, tells you whether a statistically detectable difference in a continuous outcome — a spread, a proceeds figure — is large enough to matter. Set the bands in the test plan before you see the results.

| Measure | Illustrative watch band | Illustrative fail for this procedure |
|---|---|---|
| Adverse impact ratio | 0.80 to 0.85 | Below 0.80, investigate |
| Approval-rate gap you cannot explain | — | Above 10 percent after credit controls, treat as an incident trigger |
| Denial multiple | 1.25 times the comparison group | 1.50 times, escalate |
| Severe ratio | — | Below 0.60, stop that decision type until the model is rebuilt |

The 10 percent approval gap and the 0.60 severe line are operating triggers for this draft so a desk has somewhere to start. They are not case law. Counsel and your fair-lending reviewer should replace them with the triggers you are willing to defend.

## Data you need before the test means anything

Do not run a test on a month of files and call it a program. Power and minimum cell size belong in the plan. If you cannot reach them, say the test is inconclusive and add the qualitative review. Do not fill the gap with a precise-looking ratio.

Synthetic files are allowed for a pre-deployment dry run when you do not yet have outcomes. Label them synthetic. Do not mix them into the production monitoring report as if they were your book.

A short data check before anyone calculates: the outcome is defined (approve, deny, price — pick one and stick to it), declined-incomplete files are handled the same way in every group, the period is stated, missing group data is counted rather than dropped quietly, and the person who pulled the extract is not the only person who reads the result.

## When you run it

**Before deployment.** Every method in the table that applies, on all in-scope characteristics, with the feature screen attached. No live reliance until the credit owner and the compliance owner have both signed the test memo.

**On a schedule.** Quarterly ratios and a short exception log. A fuller regression and matched review at least annually. The monitoring reference in "When the Model Changes Under You" is the companion for ordinary model updates. A material change is not ordinary.

**Immediately**, without waiting for the quarter, when any of these happen: a new feature, a new training set, a vendor model version, a fair-lending complaint, a disparity a portfolio review stumbled into, a product change (you started pricing, not only spreading), or an examiner's question.

## When a test fails

Classify the miss before you argue about it.

| Severity | Illustrative meaning | First move |
|---|---|---|
| Watch | Inside the watch band, or a small cell | Document, keep monitoring, do not "fix" the data |
| Investigate | Below 0.80, or a significant regression coefficient you cannot explain | Freeze new reliance for that decision type until the cause is written |
| Severe | Below 0.60, or a complaint plus a confirming statistic | Stop the model output for that decision type; manual underwriting until a rebuild is validated |

Cause work is specific. Which feature moves the outcome? Is it a proxy? Is the training set an older book with older habits? Is a person overriding in one direction? A five-step path that matches the risk-register playbook:

1. Stop the affected output if the severity calls for it. Write the time and the name.
2. Find the feature. Importance plots are a start. A model without the feature is the test.
3. Rebuild. Remove or rebuild the proxy. If the training history itself is the problem, do not "reweight" it quietly and move on. Document what you changed.
4. Retest, including the intersection cells, before the output returns.
5. Have someone who did not build the model read the retest. Counsel decides on notice, look-back, and anything you say to an applicant.

Overrides of a biased output are allowed only on the human-oversight protocol, with a reason, and never as a way to keep a failing model in production "for now."

## What the file contains

A test plan written before the run: population, outcomes, groups, methods, thresholds, owner. Results with the formulas applied, not only a dashboard screenshot. The remediation log: date found, severity, change made, retest result, who signed. Retention of at least five years is a planning default in this suite; your actual schedule is the one counsel and the recordkeeping rule for the product require. An EU high-risk logging duty, if it applies, can be longer. Do not assume five years is the ceiling.

Quarterly, the compliance owner should be able to show one table: adverse impact ratio by characteristic, against the prior quarter, with every group either at or above the pass screen or already inside an open remediation.

## Who signs

The person who calculates does not approve their own result. A workable three-step review: the analyst completes the test, the credit or model owner agrees the business explanation is real, and the compliance owner accepts the result or sends it back. A board or ownership report each quarter needs only the ratios, the open remediations, and whether any model is currently stopped. It does not need the chi-square formula.

If an examiner or a lender asks, the packet is the plan, the results, the log, and the name of the person who can explain a row. Vendor paperwork can be an exhibit. It cannot be the packet.

## Questions operators ask

**Why test if we never collect race on a commercial file?** Because proxies do not need the field. Geography, names, and income type can carry it. And because "we did not collect it" is a weak sentence if the outcomes still split.

**Can we rely on the vendor's test?** You can read it. You still run yours on your book, your overrides, and your products. Their test was not your applicants.

**The model does not use protected characteristics.** That is the start of the proxy section, not the end of the work.

**How often?** Before go-live, quarterly for the ratios, annually for the deeper tests, and the same week a material change or a complaint arrives.

**A test failed. Now what?** Severity first, then stop or investigate as the table says. Do not retrain in a way you cannot explain and call it fixed.

**What do we keep?** The plan, the numbers, the change log, and the names. Five years unless counsel sets a longer clock.

**Who owns it?** A named calculator, a named credit owner, and a named compliance owner. One person may hold two of those seats on a small desk. Nobody holds all three and also builds the model.

## The practical next step

1. Ask counsel for the characteristic list that applies to the product you actually originate. Write it at the top of the test plan.
2. List every model feature. Mark geography, name, income type, and anything derived from them as suspect until the screen says otherwise.
3. Compute one adverse impact ratio on the last twelve months of approvals, with the cell counts visible. If a cell is under 30, say so.
4. Put the 0.80 line in the procedure as a screen, and write the sentence that it is not a safe harbor next to it.
5. Name the three signers before the next model change, not after.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*
